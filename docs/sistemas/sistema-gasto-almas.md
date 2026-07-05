# Sistema de Gasto de Almas (Atualizado - Opção K)

## Visão Geral

Almas agora podem ser gastas de duas formas principais:

1. **Reset de Atributos** (100 Almas) - via menu `/atributos`
2. **Forja de Itens de Alto Tier** - crafting de armas e armaduras lendárias

---

## Forja das Almas (Novo)

Você pode forjar **itens de alto poder** usando **Fragmentos do Véu Rasgado** + **Almas**.

### Como Funciona

1. Colete **Fragmentos do Véu Rasgado** (drop do Guardião Corrompido e futuros bosses).
2. Tenha **Almas suficientes** (ganhas ao subir de nível + recuperando Ecos).
3. Use a **mesa de crafting normal** para combinar os fragmentos.
4. O script da Forja das Almas automaticamente verifica e consome as Almas necessárias.

Se você não tiver Almas suficientes, o craft é cancelado com uma mensagem clara.

---

## Itens Disponíveis para Forja

| Item                        | Custo em Almas | Fragmentos Necessários | Requisitos de Atributo          | Estilo de Build          |
|-----------------------------|----------------|---------------------------|---------------------------------|--------------------------|
| Espada do Véu Rasgado     | 450            | 5x                        | Força 18 + Inteligência 14   | Híbrido Melee/Mágico   |
| Peitoral do Eco Eterno      | 600            | 8x                        | Constituição 20 + Sabedoria 12 | Tank com Sustain         |
| Talismã da Alma Livre      | 350            | 3x                        | Inteligência 16 + Destreza 14 | Mágico / Crítico       |

---

## Como Instalar

1. Coloque `high-tier-items.yml` em `plugins/ItemsAdder/contents/minecraf tsoul/`
2. Coloque `forja-almas.sk` em `plugins/Skript/scripts/`
3. Recarregue:
   ```
   /ia reload
   /sk reload
   ```
4. Teste craftando os itens na mesa de crafting normal.

---

## Futuro (Expansão)

- Criar uma **Forja das Almas** como bloco customizado (clique direito abre GUI bonita)
- Adicionar mais itens de tier superior
- Adicionar bônus de set (2/4/6 peças)
- Permitir "melhorar" itens existentes gastando Almas

---

*Sistema criado em julho 2026 como parte do projeto MineCraftSoul.*