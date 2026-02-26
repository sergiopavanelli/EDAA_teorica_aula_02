# Entregável 1: EDA_1A_Lista

## Atividade: Lista de exercícios de lógica e pseudocódigo.

### 1.1 Inversão de Nomes

```delphi
Algoritmo "InverteNomes"
Var
   primeiroNome, ultimoNome: caractere
Inicio
   Escreva("Digite seu primeiro nome: ")
   Leia(primeiroNome)
   Escreva("Digite seu último nome: ")
   Leia(ultimoNome)
   Escreva(ultimoNome, ", ", primeiroNome)
FimAlgoritmo
```

### 1.2 Cálculo de Idade

```delphi
Algoritmo "CalculaIdade"
Var
   anoNascimento, anoAtual, idade: inteiro
Inicio
   anoAtual <- 2026 // Conforme data da atividade [cite: 53]
   Escreva("Digite o ano de nascimento: ")
   Leia(anoNascimento)
   idade <- anoAtual - anoNascimento
   Escreva("Sua idade é: ", idade)
FimAlgoritmo
```

### 1.3 Soma de Dois Números

```delphi
Algoritmo "SomaNumeros"
Var
   n1, n2, resultado: real
Inicio
   Escreva("Digite o primeiro número: ")
   Leia(n1)
   Escreva("Digite o segundo número: ")
   Leia(n2)
   resultado <- n1 + n2
   Escreva("O resultado da soma é: ", resultado)
FimAlgoritmo
```

### 1.4 Média Aritmética (5 Notas)

```delphi
Algoritmo "MediaCincoNotas"
Var
   n, soma, media: real
   i: inteiro
Inicio
   soma <- 0
   Para i de 1 ate 5 faca
      Escreva("Digite a nota ", i, ": ")
      Leia(n)
      soma <- soma + n
   FimPara
   media <- soma / 5
   Escreva("A média aritmética é: ", media)
FimAlgoritmo
```

### 1.5 Média de Disciplina (3 Notas)

```delphi
Algoritmo "MediaDisciplina"
Var
   n1, n2, n3, media: real
Inicio
   Escreva("Digite a primeira nota: ")
   Leia(n1)
   Escreva("Digite a segunda nota: ")
   Leia(n2)
   Escreva("Digite a terceira nota: ")
   Leia(n3)
   media <- (n1 + n2 + n3) / 3
   Escreva("A média obtida na disciplina é: ", media)
FimAlgoritmo
```

### 1.6 Cálculo de Salário por Hora

```delphi
Algoritmo "SalarioHora"
Var
   salarioTotal, horasPorDia, horasPorMes, valorHora: real
Inicio
   Escreva("Digite o salário total mensal: ")
   Leia(salarioTotal)
   Escreva("Digite as horas trabalhadas por dia: ")
   Leia(horasPorDia)
   // Considerando um mês comercial de 30 dias
   horasPorMes <- horasPorDia * 30
   valorHora <- salarioTotal / horasPorMes
   Escreva("O valor recebido por hora é: ", valorHora)
FimAlgoritmo
```


