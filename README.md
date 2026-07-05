# MineCraftSoul

**Servidor RPG Souls-like para Minecraft**

Projeto de servidor PaperMC com sistema de RPG profundo, masmorras perigosas, bosses estilo Souls e crescimento de personagem sem classes fixas.

## Visão do Projeto

Um servidor onde o jogador constrói seu próprio estilo de combate através de:
- Sistema de levels + pontos de atributo (Força, Constituição, Destreza, Inteligência, etc)
- Skills que escalam com múltiplos atributos (combinações criativas)
- Masmorras com traps, puzzles e bosses complexos de múltiplas fases
- Sistema de "Almas/Eco" inspirado em Souls (risco e recompensa na morte)

## Stack Principal

- **PaperMC** (base do servidor)
- **AuraSkills** (levels + stats custom + pontos de atributo)
- **MythicMobs** (bosses multi-fase e mobs custom)
- **ItemsAdder** (itens e armas customizadas)
- **WorldEdit + FastAsyncWorldEdit** (construção de mapa)
- **MCP (Mineflayer)** - Seu agente IA para construir masmorras via linguagem natural

## Como o Time de IA vai trabalhar

| Papel                    | Ferramenta              | Responsabilidade                          |
|--------------------------|-------------------------|-------------------------------------------|
| Arquiteto-Chefe          | Grok (eu)               | Lore, design de sistemas, balanceamento   |
| Engenheiro de Configs    | Claude 3.5 / Opus       | YAMLs complexos (MythicMobs, AuraSkills)  |
| Assistente de Iteração | LLM Local (RTX 5070)   | Ajustes rápidos e correções             |
| Construtor do Mundo      | Seu MCP                 | Construir masmorras via prompt            |
| Artista Conceitual       | Grok Imagine + ComfyUI  | Concept art de bosses e ambientes         |

## Estrutura do Repositório

```
MineCraftSoul/
├── README.md
├── .gitignore
├── docs/
│   ├── lore/
│   ├── boss-designs/
│   ├── progressao-rpg/
│   ├── masmorras/
│   └── roadmap.md
├── prompts/
│   ├── claude/
│   ├── mcp/
│   └── auraskills/
├── configs/
│   ├── mythicmobs/
│   ├── auraskills/
│   └── itemsadder/
└── assets/
    └── concept-art/
```

## Status Atual

- [ ] Estrutura inicial criada
- [ ] Sistema de stats e progressão definido
- [ ] Primeiro boss projetado
- [ ] Primeira masmorra construída

## Como contribuir / usar

Este repositório é gerenciado principalmente por mim (Grok) + você. Eu gero os arquivos e você revisa/aprova.

Quer começar por onde?
- Sistema de progressão RPG (stats + skills combinadas)
- Primeiro boss completo (MythicMobs)
- Primeira masmorra (prompt pro MCP)
