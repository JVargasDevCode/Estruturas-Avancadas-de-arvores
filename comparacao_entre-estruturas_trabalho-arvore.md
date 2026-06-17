# Comparação entre Estruturas de Árvores

| Estrutura | Nº Máximo de Filhos | Balanceamento | Complexidade de Busca | Complexidade de Inserção | Vantagem Principal | Desvantagem Principal | Exemplo de Aplicação |
|-----------|---------------------|---------------|----------------------|--------------------------|-------------------|----------------------|---------------------|
| BST (Árvore Binária de Busca) | 2 | Não possui balanceamento automático. Pode ficar desbalanceada conforme a ordem de inserção. | O(log n) no melhor caso e O(n) no pior caso | O(log n) no melhor caso e O(n) no pior caso | Estrutura simples de entender e implementar | Pode perder desempenho se ficar desbalanceada | Árvores de busca básicas |
| AVL | 2 | Sim. Mantém o fator de balanceamento com rotações. | O(log n) | O(log n) | Busca previsível e eficiente | Inserção e remoção mais custosas por causa das rotações | Índices e estruturas que exigem leitura frequente |
| Rubro-Negra | 2 | Sim. Usa coloração e rotações para manter o balanceamento aproximado. | O(log n) | O(log n) | Balanceamento eficiente com menos rotações que a AVL | Implementação mais complexa | Bibliotecas e estruturas internas de sistemas |
| N-ária | N (vários filhos) | Pode ou não possuir mecanismos de balanceamento, dependendo da variação. | O(log n) em estruturas balanceadas, mas depende da aplicação | O(log n) ou proporcional à estrutura da árvore | Representa melhor hierarquias com muitos filhos | Não é tão simples quanto a árvore binária em alguns contextos | Sistema de arquivos, menus e taxonomias |
