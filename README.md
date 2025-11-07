# 🎮 Projeto **QUEST** — Jogo de Perguntas e Respostas

Este projeto consiste em um jogo de perguntas e respostas desenvolvido em **C**, inspirado na dinâmica do jogo **Perguntados (Trivia Crack)**.
O trabalho foi desenvolvido individualmente durante os primeiros semestres da graduação, com o objetivo de aplicar conceitos de **estrutura de dados**, **manipulação de arquivos JSON** e **organização de código em C**, integrando teoria e prática no desenvolvimento de um sistema interativo em console.

---

## 🧠 Sobre o Projeto

O **QUEST** é um jogo que apresenta ao jogador perguntas de múltipla escolha organizadas por categorias.
As perguntas são carregadas dinamicamente a partir de um **arquivo JSON**, que armazena as informações de cada questão, suas alternativas, o gabarito e a categoria correspondente.

O jogador pode:

* Iniciar um novo jogo e escolher uma categoria;
* Visualizar créditos do projeto;
* Consultar o placar (função planejada para implementação futura).

O projeto reforça o uso de **estruturas compostas**, **ponteiros**, **listas encadeadas** e **leitura de dados externos**, além de explorar a utilização da biblioteca **json-c** para interpretar arquivos JSON.

---

## 🧩 Funcionalidades Principais

* 🧍‍♀️ Criação e gerenciamento de jogador
* 🧾 Leitura de perguntas e alternativas a partir de um arquivo **data.json**
* 📚 Exibição de categorias temáticas (História, Geografia, Ciências, Artes, Cinema, Geral)
* 🏆 Sistema de pontuação (em expansão)
* 💾 Estrutura modular e uso de ponteiros e structs

---

## 🧱 Estrutura do Código

### Principais estruturas:

* `t_jogador` → Armazena nome e pontuação do jogador.
* `t_pergunta` → Contém o enunciado, alternativas, gabarito e categoria.
* `t_no_pergunta` → Nó para lista encadeada de perguntas.

### Principais funções:

* `inicio()` → Exibe o menu inicial e controla o fluxo do jogo.
* `novo_jogo()` → Permite escolher a categoria e iniciar a partida.
* `exibir_creditos()` → Mostra as informações do projeto e do professor.
* `placar()` → Função destinada à exibição de pontuações (em desenvolvimento).

---

## 📂 Estrutura de Pastas

```
📦 quest
 ┣ 📜 main.c
 ┣ 📜 data.json
 ┣ 📜 Makefile (opcional)
 ┗ 📄 README.md
```

---

## 🔧 Tecnologias Utilizadas

* **Linguagem:** C
* **Bibliotecas:**

  * [`json-c`](https://github.com/json-c/json-c) — para leitura e interpretação do arquivo JSON
  * `stdio.h`, `stdlib.h` — para entrada, saída e manipulação de memória

---

## 🧪 Exemplo de Execução

```
1 - NOVO JOGO
2 - EXIBIR CRÉDITOS
3 - PLACAR
4 - SAIR
OPÇÃO: 1

Bem-vindos ao jogo Quest!
Escolha uma das seguintes categorias:

1- HISTÓRIA
2- GEOGRAFIA
3- CIÊNCIAS
4- ARTES
5- CINEMA
6- GERAL
OPÇÃO: 3
```

Em seguida, o jogo lê a pergunta correspondente do arquivo `data.json` e exibe as alternativas para o jogador responder.

---

## 👩‍💻 Desenvolvimento

**Desenvolvido por:** Giulia Campelo Bezerra
**Professor:** Daniel Souza
**Disciplina:** Lógica de Programação / Estrutura de Dados (Anos Iniciais – Ciência da Computação / IESB)

---

## 🎯 Objetivo Acadêmico

Este projeto teve como propósito:

* Aplicar **conceitos básicos de lógica de programação e estruturas de dados**.
* Compreender a **leitura e manipulação de arquivos JSON em C**.
* Desenvolver habilidades de **resolução de problemas e implementação estruturada de código**.

---

## 🚀 Possíveis Melhorias

* Implementar sistema completo de pontuação e ranking.
* Armazenar resultados em arquivo externo.
* Adicionar novas categorias e perguntas.
* Criar uma interface gráfica simples (ex: com SDL ou ncurses).
