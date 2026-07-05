# Prompt Otimizado para MCP - Catacumbas do Véu Rasgado

**Instruções importantes antes de colar no agente:**

1. Use este prompt **exatamente** como está (ou com míimas alterações)
2. Certifique-se que o agente MCP tem permissão de WorldEdit no mundo
3. Recomenda-se rodar em um mundo limpo ou em uma área isolada primeiro
4. Depois da construção automática, faça refinamentos manuais com WorldEdit

---

## PROMPT PARA COLAR NO SEU AGENTE MCP (Mineflayer)

```
Crie uma masmorra dark fantasy gótica chamada "Catacumbas do Véu Rasgado" no subsolo de uma área de ruínas na superfície.

**Localização da entrada:**
Crie ruínas de uma pequena capela gótica destruída na superfície (coordenadas aproximadas X: 150, Z: 80). Use blocos de deepslate, cracked deepslate bricks, blackstone, chains e soul fire para dar um visual sombrio e abandonado. Coloque estátuas de anjos quebradas e algumas correntes penduradas. A entrada principal deve ter uma alavanca grande que abre uma escada descendente para o subsolo.

**Estrutura geral da masmorra (3 andares subterrâneos):**

**Andar 1 - Corredores da Queda** (profundidade ~ -20 a -35):
- Corredores estreitos (3 blocos de largura) com várias curvas e salas laterais pequenas.
- Coloque armadilhas de pressão no chão que disparam flechas envenenadas (use dispensers escondidos).
- Em alguns pontos, pisos falsos que caem quando pisados (use redstone + pistons ou falling blocks).
- Iluminação muito baixa: use apenas soul lanterns e algumas soul fire.
- Spawners naturais ou via MythicMobs de esqueletos corrompidos (fracos).
- 2-3 salas laterais com baús de loot básico (itens de tier 1).

**Andar 2 - Salões dos Ecos** (profundidade ~ -40 a -55):
- Salas maiores (8x8 ou 10x10) conectadas por corredores.
- **Puzzle principal de alavancas:** 4 alavancas grandes em salas diferentes. Cada alavanca controla:
  - Fluxo de lava em canais
  - Portas de ferro
  - Ou soul fire que ilumina/desativa armadilhas
- O puzzle deve exigir que o jogador acione as alavancas na ordem correta ou todas de uma vez para abrir o caminho para o andar 3.
- Mobs mais fortes: Zumbis com armadura enferrujada e alguns Phantoms voando.
- Armadilhas de queda + blocos de soul sand que reduzem velocidade.
- Uma sala secreta bem escondida com um baú melhor (requer resolver parte do puzzle).

**Andar 3 - Arena do Guardião Corrompido** (profundidade ~ -60):
- Uma arena circular grande (mínimo 25x25 blocos de diâmetro interno).
- 6 pilares grossos de blackstone posicionados de forma simétrica (podem ser destruídos pelo jogador ou pelo boss).
- No centro da arena, um buraco circular que começa seco, mas que jorrará lava na Fase 2 do boss.
- Paredes da arena com chains penduradas e soul fire.
- Iluminação dramática e opressora.
- Espaço vertical suficiente (pelo menos 12-15 blocos de altura) para o boss pular e para mecânicas de altura.
- Saída após o boss (teleport ou portal simples para fora da masmorra).

**Regras gerais de construção:**
- Tema visual consistente: deepslate + blackstone + cracked deepslate bricks + chains + soul sand/fire + iron bars.
- Transições entre andares devem ser naturais (escadas estreitas, buracos no chão ou elevadores de redstone simples).
- A masmorra deve parecer antiga, corrupta e perigosa.
- Evite iluminação excessiva.
- Use WorldEdit para preencher áreas grandes de forma eficiente.
- Depois de construir a estrutura, me avise para que eu possa adicionar os mobs, armadilhas e o boss via MythicMobs.

Construa tudo isso de forma limpa e funcional. Me avise quando terminar.
```

---

## Dicas de uso com seu MCP

- Cole o prompt acima exatamente como está
- Se o agente pedir mais detalhes, você pode adicionar:
  - "Use apenas blocos disponíveis no vanilla + deepslate"
  - "Não use comandos que exijam plugins além de WorldEdit"
- Após a construção, use `/rg define` (se usar WorldGuard) para proteger a masmorra
- Depois disso, vamos configurar os mobs e armadilhas com MythicMobs

## Próximos passos após a construção

1. Testar a navegação da masmorra
2. Adicionar armadilhas funcionais
3. Configurar mobs com MythicMobs
4. Implementar o primeiro boss na arena (próximo passo do projeto)