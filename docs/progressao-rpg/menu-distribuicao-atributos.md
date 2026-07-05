# Menu de Distribuição de Atributos (Melhorado - A4.2)

## Visão Geral

Menu visualmente rico e funcional criado com **DeluxeMenus** para o sistema de progressão classless do MineCraftSoul.

**Comando para abrir:** `/atributos`

## Melhorias Implementadas (A4.2)

### 1. Visual e UX
- Título dinâmico com nome do jogador
- Design mais limpo e organizado (54 slots)
- Cores distintas para cada atributo
- Lore muito mais detalhado e explicativo
- Som de "level up" ao gastar ponto

### 2. Informações Extras
- Cabeçalho mostra Nível + Pontos disponíveis
- Seção de **Resumo dos Bônus** no lado direito
- Cada botão mostra exatamente o que o stat aumenta

### 3. Experiência mais imersiva
- Sons ao clicar
- Feedback visual imediato (menu reabre atualizado)
- Dicas de builds híbridas

## Como Instalar

1. Instale os plugins:
   - DeluxeMenus
   - PlaceholderAPI (com expansão do AuraSkills)
   - AuraSkills

2. Copie o arquivo:
   ```
   plugins/DeluxeMenus/menus/attribute-distribution.yml
   ```

3. Recarregue:
   ```
   /deluxemenus reload
   ```

4. Abra com:
   ```
   /atributos
   ```

## Observações Importantes

- Os placeholders `%auraskills_strength%`, `%auraskills_constitution%` etc. dependem da configuração do AuraSkills + PlaceholderAPI.
- Se algum placeholder não funcionar, verifique se a expansão do AuraSkills está instalada no PlaceholderAPI.
- O comando `auraskills addattribute` precisa estar disponível e com permissões corretas.

## Próximos Passos Sugeridos

- Adicionar botão de **Reset de Stats** (com custo em Almas)
- Criar versão ainda mais avançada com efeitos de partículas
- Integrar com o sistema de Almas/Ecos

---

**Status:** Implementado e melhorado (A4.2)