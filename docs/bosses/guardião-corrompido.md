# Guardião Corrompido

**Primeiro Boss Principal** das Catacumbas do Véu Rasgado

## Visão Geral

O Guardião Corrompido é o que resta de um antigo protetor do Véu que guardava a entrada para o plano espiritual. Após a grande ruptura, ele foi consumido pela corrupção de almas e agora vaga pela arena circular no terceiro andar das catacumbas.

- **Nível Recomendado:** 15 ~ 25
- **Tamanho de Grupo Sugerido:** 3~5 jogadores
- **Dificuldade:** Média-Alta (estilo Souls)
- **Localização:** Arena Circular (Andar 3) - Catacumbas do Véu Rasgado

## Lore

Antigamente conhecido como "Guardião do Véu", ele era responsável por manter o equilíbrio entre o mundo mortal e o plano das almas. Quando o Véu foi rasgado, a corrupção o alcançou primeiro. Agora ele está preso em um ciclo eterno de dor e fúria, atacando qualquer um que ousa entrar em sua arena.

## Mecânicas Gerais (Souls-like)

- Padrões bem telegráficos (partículas + sons + animação)
- 3 Fases distintas com transições claras
- Arena interativa (pilares destrutíveis + lava central)
- Sistema de threat (foca quem mais causa dano)
- Adds em momentos específicos
- Punição por posicionamento ruim

## Fases do Combate

### Fase 1: "O Despertar do Guardião" (100% ~ 60% HP)

**Estilo:** Melee pesado + summons iniciais

**Ataques Principais:**

1. **Golpe Pesado** (telegráfico claro)
   - O boss levanta o braço por 1.2s (partículas roxas + som grave)
   - Causa dano alto em cone frontal + knockback
   - Jogadores devem desviar para os lados

2. **Combo de 3 Golpes**
   - Sequência rápida de 3 ataques melee
   - O terceiro golpe é mais forte e causa stun curto se acertar

3. **Invocação de Almas Corrompidas** (a cada 25% HP perdido ou timer)
   - Invoca 2~3 adds pequenos (Almas Corrompidas)
   - Adds são fracos mas causam slow se acertarem
   - Devem ser priorizados ou o boss ganha bônus de dano

**Transição para Fase 2:**
Quando chega em 60% HP, o boss para, grita (som + partículas), e a lava começa a subir lentamente no centro da arena.

### Fase 2: "A Fenda se Abre" (60% ~ 30% HP)

**Estilo:** Misto (melee + ranged) + arena muda

**Ataques Principais:**

1. **Projétil de Alma** (ranged)
   - Dispara 3 projéteis em arco que causam dano mágico + slow
   - Telegráfico: boss aponta o braço e acumula energia roxa

2. **Erupção de Almas** (ataque grande)
   - Boss canaliza por 2.5s (partículas intensas)
   - Libera uma onda de almas em 360° ou em cone amplo
   - Causa dano médio-alto + fear curto
   - Jogadores devem se esconder atrás dos pilares ou desviar

3. **Destruição de Pilar** (mecânica de arena)
   - De tempos em tempos o boss foca um pilar aleatório e o destrói após 3s
   - Quando um pilar é destruído, cria uma zona segura temporária (lava não sobe ali) ou pode ser usado para interromper o boss

**Transição para Fase 3:**
Aos 30% HP o boss entra em fúria. A lava sobe mais rápido e ele fica visivelmente mais agressivo (partículas vermelhas + velocidade aumentada).

### Fase 3: "Véu Rasgado" (< 30% HP)

**Estilo:** Desespero + alta mobilidade

**Ataques Principais:**

1. **Investida Furiosa**
   - Boss corre em linha reta em direção ao jogador com mais threat
   - Causa dano + empurrão forte
   - Deixa rastro de lava temporário

2. **Tempestade de Almas** (Ultimate)
   - Canaliza por 4 segundos
   - Várias ondas de projéteis + AOE crescente no centro
   - Jogadores precisam destruir os pilares restantes ou ficar em zonas seguras para sobreviver
   - Se não interrompido, causa wipe quase certo no grupo

