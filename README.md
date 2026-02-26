# 📚 EDAA — Estrutura de Dados e Análise de Algoritmos
## 🏫 UniBH 2026/1
### Aula 02 — Lógica e Pseudocódigo

## Integrantes:

- Sérgio Pinton Pavanelli - RA 123220202  
- Samuel Zappala Batista - RA 12411504  
- Gabriel Victor Dornelas Ferreira Sathler - 12319216  
- Elizabeth Stéphany Guimarães Miranda - RA 123220604  

---

## 📋 Sobre este repositório

Este repositório reúne os entregáveis da **Aula 02** da disciplina de Estrutura de Dados e Algoritmos Avançados. As atividades abordam fundamentos de lógica de programação e construção de pseudocódigo utilizando a linguagem **Portugol/VisuAlg (sintaxe Delphi)**.

---

## 📂 Atividades

| # | Arquivo | Descrição |
|---|---------|-----------|
| 1️⃣ | [EDA_1A_Lista.md](EDA_1A_Lista.md) | Lista de exercícios de lógica e pseudocódigo |
| 2️⃣ | [EDA_1A_Pseudocódigo.md](EDA_1A_Pseudocódigo.md) | Modelagem baseada em artigo científico sobre Agentes Inteligentes |

---

## 🧮 Entregável 1 — Lista de Exercícios

> Conjunto de algoritmos em pseudocódigo cobrindo operações essenciais de entrada, processamento e saída.

| Exercício | Tema | Conceitos |
|-----------|------|-----------|
| 1.1 | 🔤 Inversão de Nomes | Variáveis do tipo `caractere`, leitura e escrita |
| 1.2 | 🎂 Cálculo de Idade | Variáveis `inteiro`, operações aritméticas simples |
| 1.3 | ➕ Soma de Dois Números | Variáveis `real`, entrada de dados |
| 1.4 | 📊 Média Aritmética (5 notas) | Estrutura de repetição `Para...FimPara`, acumulador |
| 1.5 | 📝 Média de Disciplina (3 notas) | Operações com múltiplas variáveis `real` |
| 1.6 | 💰 Cálculo de Salário por Hora | Lógica de negócio, divisão e cálculo proporcional |

### 🔑 Conceitos abordados

- 📥 Entrada e saída de dados (`Leia` / `Escreva`)
- 🔢 Tipos de dados: `inteiro`, `real`, `caractere`
- 🔁 Estrutura de repetição (`Para...FimPara`)
- ➗ Operações aritméticas fundamentais
- 📦 Declaração e uso de variáveis

---

## 🤖 Entregável 2 — Pseudocódigo com Agentes Inteligentes

> Modelagem algorítmica baseada no artigo **"Uma Experiência com Agentes Inteligentes"**, aplicada ao domínio do jogo de **Truco**.

### 🏗️ Parte A — Etapas Gerenciais de Construção (Seção 4.1 do Artigo)

Descreve o fluxo de modelagem das regras do jogo de Truco:

| Etapa | Descrição |
|-------|-----------|
| 1 | 🎯 Definição do objetivo e pontuação (12 pontos, melhor de três) |
| 2 | 🃏 Configuração da mesa: distribuição e definição de manilha |
| 3 | 📈 Mapeamento de valores não-lineares das cartas (Tabela 1 do artigo) |
| 4 | 💬 Lógica de apostas: Truco / Retruco com incrementos definidos |
| 5 | 🤖 Criação dos agentes: Juiz e quatro Jogadores autônomos |

### ♟️ Parte B — Simulação de Uma Rodada

Modelagem da tomada de decisão de um jogador em uma jogada, baseada nas redes semânticas das Figuras 1 e 2 do artigo:

| Fase | Decisão | Lógica |
|------|---------|--------|
| 1 | 📣 Pedir Truco | Se não pediu ainda E (blefa OU valor médio > 10) |
| 2 | 🃏 Escolher carta (1ª rodada, 1º a jogar) | Jogada aleatória (roleta) |
| 2 | 🃏 Escolher carta (1ª rodada, não 1º) | Se tem carta maior → joga maior; senão → joga menor |

### 🔑 Conceitos abordados

- 🧠 Modelagem de comportamento de agentes inteligentes
- ⚖️ Estruturas condicionais aninhadas (`Se...Senao...FimSe`)
- 🔣 Variáveis do tipo `lógico` e `inteiro`
- 🕹️ Tomada de decisão baseada em regras (rule-based)
- 🌐 Aplicação de rede semântica em pseudocódigo

---

## 🛠️ Tecnologias e Ferramentas

![Portugol](https://img.shields.io/badge/Linguagem-Portugol%2FVisuAlg-blue?style=flat-square)
![Markdown](https://img.shields.io/badge/Documentação-Markdown-lightgrey?style=flat-square&logo=markdown)
![VSCode](https://img.shields.io/badge/Editor-VS%20Code-007ACC?style=flat-square&logo=visual-studio-code)

---

## 👤 Autor

Desenvolvido como atividade acadêmica para a disciplina **EDAA — 2026/1**.

---

*📅 Data de entrega: Fevereiro de 2026*
