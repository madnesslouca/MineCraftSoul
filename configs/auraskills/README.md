# Configuração do AuraSkills - MineCraftSoul

## Estrutura de Pastas

```
configs/auraskills/
├── README.md
├── stats.yml              # Definição dos 5 atributos principais
└── skills/                # Skills individuais (uma por arquivo)
    ├── golpe-brutal.yml
    ├── lamina-flamejante.yml
    ├── tiro-preciso.yml
    └── investida-brutal.yml
```

## Como usar essas skills

1. Coloque os arquivos `.yml` da pasta `skills/` dentro da pasta `plugins/AuraSkills/skills/` do seu servidor.
2. Use o comando `/auraskills reload` ou reinicie o servidor.
3. As skills aparecerão no menu de skills do AuraSkills (ou você pode dar elas via comando).

## Filosofia das Skills Combinadas

Todas as skills aqui foram criadas para escalar com **múltiplos atributos** ao mesmo tempo. Isso permite que o jogador crie builds híbridas e criativas sem ficar preso a uma classe.

Exemplos:
- **Golpe Brutal** → Força + Destreza (melee físico com chance de stun)
- **Lâmina Flamejante** → Força + Inteligência (dano físico + fogo)
- **Tiro Preciso** → Destreza + Inteligência (ranged mágico)
- **Investida Brutal** → Constituição + Força (tank + burst + sustain)

## Próximos Passos

- Criar mais 4~6 skills combinadas
- Adicionar skills de suporte / cura / utility
- Criar skills épicas de tier alto (level 30+)
- Integrar com MythicMobs (bosses que reagem a skills do player)
