# Ganho de Pontos e Level Up

## Filosofia do Sistema

Queremos um sistema que recompense tanto **exploração** quanto **combate**, mas que não force o jogador a grindar de forma chata. O level up deve ser significativo e dar sensação real de progresso.

## Fontes de Experiência (XP)

O jogador ganha XP de várias formas:

- **Combate** contra mobs e bosses (maior fonte)
- **Exploração** de masmorras e biomas perigosos
- **Mineração** e coleta de recursos raros
- **Quests** e eventos narrativos
- **Construção** e conquistas (em menor escala)

## Fórmula de Ganho de Pontos por Level Up

A cada level up o jogador recebe automaticamente:

### Pontos de Atributo

| Faixa de Nível | Pontos de Atributo | Pontos de Skill | Observação                     |
|-------------------|--------------------|-----------------|----------------------------------|
| 1 – 10           | **5**              | 2               | Fase inicial (crescimento rápido) |
| 11 – 25          | **4**              | 2               | Fase intermediária                |
| 26 – 40          | **3**              | 1               | Fase avançada                     |
| 41 – 60          | **2**              | 1               | Fase late-game                     |

> Total aproximado de pontos de atributo até o level 60: **~180 pontos**

### Distribuição Livre

O jogador pode distribuir os pontos **como quiser** nos 5 atributos. Não existe classe que limite onde pode colocar pontos.

Exemplo de builds possíveis:
- **Tanque Clássico**: Alto CON + FOR
- **DPS Ranged**: Alto DEX + INT
- **Battle Mage**: FOR + INT
- **Support Híbrido**: WIS + CON + INT
- **Glass Cannon**: Alto INT + baixo CON (arriscado)

## Implementação Técnica (AuraSkills)

No AuraSkills vamos configurar:

- `level-up` rewards com comandos ou skills que dão os pontos
- Um menu (DeluxeMenus) onde o jogador gasta os pontos manualmente
- Stats customizados com fórmulas de scaling

---

## Sistema de "Almas / Ecos" (Morte com Risco)

Inspirado em Souls-like:

- Quando o jogador morre, ele dropa uma parte das almas/eco no local da morte
- Ele pode voltar e recuperar
- Se morrer novamente antes de recuperar, perde uma porcentagem permanente

Isso adiciona tensão nas masmorras e bosses.

**Status**: Planejado para implementação após o sistema básico de stats