# Auditoria de Maturidade em Ecossistemas LLM  
## Projeto: screenpipe

---

## Equipe

- Gian Glauberty Santos Nascimento – 202300061616
- Pedro César Figueiredo Carneiro – 202300061732
- Pedro Miguel Castro França – 202300061741
- João Marcelo Silva da Conceição – 202300095820
- Renner do Nascimento Brito – 202300061797
- Paulo Gabriel de Oliveira Cardoso – 202000047735

---

## Objetivo

Este repositório tem como objetivo apresentar uma auditoria de maturidade de um projeto baseado em Modelos de Linguagem (LLMs), utilizando como referência os modelos **CMMI-DEV (v2.0)** e **MPS.BR**.

O projeto analisado foi o screenpipe, uma aplicação open source que integra captura de dados de tela com processamento por inteligência artificial.

---

## Sobre o Projeto Analisado

É um sistema que permite capturar, processar e analisar informações provenientes da tela do usuário, utilizando técnicas de inteligência artificial e modelos de linguagem.

Sua arquitetura é modular, composta por:
- Captura de dados
- Pipeline de processamento
- Integração com IA
- Geração de saída

O projeto segue um modelo de desenvolvimento colaborativo baseado em GitHub, utilizando issues, pull requests e versionamento contínuo.
 Repositório oficial:  
https://github.com/screenpipe/screenpipe

---

## Metodologia da Auditoria

A análise foi realizada com base em cinco eixos principais:

### 1. Ciclo de Vida (GPR)
- Análise de releases e issues
- Identificação de práticas ágeis

### 2. Engenharia de Requisitos (GRE)
- Rastreamento de requisitos via:
  - Issues
  - Pull Requests
  - Código

### 3. Arquitetura (PJR)
- Avaliação da estrutura modular
- Identificação de desacoplamento da IA

### 4. Verificação e Validação (V&V)
- Análise de workflows e testes
- Avaliação da validação de IA

### 5. Qualidade (GQA)
- Verificação de padrões de contribuição
- Análise de práticas de qualidade

---

## Rastreabilidade de Requisitos

[Detalhes na pasta do eixo 2](./requisitos/)


---

## Arquitetura (Visão Simplificada)

[Detalhes na pasta do eixo 3](./diagramas/)

---

## Principais Achados

- Uso de ciclo de vida ágil (issues + PRs)
- Rastreamento de requisitos não formalizado
- Arquitetura modular
- Ausência de validação robusta da IA
- Falta de processos formais de qualidade

---

## Plano de Melhoria

1. Implementar rastreabilidade formal de requisitos  
2. Adotar mecanismos de validação das respostas da IA  

[Detalhamento](./plano_de_melhoria/)

---

## Vídeo da Auditoria
 Link do vídeo:  

---

## Considerações Finais

O projeto apresenta boas práticas técnicas e alinhamento com metodologias ágeis, porém possui oportunidades de melhoria relacionadas à maturidade de processos, especialmente em requisitos, validação de IA e qualidade de software.

---
