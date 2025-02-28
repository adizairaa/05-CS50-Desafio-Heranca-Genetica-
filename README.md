# Gerador de Herança Genética de uma  Família e seus Tipos Sanguíneos 👨‍👩‍👧‍👦🧬

Este programa simula a criação de uma arvore genetica de  família de 3 gerações e gera aleatoriamente os tipos sanguíneos (alélos) de cada membro, passando de geração em geração.

## Descrição 📜

Este programa utiliza estruturas de dados em C para representar uma família com pais e filhos, onde cada pessoa tem dois alelos que determinam seu tipo sanguíneo. O código gera aleatoriamente os tipos sanguíneos de cada pessoa, baseados nos alelos dos pais.

## Funcionalidade 🔧

- **Geração de Família:** A função `create_family` cria uma árvore genealógica de até 3 gerações.
- **Impressão da Família:** A função `print_family` imprime a árvore genealógica gerada, exibindo o tipo sanguíneo de cada pessoa.
- **Liberação de Memória:** A função `free_family` é responsável por liberar a memória alocada durante a criação da árvore genealógica.

## Estrutura de Dados 🧩

A estrutura `person` contém:
- **parents[2]:** Um vetor de ponteiros que representa os pais da pessoa.
- **alleles[2]:** Um vetor de caracteres que representa os alelos da pessoa, que determinam seu tipo sanguíneo.

## Como Funciona 🔍

1. **Criação da Família:** A função `create_family` aloca memória para uma pessoa e, se a geração for maior que 1, cria dois pais para essa pessoa.
2. **Atribuição de Alelos:** Para cada pessoa, a função escolhe aleatoriamente um alelo de cada um de seus pais (ou gera alelos aleatórios para a primeira geração).
3. **Impressão da Família:** A árvore genealógica é impressa com identação para representar diferentes gerações.
4. **Liberação de Memória:** Após a impressão, a memória é liberada para evitar vazamentos de memória.

## Exemplo de Saída 📊

Geração 0, tipo sanguíneo AO
Geração 1, tipo sanguíneo OO
Geração 2, tipo sanguíneo AB
Geração 2, tipo sanguíneo O
Geração 1, tipo sanguíneo AB
Geração 2, tipo sanguíneo O
Geração 2, tipo sanguíneo AB

## Funções 🔨

- `create_family(int generations)` — Cria uma nova pessoa e seus pais, se necessário.
- `free_family(person *p)` — Libera a memória da pessoa e seus pais.
- `print_family(person *p, int generation)` — Imprime a árvore genealógica.
- `random_allele()` — Gera aleatoriamente um dos três tipos sanguíneos: A, B ou O.

## Compilação e Execução 🛠️

1. Compile o código com um compilador C, por exemplo:

    ```bash
    gcc -o gerador_familia gerador_familia.c
    ```

2. Execute o programa:

    ```bash
    ./gerador_familia
    ```

## Dependências 📦

- **Linguagem:** C (compilador GCC)
- **Bibliotecas:** `stdio.h`, `stdlib.h`, `time.h`, `stdbool.h`

## Contribuições 🤝

Sinta-se à vontade para fazer um fork deste repositório e enviar pull requests. Se encontrar algum erro ou tiver sugestões, fique à vontade para abrir uma issue.




