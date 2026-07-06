# Sistema de Archetypes - MineCraftSoul

## Introdução

O sistema de **Archetypes** (Origens) foi criado para dar **identidade** aos personagens sem perder a liberdade do sistema classless.

Cada jogador escolhe **um Archetype** que representa a origem da sua alma dentro do universo do **Véu Rasgado**.  
O Archetype **não trava** stats nem skills — ele apenas oferece bônus passivos e uma mecânica especial temática.

---

## Filosofia do Sistema

- **Liberdade de Build**: O jogador continua distribuindo pontos de atributo livremente nos 5 stats (Força, Constituição, Destreza, Inteligência e Sabedoria).
- **Identidade**: Cada Archetype oferece uma personalidade e um estilo de jogo diferente.
- **Expansível**: Novos Archetypes podem ser adicionados facilmente no futuro.
- **Integração**: O sistema funciona em conjunto com o sistema de Almas, Skills e Itens customizados.

---

## Archetypes Disponíveis

### 1. Nascido do Véu (Veilborn)

**Lore:**  
Ser que nasceu diretamente da corrupção do Véu. Sua existência está profundamente ligada à escuridão que consome o mundo.

**Bônus Passivo:**  
- **+12%** de dano contra mobs e bosses marcados como "Corrompidos".

**Efeito Especial:**  
- Ao matar um mob corrompido, tem **25% de chance** de ganhar **+1 Alma** extra.

**Estilo Recomendado:**  
Builds ofensivas focadas em farming de Almas e dano contra o conteúdo principal do servidor.

---

### 2. Alma Cicatrizada (Soulscarred)

**Lore:**  
Almas que foram profundamente marcadas pela corrupção e aprenderam a transformar sua dor em força.

**Bônus Passivo:**  
- **+8%** de dano recebido (aumenta o risco).

**Efeito Especial:**  
- Quando a vida está **abaixo de 40%**, ganha **+18%** de dano total.

**Estilo Recomendado:**  
Jogadores que gostam de jogar de forma agressiva e arriscada (estilo hardcore).

---

### 3. Nascido do Eclipse (Eclipseborn)

**Lore:**  
Nascidos no exato momento em que o grande Eclipse rasgou o Véu. Possuem forte afinidade com poderes ocultos e instáveis.

**Bônus Passivo:**  
- **+10%** de Inteligência.

**Efeito Especial:**  
- Skills que causam dano mágico têm **+10%** de chance de acerto crítico.

**Estilo Recomendado:**  
Builds híbridas ou mágicas que utilizam Inteligência como atributo principal.

---

### 4. Guardião Oco (Hollow Warden)

**Lore:**  
Antigos guardiões enviados para selar o Véu que tiveram parte de sua alma consumida pela corrupção. Agora vagueiam como cascas vazias.

**Bônus Passivo:**  
- **+15%** de vida máxima.

**Efeito Especial:**  
- Ao cair **abaixo de 30%** de vida, ganha automaticamente um **escudo equivalente a 25% da vida máxima** (Cooldown: 90 segundos).

**Estilo Recomendado:**  
Builds tanque e de sobrevivência.

---

### 5. Andarilho da Fenda (Riftwalker)

**Lore:**  
Indivíduos que aprenderam a navegar pelas fendas instáveis do Véu. Conseguem se mover entre realidades por breves momentos.

**Bônus Passivo:**  
- **+12%** de velocidade de movimento.

**Efeito Especial:**  
- Após matar um inimigo, fica **invisível por 4 segundos** (Cooldown: 50 segundos).

**Estilo Recomendado:**  
Builds de mobilidade, assassino ou exploração.

---

### 6. Atado às Cinzas (Ashenbound)

**Lore:**  
Almas que se ligaram aos restos dos que foram consumidos pelo Véu. Acreditam que honrar os caídos é a única forma de encontrar sentido no mundo destruído.

**Bônus Passivo:**  
- **+10%** de Sabedoria.

**Efeito Especial:**  
- Ao recuperar um **Eco da Alma**, recebe **+30% mais Almas** do que o normal.

**Estilo Recomendado:**  
Jogadores que querem focar no sistema de Almas e em mecânicas de suporte/colecionador.

---

## Como Escolher o Archetype

### Primeira Vez
- Ao fazer login pela primeira vez, o menu de Archetypes abrirá automaticamente.
- Escolha um dos 6 Archetypes disponíveis.

### Depois da Primeira Escolha
- Use o comando:
  ```
  /archetypes
  ```

---

## Implementação

| Componente | Arquivo |
|---|---|
| Script Skript | `configs/skript/scripts/archetypes.sk` |
| Documentação | `docs/archetypes/archetypes.md` |

> **Nota:** O Archetype **Atado às Cinzas** está documentado mas ainda não implementado no script — será adicionado na próxima versão do `archetypes.sk`.
