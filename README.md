# 📊 Auditoria de Maturidade em Ecossistemas LLM  
## Projeto: ScreenPipe

---

## 👥 Equipe

- Gian Glauberty Santos Nascimento – 202300061616
- Pedro César Figueiredo Carneiro – 202300061732
- Pedro Miguel Castro França – 202300061741
- João Marcelo Silva da Conceição – 202300095820
- Renner do Nascimento Brito – 202300061797
- Paulo Gabriel de Oliveira Cardoso – 202000047735

---

## 🎯 Objetivo

Este repositório tem como objetivo apresentar uma auditoria de maturidade de um projeto baseado em Modelos de Linguagem (LLMs), utilizando como referência os modelos **CMMI-DEV (v2.0)** e **MPS.BR**.

O projeto analisado foi o ScreenPipe, uma aplicação open source que integra captura de dados de tela com processamento por inteligência artificial.

---

## 🔎 Sobre o Projeto Analisado

O ScreenPipe é um sistema que permite capturar, processar e analisar informações provenientes da tela do usuário, utilizando técnicas de inteligência artificial e modelos de linguagem.

Sua arquitetura é modular, composta por:
- Captura de dados
- Pipeline de processamento
- Integração com IA
- Geração de saída

O projeto segue um modelo de desenvolvimento colaborativo baseado em GitHub, utilizando issues, pull requests e versionamento contínuo.

🔗 Repositório oficial:  
https://github.com/screenpipe/screenpipe

---

## 🧪 Metodologia da Auditoria

A análise foi realizada com base em cinco eixos principais:

### 🔵 1. Ciclo de Vida (GPR)
- Análise de releases e issues
- Identificação de práticas ágeis

### 🟢 2. Engenharia de Requisitos (GRE)
- Rastreamento de requisitos via:
  - Issues
  - Pull Requests
  - Código

### 🟣 3. Arquitetura (PJR)
- Avaliação da estrutura modular
- Identificação de desacoplamento da IA

### 🟠 4. Verificação e Validação (V&V)
- Análise de workflows e testes
- Avaliação da validação de IA

### 🔴 5. Qualidade (GQA)
- Verificação de padrões de contribuição
- Análise de práticas de qualidade

---

## 🔗 Rastreabilidade de Requisitos
Não foram identificados processos formais de RFC (Request for Comments) no projeto. As propostas de funcionalidades e melhorias são realizadas diretamente por meio de Issues no GitHub, o que caracteriza uma abordagem mais ágil e menos formal na definição de requisitos.

### Requisito 1 (Correção de falha na gravação de áudio)
Issue: Relato de erro na gravação de áudio em ambiente macOS (https://github.com/screenpipe/screenpipe/issues/2903)
Pull Request: Correção implementada no módulo de captura de áudio (https://github.com/screenpipe/screenpipe/pull/2905)
Código: Alterações realizadas em arquivos relacionados ao sistema de captura de áudio (https://github.com/screenpipe/screenpipe/pull/2905/changes)

### Requisito 2 (O servidor deixa de reiniciar após detectar uma instância já em execução durante a inicialização)
Issue:Descrição do bug (https://github.com/screenpipe/screenpipe/issues/2880)
Pull Request: Explicação da função de correção (https://github.com/screenpipe/screenpipe/pull/2892)
Código: Alterações na função do arquivo principal relacionados à conexão com o servidor (https://github.com/screenpipe/screenpipe/pull/2892/changes)

### Requisito 3A aplicação no Windows entra em conflito no executor de loop de eventos “tao”
Issue: Relatório especificando a origem do erro (https://github.com/screenpipe/screenpipe/issues/2495)
Pull Request: Explicação da solução para o “crash” (https://github.com/screenpipe/screenpipe/pull/2535)
Código: Alterações em 2 seções de arquivos direcionadas ao funcionamento no Windows (https://github.com/screenpipe/screenpipe/pull/2535/changes)

Foi possível identificar rastreabilidade parcial entre requisitos e implementação por meio da relação entre Issues, Pull Requests e código. No entanto, essa rastreabilidade não é formalmente documentada, o que pode dificultar a gestão de mudanças.
---

## 🏗️ Arquitetura (Visão Simplificada)
ScreenPipeApp
├── CaptureService
├── ProcessingPipeline
├── LLMService
├── OutputHandler

Diagrama visual
!(./diagramas/arq.jpeg)

A arquitetura demonstra separação de responsabilidades e desacoplamento parcial da camada de inteligência artificial.

---

## ⚙️ Principais Achados

- Uso de ciclo de vida ágil (issues + PRs)
- Rastreamento de requisitos não formalizado
- Arquitetura modular
- Ausência de validação robusta da IA
- Falta de processos formais de qualidade

---

## 🚀 Plano de Melhoria

1. Implementar rastreabilidade formal de requisitos  
2. Adotar mecanismos de validação das respostas da IA  

---

## 🎥 Vídeo da Auditoria

📺 Link do vídeo:  


---

## 📁 Estrutura do Repositório

/docs → documentação
/diagramas → UML e imagens
/anotacoes → análises da equipe

---

## 📌 Considerações Finais

O projeto apresenta boas práticas técnicas e alinhamento com metodologias ágeis, porém possui oportunidades de melhoria relacionadas à maturidade de processos, especialmente em requisitos, validação de IA e qualidade de software.

---
