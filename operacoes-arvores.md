# Operações em Árvores

---

# Rotação Simples à Direita

## Conceito

É uma operação utilizada em árvores binárias de busca balanceadas (como as árvores AVL) para corrigir um desequilíbrio causado pelo crescimento excessivo do lado esquerdo da árvore. A rotação reorganiza os nós sem alterar a ordem dos elementos.

## Situação em que é utilizada

Acontece no caso **Esquerda-Esquerda (LL)**:

- Um novo nó é inserido na subárvore esquerda;
- Esse nó fica na subárvore esquerda do filho esquerdo;
- O fator de balanceamento torna-se maior que **+1**.

## Exemplo

### Antes da rotação

```text
      C
     /
    B
   /
  A
```

### Depois da rotação

```text
      B
     / \
    A   C
```

---

# Rotação Simples à Esquerda

## Conceito

É utilizada para corrigir desequilíbrios causados pelo crescimento excessivo do lado direito da árvore.

## Situação em que é utilizada

Acontece no caso **Direita-Direita (RR)**:

- Um novo nó é inserido na subárvore direita;
- Esse nó fica na subárvore direita do filho direito;
- O fator de balanceamento torna-se menor que **-1**.

## Exemplo

### Antes da rotação

```text
  A
   \
    B
     \
      C
```

### Depois da rotação

```text
      B
     / \
    A   C
```

---

# Rotação Dupla Esquerda-Direita (LR)

## Conceito

É utilizada para corrigir um desequilíbrio em que o crescimento ocorre na subárvore direita do filho esquerdo do nó desbalanceado.

Essa operação realiza duas rotações:

1. Rotação simples à esquerda no filho esquerdo;
2. Rotação simples à direita no nó desbalanceado.

## Situação em que é utilizada

Quando:

- O nó está desbalanceado para a esquerda;
- O novo elemento foi inserido na subárvore direita do filho esquerdo.

## Exemplo

### Antes da rotação

```text
      C
     /
    A
     \
      B
```

### Depois da rotação

```text
      B
     / \
    A   C
```

---

# Rotação Dupla Direita-Esquerda (RL)

## Conceito

É utilizada para corrigir um desequilíbrio em que o crescimento ocorre na subárvore esquerda do filho direito do nó desbalanceado.

Essa operação realiza duas rotações:

1. Rotação simples à direita no filho direito;
2. Rotação simples à esquerda no nó desbalanceado.

## Situação em que é utilizada

Quando:

- O nó está desbalanceado para a direita;
- O novo elemento foi inserido na subárvore esquerda do filho direito.

## Exemplo

### Antes da rotação

```text
    A
     \
      C
     /
    B
```

### Depois da rotação

```text
      B
     / \
    A   C
```

---

# Inversão (Espelhamento)

## Conceito

A inversão (ou espelhamento) consiste em trocar os filhos esquerdo e direito de todos os nós da árvore. Dessa forma, a subárvore esquerda passa a ocupar a posição da subárvore direita e vice-versa.

## Aplicações

Pode ser utilizada para:

- Verificação de simetria entre árvores;
- Processamento de estruturas hierárquicas;
- Manipulação de estruturas de dados em sistemas computacionais;
- Estudos e testes de algoritmos em árvores binárias.

## Exemplo

### Antes da inversão

```text
          10
         /  \
        5    15
       / \   / \
      3   7 12 18
```

### Depois da inversão

```text
          10
         /  \
       15    5
      / \   / \
     18 12 7   3
```