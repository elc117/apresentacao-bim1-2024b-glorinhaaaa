# Prova Paradigmas - Questão 2

## Função: `funq2`

```haskell
funq2 :: [Int] -> [Int]
funq2 ns = map (\n -> if even n then n + 1 else 0) ns
```

### Tipo da Função
A função `funq2` recebe uma lista de inteiros do tipo `[Int]` e retorna uma nova lista também do tipo `[Int]`.

### Corpo da Função
A expressão `funq2 ns = map (\n -> if even n then n + 1 else 0) ns` realiza a seguinte operação:

- **`map`**: É uma função que aplica uma transformação a cada elemento de uma lista, retornando uma nova lista.

### Função Anônima
A função anônima **`\n -> if even n then n + 1 else 0`** realiza as seguintes etapas:

1. **Parâmetro**:
   - `n`: Representa cada elemento da lista `ns` durante a iteração.

2. **Condição**:
   - A condição `if even n` verifica se `n` é um número **par**.
     - Se **verdadeiro**:
       - Retorna `n + 1`: Incrementa o número par em 1.
     - Se **falso**:
       - Retorna `0`: Substitui o número ímpar por 0.

### Resumo do Comportamento
A função `funq2` processa uma lista de inteiros e gera uma nova lista com as seguintes características:

- Os números **pares** são incrementados em **1**.
- Os números **ímpares** são substituídos por **0**.

### Exemplos de Uso

- **Entrada**: `funq2 [2, 5, 8, 13]`
  - **Saída**: `[3, 0, 9, 0]`
  - **Explicação**:
    - `2` é par → `2 + 1 = 3`
    - `5` é ímpar → `0`
    - `8` é par → `8 + 1 = 9`
    - `13` é ímpar → `0`

- **Entrada**: `funq2 [1, 2, 3, 4]`
  - **Saída**: `[0, 3, 0, 5]`
  - **Explicação**:
    - `1` é ímpar → `0`
    - `2` é par → `2 + 1 = 3`
    - `3` é ímpar → `0`
    - `4` é par → `4 + 1 = 5`

## Conclusão
A função `funq2` é útil para transformar listas de inteiros, facilitando a manipulação de dados numéricos com base em condições simples.
