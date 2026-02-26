# Entregável 2: EDA_1A_Pseudocódigo

## Atividade: Modelagem baseada no artigo "Uma Experiência com Agentes Inteligentes".

### a. Etapas Gerenciais de Construção (Seção 4.1 do Artigo):

- Este algoritmo descreve o fluxo de modelagem das regras do jogo de Truco conforme especificado no texto.

```Delphi
Algoritmo "Construcao_Software_Truco"
Inicio
   // 1. Definição do Objetivo e Pontuação (12 pontos) [cite: 170]
   Definir_Objetivo(12, "Melhor de Três");
   
   // 2. Modelagem da Distribuição e Manilha [cite: 172]
   Configurar_Mesa(3_cartas_por_jogador, definir_manilha);
   
   // 3. Atribuição de Valores Não-Lineares (Tabela 1) [cite: 178, 181]
   Mapear_Valor_Cartas(); // Ex: 4=1, 3=10, Manilha Paus=14
   
   // 4. Implementação da Lógica de Apostas (Truco/Retruco) [cite: 175, 176]
   Definir_Regras_Aposta(valor_inicial=1, incremento=3);
   
   // 5. Modelagem do Comportamento dos Agentes [cite: 187, 188]
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
   // FASE 1: Decisão de Truco (Figura 1) [cite: 259]
   Se (Nao equipe_pediu_truco) Entao
      Se (blefar) OU (valor_medio_cartas > 10) Entao
         Pedir_Truco()
      FimSe
   FimSe

   // FASE 2: Decisão de Jogar Carta (Figura 2) [cite: 313]
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

