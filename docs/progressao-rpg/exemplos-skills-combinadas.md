# Exemplos de Skills Combinadas

## Conceito

Skills que escalam com **dois ou mais atributos** ao mesmo tempo. Isso é o que permite builds realmente criativas e recompensadoras.

## Skills de Dano Físico / Híbrido

### 1. Golpe Brutal (Força + Constituição)

- **Dano base**: Alto
- **Escala**: 1.2x Força + 0.8x Constituição
- **Efeito especial**: Ganha escudo de vida temporária (15% do dano causado)
- **Cooldown**: 8 segundos
- **Build ideal**: Tanque melee agressivo

### 2. Lâmina Arcana (Força + Inteligência)

- **Dano**: Físico + Mágico (metade de cada)
- **Escala**: 1.0x Força + 1.0x Inteligência
- **Efeito especial**: Aplica queimadura (dano ao longo do tempo)
- **Build ideal**: Guerreiro-mago, paladino sombrio

### 3. Tiro Perfurante (Destreza + Inteligência)

- **Dano**: Ranged + Mágico
- **Escala**: 1.3x Destreza + 0.9x Inteligência
- **Efeito especial**: Ignora 30% da armadura do alvo
- **Build ideal**: Arqueiro mágico / Ranger arcano

### 4. Investida Sombria (Destreza + Constituição)

- **Dano**: Médio-Alto
- **Escala**: 1.1x Destreza + 0.7x Constituição
- **Efeito especial**: Aumenta esquiva por 4 segundos após o uso + empurra inimigos
- **Build ideal**: Assassino / Duelista ágil

## Skills de Área / Suporte

### 5. Erupção Arcana (Inteligência + Sabedoria)

- **Dano**: Mágico em área
- **Escala**: 1.4x Inteligência + 0.6x Sabedoria
- **Efeito especial**: Cura aliados próximos em 40% do dano causado
- **Build ideal**: Mage de batalha / Suporte ofensivo

### 6. Martelo Divino (Força + Sabedoria)

- **Dano**: Físico + Sagrado
- **Escala**: 1.0x Força + 1.0x Sabedoria
- **Efeito especial**: Stun de 1.5s + pequena cura próprio
- **Build ideal**: Paladino / Tank suporte

---

## Como serão implementadas

- As skills mais simples começarão como **habilidades do AuraSkills**
- Skills mais complexas (com efeitos especiais) serão feitas com **MythicMobs skills** ou scripts custom
- O scaling com múltiplos stats será feito via placeholders do PlaceholderAPI

**Status**: Conceito pronto. Próximo passo: implementar as primeiras 3 skills no servidor de teste.