# ranking-notas
### Objetivo do algoritmo: Realizar a classificação de uma lista notas com base em critérios diferentes.
**Problema:** João é professor e precisa organizar notas de seus alunos de diversas formas. Faça um algoritmo que o ajude a:
  - (A) Calcular a média da turma;
  - (B) Mostrar as notas maiores que a média da turma;
  - (C) Ordenar a lista de notas em ordem decrescente;
  - (C) Mostrar o aluno com a nota mais alta da turma e o aluno com a nota mais baixa, considerando que podem existir alunos com notas iguais!

### Objetivos do exercicio:
- Desenvolver a capacidade de analisar um problema, encontrar as suas especificidades e conseguir transformar todos esses pontos em um código com boas práticas.

### Entrada
- Número que irá representar a nota.
- Letra **p** para indicar que todas as notas ja foram inseridas.

### Saídas
- Média de turma
- Notas maiores que a média
- Lista de notas ordenada de forma decrescente
- Maior(es) e Menor(es) nota(s).

### Observações
**Obs1.:** O usuário deve poder inserir números decimais com vírgula ou com ponto. Ex: 8.7 e 8,7 devem representar o mesmo número: 8.7.

**Obs2.:** As notas devem ser inseridas uma de cada vez. Ou seja, não serão aceitas entradas com multiplas notas em um só input. Exemplo:
```sh
## Forma errada
Insira uma nota: 8.8 9 10

## Forma correta
Insira uma nota: 8.8
Insira uma nota: 9
Insira uma nota: 10
```

### Exemplos
#### Exemplo 1
##### Entrada
```sh
8
4
9
5
10
p
```
##### Saida
```sh
(A) 7.2
(B) [8.0, 9.0, 10.0]
(C) [10.0, 9.0, 8.0, 5.0, 4.0]
(D) 10.0, 4.0
```

#### Exemplo 2
##### Entrada
```sh
9.7
4,5
1,2
1qa2
1.2
7
p
```
##### Saida
```sh
(A) 4.72
(B) [9.7, 7.0]
(C) [9.7, 7.0, 4.5, 1.2, 1.2]
(D) 9.7, [1.2, 1.2]
```

#### Exemplo 3
##### Entrada
```sh
p
```
##### Saida
```sh
Nenhuma nota inserida.
```

#### Exemplo 4
##### Entrada
```sh
9.0
9,0
9
p
```
##### Saida
```sh
(A) 9.0
(B) Não há notas maiores que a media.
(C) [9.0, 9.0, 9.0]
(D) Todas as notas são iguais.
```

### Instruções gerais
- Escreva seu código dentro do arquivo **exercicio.py**
- Fique atento a formtação das saídas. Caso haja algum texto incorreto, o teste irá falhar.
- Os inputs do algoritmo não podem conter frases.
- Exemplo de como **não** usar os inputs na sua resposta:
```sh
numero = int(input("Insira seu numero"))
```

- Exemplo de como usar os inputs **corretamente** na sua resposta:
```sh
numero = int(input())
```
- Caso não haja numeros da lista de notas a saida deverá ser:
```sh
Nenhuma nota inserida.
```
- Em relação ao item (B), caso não haja notas maiores que a média, veja **exemplo 4**, a saida para o item (B) deve ser:
```sh
Não há notas maiores que a media.
```
- A saida do item (D) deverá ser no formato: "maior(res), menor(res)". Caso haja apenas uma nota no maior ou no menor, a saida deverá ser o número. Caso haja mais de um numero no maior ou menor, a saida deverá ser a lista com esses numeros, observe o **exemplo 2**. Caso não haja notas maiores ou menores, ou seja, todas as notas são iguais, a saida do item (D) deve ser:
```sh
Todas as notas são iguais.
```
- Todas as entradas inválidas devem ser igoradas e não encerrar o programa. Observe o **exemplo 2**. **Dica:** Use `try except`.
