# DevCalc API

![CI](https://github.com/Abrahao02/devcalc-api/actions/workflows/ci.yml/badge.svg)

## 🚀 Execução Manual

O pipeline pode ser executado manualmente via aba "Actions" do GitHub, através do botão `Run workflow`. Isso permite selecionar parâmetros personalizados (como executar ou não testes/linting) e simular cenários reais de CI/CD.

## 🧪 Experimento de Falha no Pipeline

Durante o desenvolvimento do pipeline, foi propositalmente inserido um erro de execução (`exit 1`) para verificar a detecção de falhas. O erro foi identificado na aba de *Actions* no GitHub, onde os logs mostraram exatamente onde a falha ocorreu. Após isso, o erro foi corrigido e uma nova execução foi feita com sucesso.


DevCalc é uma API REST escrita em Java que oferece operações matemáticas simples (adição, subtração, multiplicação e divisão). O projeto tem como objetivo servir de base para a construção de um pipeline de CI/CD utilizando **GitHub Actions**.

## 📌 Objetivo

Este projeto foi desenvolvido como ponto de partida para validar e demonstrar práticas de integração e entrega contínuas (CI/CD), incluindo:

- Verificação de código
- Testes automatizados
- Build e empacotamento
- Simulação de deploy
- Execução manual de workflows e validação de pull requests

## 🛠️ Tecnologias e Ferramentas

- **Java 17**
- **Maven** como sistema de build
- **Javalin** como framework web para criação da API REST
- **JUnit** para testes automatizados
- **GitHub Actions** para pipelines CI/CD

## 🗂️ Estrutura do Projeto

```text
devcalc-api/
├── .github/
│   └── workflows/
│       ├── hello.yml
│       └── ci.yml
├── src/
│   ├── main/
│   │   └── java/
│   │       └── com/
│   │           └── devcalc/
│   │               ├── App.java
│   │               └── CalculatorService.java
│   └── test/
│       └── java/
│           └── com/
│               └── devcalc/
│                   └── CalculatorServiceTest.java
├── evidencias/
│   └── (prints do terminal e execuções dos workflows)
├── pom.xml
└── README.md
