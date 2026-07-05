# Implementação das Skills Combinadas

**Data:** Julho 2026  
**Status:** Balanceamento Concluído (Opção D.1)

## Skills Atuais no Repositório

Foram implementadas **9 skills combinadas** e balanceadas:

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

## Balanceamento Realizado (D.1)

### Principais Ajustes:

- **Requisitos de atributo** mais acessíveis no early game (reduzidos de 15~20 para 8~12)
- **Curva de dano** mais equilibrada (multiplicadores ajustados para não serem fortes demais no late game)
- **Mana cost** mais consistente entre as skills
- **Cooldowns** com melhor progressão (escalam com o nível da skill)
- Adicionado `level-requirement` em todas as skills
- Melhorias nas descrições e feedback visual
- Ajustes finos em chance de efeitos (stun, slow, reflect)

## Como as fórmulas funcionam

As fórmulas usam os placeholders do AuraSkills:

- `player_strength`
- `player_constitution`
- `player_dexterity`
- `player_intelligence`
- `player_wisdom`

Exemplo de fórmula balanceada:
```yaml
daño: "(player_strength * 2.4) + (player_dexterity * 1.3) + (level * 3.5)"
```

Isso faz com que a skill fique forte tanto em builds puras quanto em builds híbridas criativas, sem quebrar o jogo.

## Filosofia das Skills

- Sem travas de classe
- Combinações de 2 atributos por skill
- Incentiva builds híbridas (ex: Força + Inteligência = guerreiro mágico)
- Cada skill tem identidade clara
- Balanceamento visando diversão + fairness

## Próximos Passos Recomendados

1. Testar todas as 9 skills no servidor com o menu de atributos.
2. Ajustar multiplicadores conforme o feedback de testes reais.
3. Criar skills de tier mais alto (nível 25~40).
4. Adicionar skills de utility / mobilidade / crowd control.
5. Integrar com o Sistema de Almas/Ecos.
6. Criar versões "Ultimate" das skills principais.
