# Auditoria de Maturidade: Projeto Screenpipe

**Eixo:** Qualidade (GQA) e Considerações Finais  
**Projeto Auditado:** screenpipe  

---

## 5. Eixo V — Gerência de Garantia da Qualidade (GQA)

### 5.1 Problema Central
A garantia da qualidade no *screenpipe* concentra-se quase exclusivamente na **Verificação Técnica** (se o código compila e segue o estilo), mas falha na **Garantia de Processo**. Sob as normas **MPS.BR Nível G** e **CMMI-DEV v2.0**, a qualidade exige que os processos de gestão sejam auditáveis e repetíveis, o que hoje é suplantado por uma cultura de desenvolvimento puramente orgânica.

### 5.2 Análise de Práticas Atuais
* **Integração Contínua (CI):** O projeto utiliza *GitHub Actions* para automação de testes de unidade e *linting*. Embora eficaz para a integridade do código, não assegura que os requisitos levantados no Eixo II foram satisfeitos.
* **Inspeção por Pares:** A revisão de código via *Pull Requests* é o principal mecanismo de controle. No entanto, não existem *checklists* formais de qualidade, tornando a aceitação de novas funcionalidades dependente da subjetividade do revisor.

### 5.3 Lacunas de Maturidade (Gaps)
* **Ausência de Auditoria Interna:** Não há um papel definido para validar se o plano de projeto e o ciclo de vida estão sendo seguidos, o que caracteriza um processo de Nível 1 (Inicial).
* **Métricas de Qualidade em IA:** Por integrar LLMs, o projeto carece de indicadores de desempenho específicos (KPIs) para medir a acurácia das extrações e a taxa de falha semântica dos modelos de linguagem.

---

## 6. Considerações Finais

A auditoria realizada no projeto **screenpipe** demonstra que o sistema possui uma excelência técnica e arquitetural superior à sua maturidade de processos. Atualmente, o projeto classifica-se no **Nível 1 (Inicial)**, com dependência crítica da competência individual dos desenvolvedores.

### 6.1 Síntese do Diagnóstico
* **Formalização vs. Agilidade:** O projeto se beneficia da velocidade do modelo *Open Source*, mas a falta de uma Gerência de Requisitos (GRE) e de Qualidade (GQA) formalizada gera riscos de sustentabilidade e rastreabilidade a longo prazo.
* **Impacto da IA no Cotidiano:** Como o software processa dados sensíveis (captura de tela), a maturidade de processo torna-se um requisito ético. A transição para o **Nível 2 (Gerenciado)** é imperativa para que o sistema possa ser utilizado em ambientes corporativos que exigem conformidade e previsibilidade.

### 6.2 Veredito Técnico
O *screenpipe* é uma solução inovadora com alto potencial de mercado. No entanto, para atingir os padrões de maturidade do **CMMI** e **MPS.BR**, deve evoluir de uma gestão "baseada em heróis" para uma gestão baseada em processos documentados, auditáveis e mensuráveis. O sucesso futuro da ferramenta dependerá do equilíbrio entre sua capacidade de inovação e o rigor da sua engenharia de processos.

---

**Auditor Responsável:** Renner Brito  
**Instituição:** Universidade Federal de Sergipe (UFS)  
**Data:** 28 de abril de 2026