3. **Summon Final**
   - Invoca 1 add maior ("Eco do Guardião") que tem bastante vida e causa dano em área

**Derrota:**
Ao morrer, o boss explode em uma grande liberação de almas (efeito visual bonito) e dropa o loot + almas para o sistema de recuperação.

## Recompensas e Loot

### Drops Principais (ItemsAdder)

| Item | Chance | Quantidade | Descrição |
|------|--------|------------|---------|
| **Lâmina do Véu Corrompido** | 35% | 1 | Espada híbrida que escala com **Força + Inteligência**. Causa dano melee + chance de Queimadura de Alma (DoT). |
| **Elmo do Guardião Corrompido** | 40% | 1 | Capacete tanque com alto bônus de **Constituição** e resistência mágica. |
| **Anel da Alma Presa** | 25% | 1 | Acessório que dá bônus de **Inteligência + Sabedoria** e dano extra contra mobs corrompidos. |
| **Fragmento do Véu Rasgado** | 80% | 1~3 | Material raro de crafting. Usado para forjar equipamentos de tiers superiores. |

### Integração com Sistema de Stats

Todos os itens acima têm **requisitos de atributo** e **bônus escaláveis** com o sistema de AuraSkills:

- **Lâmina do Véu Corrompido** → Requer Força 12 + Inteligência 10
- **Elmo do Guardião Corrompido** → Requer Constituição 14

### Sistema de Almas (Estilo Souls)

- Grande quantidade de **Ecos de Alma** (para o sistema de morte com risco)
- O boss dropa almas no local da morte que podem ser recuperadas

### Experiência

Alta quantidade de XP (bom para subir de nível rápido no early-mid game).

## Dicas de Combate

- Fase 1: Foque em adds quando aparecem e aprenda o timing do Golpe Pesado.
- Fase 2: Use os pilares como cobertura. Não fique no centro quando a lava subir.
- Fase 3: Priorize interrupção da Tempestade de Almas destruindo pilares ou causando muito dano no boss.
- Builds híbridas funcionam muito bem (Força + Inteligência ou Destreza + Sabedoria).

## Status Base (MythicMobs)

**Tuning brutal**: mesmo com grupo de 4 (nível 15~25) o wipe nas primeiras tentativas é o esperado. O boss é um "muro" que empurra o grupo a upar, explorar e voltar mais forte — filosofia Souls.

- **Vida:** 12000 (~5 a 7 min de luta para grupo coordenado)
- **Dano (melee básico):** 22
- **Defesa (Armor):** 16
- **Velocidade:** 0.28 (Velocidade II + Força II permanentes na Fase 3)
- **Aggro:** ThreatTable ativa (tanque consegue segurar o boss)
- **Anti-cheese:** imune a fogo/lava/queda/veneno/wither; dano de projétil reduzido a 60%

### Mecânicas de arena e punição (v2)

- **Chuva de Almas** (Fase 2+): zonas corrompidas surgem na posição de cada jogador — telegraph de anel, erupção e poça persistente de 10s (dano + Lentidão III) que nega área.
- **Olhar do Véu** (Fase 2+): após 2,5s de canalização, causa 55 de dano a todo jogador na **linha de visão** do boss. Substitui a antiga "Destruição de Pilar": os pilares agora importam porque bloqueiam o Olhar do Véu e a Tempestade de Almas (4 ondas, também por linha de visão).
- **Represália**: 12% de chance de contra-ataque em 180° ao ser golpeado de perto — spam de ataque colado no boss é aposta perigosa.
- **Agarrão**: quem gruda no boss ignorando o moveset toma 38 de dano e é arremessado.
- **Investida dupla** (Fase 3): dois dashes em sequência; o segundo pune quem relaxa após esquivar o primeiro.

> Configs: `configs/mythicmobs/bosses/guardiao-corrompido.yml` (mobs) e `configs/mythicmobs/skills/guardiao-corrompido-skills.yml` (metaskills). ID interno do mob: `GuardiaoCorrompido` (sem acento).

---

*Boss criado para o projeto MineCraftSoul - RPG Souls-like em Minecraft*