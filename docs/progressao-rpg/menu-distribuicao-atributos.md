# Menu de Distribuição de Atributos (DeluxeMenus)

## Visão Geral

Este menu permite que o jogador distribua livremente seus **pontos de atributo** entre os 5 stats principais, sem nenhuma trava de classe.

É a interface principal do sistema classless que queremos.

## Como funciona

- O menu é aberto com o comando **/atributos**
- Mostra os valores atuais de cada stat usando placeholders do AuraSkills
- Cada botão aumenta o stat em **+1** (consumindo 1 ponto de atributo)
- O menu atualiza automaticamente após cada clique (refresh)
- Requer que o jogador tenha pelo menos 1 ponto disponível para ver os botões de aumento

## Stats suportados

| Stat            | Material no Menu     | Efeito principal                     |
|-----------------|----------------------|--------------------------------------|
| Força          | Diamond Sword        | Dano melee + carga                   |
| Constituição   | Shield               | Vida + resistência física            |
| Destreza        | Bow                  | Crítico + ranged + esquiva          |
| Inteligência    | Enchanted Book       | Dano mágico + mana + skills         |
| Sabedoria       | Experience Bottle    | Resistência mágica + cura            |

## Instalação e Configuração

1. Instale os plugins:
   - **DeluxeMenus**
   - **PlaceholderAPI** (com expansões do AuraSkills)
   - **AuraSkills**

2. Coloque o arquivo `attribute-distribution.yml` em:
   `plugins/DeluxeMenus/menus/`

3. Dê reload no DeluxeMenus:
   `/deluxemenus reload`

4. (Opcional) Dê ao jogador permissão para usar o comando:
   `deluxemenus.menu.atributos`

## Comandos úteis

- `/atributos` — Abre o menu
- `/auraskills stats <jogador>` — Vê stats atuais
- `/auraskills addattribute <jogador> <stat> <quantidade>` — Adiciona manualmente (console)

## Dicas de balanceamento

- No início, os pontos vêm rápido (level 1~20)
- Depois o ganho diminui (conforme documentado em `ganho-de-pontos-e-level-up.md`)
- O menu incentiva o jogador a testar builds híridas

## Próximos passos possíveis

- Adicionar botão de "Reset de Stats" (com custo em almas ou dinheiro)
- Criar menus secundários por build (ex: "Build Tanque", "Build DPS")
- Integrar com o sistema de Almas/Ecos (morte perde pontos temporários)
