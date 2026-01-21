# Projeto GCP + Xadrez Técnico em C++

## Visão Geral

Este projeto tem como objetivo **aprender C++ de forma profunda, prática e estratégica**, evitando exercícios triviais e focando em conceitos que **realmente diferenciam C++ de linguagens como Python e Java**.

Em vez de projetos simples (calculadora, CRUD, etc.), o foco é construir um **núcleo técnico reutilizável**, inspirado em jogos, engines e simulações.

O projeto é dividido em dois grandes blocos integrados:

* **GCP (Game Core Project)**: um núcleo técnico genérico
* **Jogo de Xadrez Técnico**: aplicação prática e controlada desse núcleo

---

## Por que este projeto existe

### Motivações principais

* Consolidar fundamentos reais de C++
* Aprender C++ como linguagem de **sistemas e alto desempenho**
* Desenvolver raciocínio próximo ao usado em engines de jogos
* Evitar reaprender conceitos já dominados em outras linguagens

### O que NÃO é objetivo

* Não é aprender lógica básica
* Não é focar em interface gráfica avançada
* Não é criar um jogo comercial

> O foco é **arquitetura, controle, clareza e performance**.

---

## O que é o GCP (Game Core Project)

O **GCP** é um **núcleo técnico reutilizável**, não um jogo.

Ele representa uma mini-engine conceitual que pode ser usada para:

* Jogos 2D simples
* Simulações
* Experimentos de física

### Responsabilidades do GCP

* Gerenciamento de memória e recursos
* Estrutura base de objetos
* Atualização de estados (update loop)
* Separação clara entre lógica e visual

---

## Componentes Técnicos do GCP

### 1. Estrutura Base do Projeto

* Separação clara `.hpp` / `.cpp`
* Organização por módulos
* Código legível e sustentável

Exemplo de módulos:

* `core/`
* `math/`
* `physics/`
* `graphics/`
* `game/`

---

### 2. Matemática e Fundamentos

Foco em matemática aplicada:

* Vetores 2D
* Operações básicas (soma, produto escalar)
* Uso intenso de `const` e referências

Objetivo:

> Treinar **design de tipos matemáticos eficientes** em C++.

---

### 3. Motor de Física 2D (Simplificado)

Mesmo sendo um jogo de tabuleiro, a física será usada como **exercício conceitual**.

Inclui:

* Sistema de posições
* Velocidade e aceleração (conceitual)
* Atualização por delta time
* Detecção simples de colisão (caixa)

> A física aqui é pedagógica, não realista.

---

### 4. Engine Gráfica Básica

Visual simples, mas com arquitetura correta:

* Renderização de formas básicas
* Separação entre lógica e renderização
* Pipeline simples:

  * Atualização
  * Renderização

O foco NÃO é estética, e sim:

* Organização
* Fluxo de dados
* Controle do ciclo do programa

---

### 5. Gerenciamento de Recursos

Parte obrigatória do projeto.

Inclui:

* Controle explícito do tempo de vida dos objetos
* Uso de RAII
* Evitar vazamentos de memória
* Uso consciente de ponteiros

Exemplos:

* Recursos gráficos
* Objetos do jogo

---

## Aplicação: Jogo de Xadrez Técnico

O xadrez será a **aplicação prática** do GCP.

### Por que xadrez?

* Regras bem definidas
* Estrutura clara
* Baixa dependência gráfica
* Excelente para OO e arquitetura

---

## O que será implementado no Xadrez

### 1. Modelagem Orientada a Objetos

* `Piece`
* `Board`
* `Game`
* Hierarquia controlada (sem exageros)

Foco em:

* Encapsulamento
* Clareza
* Uso correto de ponteiros e referências

---

### 2. Integração com o Motor de Física

Mesmo sendo conceitual:

* Peças possuem posição
* Movimento é tratado como transição física
* Atualização via loop do GCP

Objetivo:

> Usar a física como **ferramenta arquitetural**, não como necessidade real.

---

### 3. Renderização do Tabuleiro

* Uso da engine gráfica básica
* Renderização por camadas
* Separação total entre lógica do jogo e visual

---

### 4. Boas Práticas Obrigatórias

* Const correctness
* RAII
* Nenhum `new/delete` desnecessário
* Código previsível e limpo

---

## O que será aprendido com este projeto

### Técnicamente

* C++ moderno e consciente
* Ponteiros vs referências
* Gerenciamento de memória
* Organização de projetos reais

### Mentalmente

* Pensar como programador de engine
* Projetar antes de codar
* Escrever menos código, mais correto

---

## Escopo e Tempo

* Projetos pequenos e controlados
* Iterações curtas
* Cada módulo pode ser desenvolvido em ~1 hora

---

## Resultado Esperado

Ao final do projeto:

* Capacidade real de usar C++ para sistemas complexos
* Base sólida para jogos, simulações e física computacional
* Confiança para avançar para engines maiores

---

> **Este projeto não é sobre terminar rápido.**
> É sobre terminar sabendo exatamente o que está fazendo.
