# Implementação das Primeiras Skills Combinadas

**Data:** Julho 2026
**Status:** Implementado (Opção A)

## Skills Criadas

Foram implementadas as primeiras 4 skills combinadas reais no formato AuraSkills:

| Skill                | Atributos Principais      | Estilo de Jogo          | Nível Máx |
|----------------------|---------------------------|-------------------------|---------------|
| Golpe Brutal        | Força + Destreza        | Melee Burst + Stun     | 20            |
| Lâmina Flamejante | Força + Inteligência   | Melee + DoT (Fogo)     | 20            |
| Tiro Preciso        | Destreza + Inteligência | Ranged / Mágico       | 20            |
| Investida Brutal    | Constituição + Força  | Tank + Engage + Sustain| 15            |

## Como as fórmulas funcionam

As fórmulas usam os placeholders do AuraSkills:

- `player_strength`
- `player_constitution`
- `player_dexterity`
- `player_intelligence`
- `player_wisdom`

Exemplo de fórmula:
```yaml
daño: "(player_strength * 2.8) + (player_dexterity * 1.4) + (level * 4)"
```

Isso faz com que a skill fique forte tanto em builds puras quanto em builds híbridas.

## Próximos Passos Recomendados

1. Testar essas skills no servidor com o AuraSkills instalado.
2. Ajustar os valores de scaling (multiplicadores) conforme o balanceamento desejado.
3. Criar mais skills (especialmente de suporte e utility).
4. Criar skills de tier mais alto (level 25~40) com efeitos mais poderosos.
5. Integrar com o sistema de Almas/Ecos (morte com risco).
