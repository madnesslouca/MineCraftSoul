# Sistema de Progressão RPG - MineCraftSoul

## Filosofia

Sem classes fixas. O jogador ganha **pontos de atributo** a cada level up e distribui livremente entre os stats. Isso permite combinações criativas e builds únicas.

## Stats Principais

| Stat            | Efeito Principal                          | Exemplos de Skills que escalam com ele |
|-----------------|-------------------------------------------|----------------------------------------|
| **Força**      | Dano melee, capacidade de carga, stun     | Golpe Poderoso, Investida Brutal       |
| **Constituição** | Vida máxima, regeneração, resistência   | Tanque, skills de sobrevivência       |
| **Destreza**    | Velocidade de ataque, chance crítico, esquiva, dano ranged | Tiro Preciso, Lâmina Rápida         |
| **Inteligência** | Dano mágico, mana, potência de skills   | Lâmina Flamejante, Bola de Fogo       |
| **Sabedoria**   | Resistência mágica, cura, mana regen     | Cura, Escudo Mágico                   |

## Como funciona o ganho de pontos

- A cada level up o jogador recebe:
  - **X pontos de atributo** (configurável)
  - **Y pontos de skill** (para desbloquear habilidades)

- O jogador abre um menu (DeluxeMenus) e distribui os pontos livremente.

## Skills Combinadas (exemplos)

- **Golpe Poderoso**: Escala com Força + Destreza
- **Lâmina Flamejante**: Escala com Força + Inteligência (dano físico + fogo)
- **Investida Brutal**: Escala com Constituição + Força
- **Tiro Preciso**: Escala com Destreza + Inteligência

## Próximos Passos

1. Configurar AuraSkills com esses stats
2. Criar o menu de distribuição de pontos
3. Implementar as primeiras skills
