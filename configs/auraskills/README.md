# Configuração do AuraSkills

Este diretório contém as configurações do **AuraSkills** para o sistema de progressão RPG classless do MineCraftSoul.

## Arquivos

- `stats.yml` — Definição dos 5 stats principais (Força, Constituição, Destreza, Inteligência, Sabedoria)
- `skills/` — Skills que escalam com combinações de atributos

## Como o sistema funciona

- Jogador sobe de nível normalmente
- A cada level up recebe **pontos de atributo** (distribuição livre)
- Não existe trava de classe
- Skills podem escalar com 2 ou mais stats ao mesmo tempo

## Menu de Distribuição de Pontos

O menu principal para o jogador distribuir pontos está em:

**`configs/deluxemenus/attribute-distribution.yml`**

- Comando para abrir: **`/atributos`**
- Usa DeluxeMenus + PlaceholderAPI
- Atualiza automaticamente após cada aumento

## Placeholders importantes (PlaceholderAPI)

- `%auraskills_strength%`
- `%auraskills_constitution%`
- `%auraskills_dexterity%`
- `%auraskills_intelligence%`
- `%auraskills_wisdom%`
- `%auraskills_attribute_points%`
- `%player_level%`

## Próximos passos

- Testar as skills combinadas no servidor
- Ajustar multiplicadores de dano
- Criar mais skills (suporte, área, ultimate)
- Integrar com o primeiro boss (MythicMobs)
