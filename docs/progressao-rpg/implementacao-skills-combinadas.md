# Implementação das Skills Combinadas

**Data:** Julho 2026
**Status:** Expandido (Opção D)

## Skills Atuais no Repositório

Foram implementadas **9 skills combinadas** até o momento:

### Fase 1 (Opção A)

| Skill                | Atributos Principais      | Estilo de Jogo                  | Nível Máx |
|----------------------|---------------------------|----------------------------------|---------------|
| Golpe Brutal        | Força + Destreza        | Melee Burst + Stun              | 20            |
| Lâmina Flamejante | Força + Inteligência   | Melee + DoT (Fogo)              | 20            |
| Tiro Preciso        | Destreza + Inteligência | Ranged / Mágico               | 20            |
| Investida Brutal    | Constituição + Força  | Tank + Engage + Sustain         | 15            |

### Fase 2 (Opção D)

| Skill                | Atributos Principais         | Estilo de Jogo                     | Nível Máx |
|----------------------|------------------------------|------------------------------------|---------------|
| **Golpe Sísmico**   | Força + Constituição     | Melee AoE + Knockback             | 20            |
| **Escudo Arcano**    | Constituição + Inteligência | Defesa + Reflexão de dano        | 15            |
| **Rajada Arcana**    | Destreza + Inteligência    | Ranged Mágico + Slow             | 20            |
| **Dança das Lâminas** | Destreza + Força         | Multi-hit AoE melee               | 18            |
| **Cura Rúnica**     | Sabedoria + Inteligência   | Cura + HoT (Regeneração)       | 15            |

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

Isso faz com que a skill fique forte tanto em builds puras quanto em builds híbridas criativas.

## Filosofia das Skills

- Sem travas de classe
- Combinações de 2 atributos por skill
- Incentiva builds híbridas (ex: Força + Inteligência = guerreiro mágico)
- Cada skill tem identidade clara

## Próximos Passos Recomendados

1. Testar todas as 9 skills no servidor.
2. Ajustar multiplicadores conforme o balanceamento do servidor.
3. Criar skills de tier mais alto (nível 25~40).
4. Adicionar skills de utility / mobilidade / crowd control.
5. Integrar com o Sistema de Almas/Ecos.
6. Criar versões "Ultimate" das skills principais.
