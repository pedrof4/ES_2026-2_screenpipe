# Plano de Melhoria de Processo: Projeto Screenpipe

**Eixo: Estratégia e Plano de Melhoria** 

**Projeto Auditado:** [screenpipe](https://github.com/mediar-ai/screenpipe)

## 1. Introdução
Este plano visa corrigir as lacunas identificadas na auditoria do projeto screenpipe, focando nos níveis de maturidade **MPS.BR Nível G** e **CMMI-DEV v2.0 Nível 2**. Como o screenpipe lida com captura de dados e processamento por IA, a formalização é essencial para garantir confiança e rastreabilidade.

## 2. Síntese dos Gaps Identificados
A auditoria mostrou que o projeto tem uma base técnica forte, mas carece de gestão formal:

| Eixo | Gap Central | Impacto | Nível MPS.BR Atual |
|------|------------|---------|-------------------|
| **GRE (Eixo II)** | Rastreabilidade manual; ausência de RFCs. | Dificulta a previsão de impactos em mudanças multiplataforma. | Abaixo do Nível G |
| **V&V (Eixo IV)** | Ausência de validação semântica para IA. | Risco de alucinações e baixa confiabilidade nos resultados. | Parcial |

## 3. Ação 1 — Rastreabilidade Formal de Requisitos (GRE)

### 3.1 Problema Central
A definição de requisitos é informal (via Issues). Casos complexos, como o conflito no Windows (Issue #2495) ou falhas de áudio no macOS (Issue #2903), são resolvidos sem um documento de impacto ou discussão estruturada prévia (RFC).

### 3.2 Medidas Propostas
* **Matriz de Rastreabilidade (RTM):** Criar um ficheiro `TRACEABILITY.md` para ligar formalmente cada Issue ao seu respetivo Pull Request e módulo de código afetado.
* **Implementação de RFCs:** Criar o diretório `docs/rfcs/`. Mudanças estruturais devem obrigatoriamente passar por uma proposta técnica antes da implementação para avaliar riscos em diferentes sistemas operativos.

## 4. Ação 2 — Validação de Saída da IA (V&V)

### 4.1 Problema Central
O projeto verifica se o código funciona (build/linting), mas não valida se a resposta da IA é correta. Não há testes automáticos para garantir que o processamento de IA atende às expectativas do utilizador final.

### 4.2 Medidas Propostas
* **Integração de Golden Datasets:** Criar conjuntos de dados de referência no GitHub Actions para testar se a IA extrai a informação correta das janelas capturadas.
* **Frameworks de Avaliação:** Adotar ferramentas para medir a precisão da IA (evitando alucinações), tornando a qualidade do processamento algo auditável e não apenas subjetivo.

## 5. Cronograma de Execução (4 Semanas)
* **Semana 1:** Criação de templates de Issues e estrutura de RFCs.
* **Semana 2:** Mapeamento retroativo dos requisitos de áudio e Windows no ficheiro de rastreabilidade.
* **Semana 3:** Implementação de testes de validação semântica para o módulo de IA no CI.
* **Semana 4:** Atualização do `CONTRIBUTING.md` com as novas regras de qualidade.

---

Este plano foi desenhado para transformar o seu projeto de um modelo puramente ágil e informal para um nível de **Gestão Controlada**, conforme exigido pelas normas de Engenharia de Software.
