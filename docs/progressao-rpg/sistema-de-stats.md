# Sistema de Stats e Progressão RPG (Classless)

## Visão Geral

O sistema de crescimento de personagem do **MineCraftSoul** é **classless** (sem classes travadas). O jogador sobe de nível livremente e distribui pontos de atributo como quiser, criando builds únicas e criativas.

O foco é em **combinações de stats** para criar skills poderosas, em vez de escolher uma classe no início.

---

## Stats Principais

Usaremos **5 atributos clássicos** de RPG antigo, adaptados para Minecraft:

| Atributo       | Nome Curto | Efeito Principal                              | Efeito Secundário                     | Recomendado para          |
|----------------|------------|-----------------------------------------------|----------------------------------------|---------------------------|
| **Força**     | STR       | Dano físico melee                             | Capacidade de carga, requisitos de arma | Tanques, melee bruto     |
| **Constituição** | CON     | Vida máxima + Regeneração                 | Resistência a dano físico            | Tanques, sobrevivência   |
| **Destreza**   | DEX       | Velocidade de ataque + Chance de crítico   | Dano ranged, esquiva, precisão       | DPS ranged / melee ágil |
| **Inteligência** | INT    | Dano mágico + Mana máxima                  | Potência de skills                   | Mages, skills híbridas  |
| **Sabedoria**  | WIS       | Resistência mágica + Cura                   | Regeneração de mana, percepção     | Suporte, híbridos       |

> **Importante**: Não há trava de classe. Um jogador pode colocar pontos em qualquer combinação que quiser (ex: Força + Inteligência = guerreiro mágico).

---

## Como Funciona o Ganho de Pontos

A cada level up o jogador recebe:

- **Pontos de Atributo** (para distribuir nos 5 stats acima)
- **Pontos de Skill** (para desbloquear/habilidades ativas ou passivas)

### Exemplo de Progressão

| Nível | Pontos de Atributo por level | Pontos de Skill por level | Total aproximado de pontos de atributo aos 50 |
|----------|------------------------------|---------------------------|--------------------------------------------------|
| 1~10    | 4                            | 2                         | ~36                                              |
| 11~30   | 3                            | 2                         | ~96                                              |
| 31~50   | 2                            | 1                         | ~136                                             |

> Os valores exatos serão ajustados durante o balanceamento.

---

## Skills Combinadas (o coração do sistema)

Em vez de skills fixas por classe, criaremos skills que **escalam com múltiplos atributos** ao mesmo tempo.

Isso permite builds muito mais criativas e recompensadoras.

### Exemplos de Skills Combinadas

| Skill                | Stats que escalam          | Tipo de Dano          | Efeito Especial                     | Build Exemplo              |
|----------------------|----------------------------|-----------------------|-------------------------------------|----------------------------|
| Golpe Brutal        | Força + Constituição   | Físico               | Ganha vida temporária              | Tanque melee               |
| Lâmina Arcana      | Força + Inteligência    | Físico + Mágico     | Dano extra de fogo/arcano         | Guerreiro-mago             |
| Tiro Perfurante     | Destreza + Inteligência  | Ranged + Mágico     | Penetração de armadura            | Arqueiro mágico           |
| Investida Sombria   | Destreza + Constituição | Físico               | Esquiva + dano aumentado            | Assassino / Agil           |
| Erupção Arcana    | Inteligência + Sabedoria | Mágico                | Área + cura aliados próximos      | Mage suporte               |
| Martelo Divino      | Força + Sabedoria        | Físico + Sagrado     | Stun + bônus de cura próprio      | Paladino híbrido          |

Essas skills serão implementadas via **AuraSkills** + custom skills (usando MythicMobs ou scripts quando necessário).

---

## Integração com AuraSkills

Usaremos o plugin **AuraSkills** como base do sistema.

- Stats customizados serão criados
- O menu de distribuição de pontos será feito com **DeluxeMenus**
- Skills serão registradas no AuraSkills
- Itens custom (ItemsAdder) poderão ter requisitos de atributo

---

## Próximos Passos

1. Definir valores exatos de ganho de pontos por level
2. Criar as primeiras 6~8 skills combinadas
3. Gerar a configuração inicial do AuraSkills
4. Criar o menu de distribuição de pontos (DeluxeMenus)
5. Testar no servidor

---

**Status**: Em desenvolvimento ativo