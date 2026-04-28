# Auditoria de Maturidade em Ecossistemas LLM  
## Projeto: screenpipe

---

## Equipe

- Gian Glauberty Santos Nascimento – 202300061616 (Eixo III - Arquitetura e Modelagem)
- Pedro César Figueiredo Carneiro – 202300061732 (Eixo IV - Verificação e Validação)
- Pedro Miguel Castro França – 202300061741 (Eixo II - Engenharia de Requisitos)
- João Marcelo Silva da Conceição – 202300095820 (Eixo VI - Estrategia e Plano de Melhoria)
- Renner do Nascimento Brito – 202300061797 (Eixo V - Qualidade de Software e Conclusão da Auditoria)
- Paulo Gabriel de Oliveira Cardoso – 202000047735 (Eixo I - Ciclo de Vida)

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
- Gestão de riscos

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

## Estrutura do repositório separado por eixos

[Análise Ciclo de Vida](./Eixo%20I%20-%20Ciclo%20de%20Vida/ciclodevida.md)

[Análise Engenharia de Requisitos](./Eixo%20II%20-%20Engenharia%20de%20Requisitos/reg.md/)

[Análise Arquitetura e Modelagem](./Eixo%20III%20-%20Arquitetura%20e%20Modelagem/analise-arq.md/)

[Análise Verificação e Validação](./Eixo%20IV%20-%20Verificação%20e%20Validação/analise_v&v.md)

[Análise Qualidade](./Eixo%20V%20-%20Qualidade/analise-qualidade-mais-conclusão.md)

[Estratégia e Plano de Melhoria](./Eixo%20VI%20-%20Plano%20de%20melhoria/analise-plano.md)

---

## Principais Achados

- Uso de ciclo de vida ágil (issues + PRs)
- Rastreamento de requisitos não formalizado
- Arquitetura modular
- Ausência de validação robusta da IA
- Falta de processos formais de qualidade

---

## Vídeo da Auditoria
 Link do vídeo:  

---

## Considerações Finais

O projeto apresenta boas práticas técnicas e alinhamento com metodologias ágeis, porém possui oportunidades de melhoria relacionadas à maturidade de processos, especialmente em requisitos, validação de IA e qualidade de software.

---
