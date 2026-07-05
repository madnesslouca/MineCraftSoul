# Sistema de Almas / Ecos (Souls-like)

## Filosofia do Sistema

Este sistema é inspirado diretamente em Dark Souls / Elden Ring. O objetivo é criar **tensão real** toda vez que o jogador morre, sem ser frustrante demais.

**Regras principais:**

- Ao morrer, o jogador **dropa a maior parte das suas Almas** no local da morte.
- Uma pequena porcentagem é **perdida permanentemente** (risco).
- O jogador pode voltar ao local e recuperar as Almas.
- Se morrer novamente antes de recuperar → perde as Almas dropadas + nova porcentagem.
- Almas servem como **moeda de risco/recompensa** e podem ser gastas em melhorias, crafting especial ou rituais.

---

## Como Funciona (Fluxo Completo)

### 1. Quando o Jogador Morre

1. O sistema calcula:
   - `Almas_Perdas_Permanente` = Total_Almas * 0.15 (15% perdido para sempre)
   - `Almas_Dropadas` = Total_Almas - Almas_Perdas_Permanente

2. As `Almas_Dropadas` são armazenadas em um **Eco da Alma** que aparece no local exato da morte.

3. O jogador renasce no último checkpoint (cama ou spawn configurado).

4. Uma mensagem aparece:
   > "Você perdeu 15% das suas Almas... Um Eco da Alma foi deixado para trás."

### 2. O Eco da Alma

- É uma entidade flutuante (MythicMobs) com visual de alma brilhante.
- Mostra via hologram ou bossbar a quantidade de Almas que contém.
- Pode ser **interagido com clique direito** para recuperar tudo.
- Tem tempo de vida de **12 minutos**. Depois disso some e as Almas são perdidas.
- Só o dono original pode recuperar (ou grupo, se configurado).

### 3. Se o Jogador Morrer Novamente (antes de recuperar)

- Perde as Almas do Eco anterior permanentemente.
- Novo Eco é criado com as novas Almas.

### 4. Uso das Almas

As Almas podem ser usadas para:
- Comprar itens raros de NPCs
- Melhorar equipamentos (affixes)
- Pagar rituais de reforjamento
- Desbloquear skills mais poderosas
- Como requisito de entrada em masmorras de alto nível

---

## Implementação Técnica (Stack Atual)

### Plugins Necessários

| Plugin       | Finalidade                          | Obrigatório? |
|--------------|-------------------------------------|------------------|
| MythicMobs   | Criar o "Eco da Alma" como entidade | Sim             |
| Skript       | Detectar morte e spawnar o Eco     | **Altamente recomendado** |
| PlaceholderAPI | Mostrar quantidade de Almas       | Sim             |
| BossBarAPI ou similar | Mostrar barra flutuante       | Recomendado     |

### Por que Skript?

Skript é leve, fácil de editar e perfeito para mecânicas complexas de morte sem precisar programar um plugin Java do zero. A maioria dos servidores Souls-like no Minecraft usa Skript ou um plugin custom para isso.

---

## Config do MythicMobs - Eco da Alma

Arquivo: `configs/mythicmobs/mobs/eco-da-alma.yml`

```yaml
eco_da_alma:
  Type: ALLAY
  Display: '&dEco da Alma'
  Health: 1
  Damage: 0
  Options:
    Silent: true
    Invincible: true
    NoAI: true
    Glowing: true
    Persistent: false
  AIGoalSelectors:
    - clear
  AITargetSelectors:
    - clear
  Skills:
    - message{msg="&dClique direito para recuperar suas Almas!"; radius=3} @Trigger
    - effect:particles{particle=SOUL; amount=15; speed=0.05} @Trigger
  Drops:
    - nothing
  Equipment:
    helmet: SOUL_LANTERN
```

**Observações:**
- Usamos Allay como base (leve e flutua).
- Glow + partículas de alma para visual bonito.
- Sem IA para não fugir.
- Tempo de vida deve ser controlado via Skript (despawn após 12 minutos).

---

## Exemplo Básico de Skript (on death)

Crie um arquivo em `plugins/Skript/scripts/almas-ecos.sk`

```sk
on death of player:
  set {_player} to victim
  set {_almas} to {almas::%{_player}%} or 0
  if {_almas} > 0:
    set {_perda} to {_almas} * 0.15
    set {_drop} to {_almas} - {_perda}
    
    # Remove as almas do jogador
    set {almas::%{_player}%} to 0
    
    # Cria o Eco da Alma na localização da morte
    spawn "EcoDaAlma" at location of victim
    set {_eco} to last spawned entity
    
    # Armazena quantas almas esse eco tem (usando scoreboard ou metadata)
    set metadata value "almas" of {_eco} to {_drop}
    set metadata value "owner" of {_eco} to {_player}'s uuid
    
    # Mensagem pro jogador
    send "&cVocê morreu... &7Perdeu &c%{_perda}% &7Almas permanentemente." to {_player}
    send "&dUm Eco da Alma foi deixado no local da sua morte. Você tem 12 minutos para recuperar." to {_player}
    
    # Agenda o despawn do eco após 12 minutos (720 segundos)
    wait 720 seconds
    if {_eco} is set:
      kill {_eco}
      send "&7O Eco da Alma desapareceu... as almas foram perdidas." to {_player}
```

**Nota:** Este é um exemplo inicial. Podemos refinar bastante (adicionar bossbar flutuante, som, partículas constantes, verificar se o jogador ainda está online, etc).

---

## Próximos Passos de Implementação

1. Adicionar o plugin **Skript** no servidor
2. Instalar **MythicMobs** (já estamos usando)
3. Criar o mob `eco_da_alma` no MythicMobs
4. Criar o script Skript acima (vamos melhorar ele juntos)
5. Testar o fluxo completo de morte + recuperação
6. Integrar as Almas com o sistema de compra / crafting

---

## Integração com o Resto do Projeto

- **AuraSkills**: Podemos fazer as Almas serem ganhas ao subir de level ou ao matar mobs.
- **MythicMobs Bosses**: Bosses podem dropar Almas em quantidade maior.
- **Loja de NPCs**: Usar Almas como moeda especial.
- **Masmorras**: Algumas masmorras podem exigir uma quantidade mínima de Almas para entrar (risco).

Este sistema vai dar um peso muito maior às mortes nas masmorras e bosses que estamos criando.
