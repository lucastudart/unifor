# UNIFOR
**Nome**:Lucas
**Disciplina**:Raciocínio lógico algorítmico
## Exercício 3
### Fluxograma
```mermaid
flowchart TD
A([INICIO])--> B{{Digite um número>:}}
B --> C[\numero\]
C --> D{numero > 0}
D --NÃO--> E[0 número não é positivo!]
D --SIM --> F[rest = numero % 2]
E --> Z([FIM])
F --> G{resto == 0}
G --NÃO--> H{{O número é impar!}}
G --SIM--> I{{O número é par!}}
H --> Z
I --> Z
```
### Pseudocódigo
````
1 ALGORITIMO verifica_par_impar
2 DECLARE numero, resto NUMERICO
3 ESCREVA "Digite um número: "
4 LEIA numero 
5 SE numero > 0 ENTAO 
6       resto = numero % 2 
7       SE resto == 0 ENTAO
8              ESCREVA "O número é par!'
9       SENAO
10                 ESCREVA " O número é impar!"
11  SENAO
12       ESCREVA "O número não é positivo!"
13   FIM_ALGORITIMO

#### Teste de mesa 
| numero | numero >= 0 | resto | resto == 0 | Saída |
| -- | -- | -- | -- | -- | 
| -1 | F |   |   | "O número deve ser postivo!" |
| 0  | V | 0 | V | "O número é par!" |
| 13 | V | 1 | F | "O número é impar!" |
| 30 | V | 0 | V | "O número é par!" |

###exercicio 3
``` mermaid
flowchart TD;
    Inicio --> ReceberNota1;
    ReceberNota1 --> ReceberNota2;
    ReceberNota2 --> CalcularMedia;
    CalcularMedia -->|Se média >= 6| Aprovado;
    CalcularMedia -->|Se média < 6| Reprovado;
    Aprovado --> MostrarAprovado;
    Reprovado --> MostrarReprovado;
    MostrarAprovado --> Fim;
    MostrarReprovado --> Fim;
 ```
Algoritmo CalcularMediaEStatus
    // Solicita e lê as duas notas do aluno
    Escrever "Digite a primeira nota do aluno:"
    Ler nota1
    Escrever "Digite a segunda nota do aluno:"
    Ler nota2
    
    // Calcula a média aritmética das notas
    media <- (nota1 + nota2) / 2
    
    // Verifica se a média é maior ou igual a 6
    Se media >= 6 Então
        Escrever "O aluno está aprovado com média:", media
    Senão
        Escrever "O aluno está reprovado com média:", media
    Fim Se
Fim Algoritmo


| número | número >= 0 | resto | resto == 0 | Saída |
| ------ | ----------- | ----- | ---------- | ------|
| -1     | F           |       |            | "O número deve ser positivo!" |
| 0      | V           | 0     | V          | "O número é par!" |
| 13     | V           | 1     | F          | "O número é ímpar!" |
| 30     | V           | 0     | V          | "O número é par!" |

###Exercicio 4





