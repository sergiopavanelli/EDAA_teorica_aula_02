# UC: Estrutura de Dados e Análise de Algoritmos

## Título: Prática nº 01A – Artigo e Pseudocódigo –  EDA_1A_Pseudocódigo
## Data: 26/02/2026

## Integrantes:

- Sérgio Pinton Pavanelli - RA 123220202  
- Samuel Zappala Batista - RA 12411504  
- Elizabeth Stéphany Guimarães Miranda - RA 123220604  
- Gabriel Victor Dornelas Ferreira Sathler - 12319216  
- Ana Luiza Mattos de Carvalho - RA 124114111  
- Júlia Starling Negrini Fudoli - RA 124222027  
- Ana Clara Domingos Dias Silva - RA 12316965  
- Miguel Pedro Pinheiro - RA 12315515  
- Geovana Dias de Almeida - RA 123221311  

### Tema:   Programação de Soluções Computacionais 
### Objetivo:  Introdução aos principais conceitos e motivação 
### Roteiro: Formar grupos e desenvolver as atividades propostas. 

---

## Atividade: Modelagem baseada no artigo "Uma Experiência com Agentes Inteligentes".

### a. Etapas Gerenciais de Construção (Seção 4.1 do Artigo):

- Este algoritmo descreve o fluxo de modelagem das regras do jogo de Truco conforme especificado no texto.

```Delphi
Algoritmo "Construcao_Software_Truco"
Inicio
   // 1. Definição do Objetivo e Pontuação (12 pontos) 
   Definir_Objetivo(12, "Melhor de Três");
   
   // 2. Modelagem da Distribuição e Manilha 
   Configurar_Mesa(3_cartas_por_jogador, definir_manilha);
   
   // 3. Atribuição de Valores Não-Lineares (Tabela 1) 
   Mapear_Valor_Cartas(); // Ex: 4=1, 3=10, Manilha Paus=14
   
   // 4. Implementação da Lógica de Apostas (Truco/Retruco) 
   Definir_Regras_Aposta(valor_inicial=1, incremento=3);
   
   // 5. Modelagem do Comportamento dos Agentes 
   Criar_Agente_Juiz(); 
   Criar_Agentes_Jogadores(4);
FimAlgoritmo
```

### b. Simulação de "UMA RODADA" (Um Jogador, Uma Jogada):

- Baseado na rede semântica de decisão do artigo (Figuras 1 e 2).

```Delphi
Algoritmo "Simulacao_Jogada_Truco"
Var
   equipe_pediu_truco, primeira_rodada, possui_carta_maior: logico
   valor_medio_cartas: inteiro
Inicio
   // FASE 1: Decisão de Truco (Figura 1) 
   Se (Nao equipe_pediu_truco) Entao
      Se (blefar) OU (valor_medio_cartas > 10) Entao
         Pedir_Truco()
      FimSe
   FimSe

   // FASE 2: Decisão de Jogar Carta (Figura 2) 
   Se (primeira_rodada) Entao
      Se (primeiro_a_jogar) Entao
         Jogar_Carta_Roleta() // Escolha aleatória inicial
      Senao
         Se (possui_carta_maior_que_mesa) Entao
            Jogar_Maior_Carta()
         Senao
            Jogar_Menor_Carta()
         FimSe
      FimSe
   FimSe
FimAlgoritmo
```