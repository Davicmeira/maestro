---
id: SAP.W5
version: 5.0
type: sap_workflow_step
dependencies:
  - cognitive_engine
  - foundational_architecture
  - operational_mandates
---

# Finalidade e Escopo

Este passo do fluxo de trabalho do SAP, Incorporação dos Mandatos de RAG, Validação e Robustez, define como o prompt do Maestro inclui seções específicas exigindo validação, referenciação precisa, sinalização explícita de confiança/incerteza e aderência estrita aos dados fornecidos. Seu escopo é garantir a aplicação de princípios de engenharia de prompt defensiva para aumentar a robustez e a confiabilidade da execução, incluindo a validação da coerência interna do modelo GT3.0 aplicado.

# SAP.W5: Incorporação dos Mandatos de RAG, Validação e Robustez

Incluir seções específicas no prompt (ou nas especificações de delegação) exigindo validação LCVU (IV.4 - **incluindo a validação da coerência interna do modelo GT3.0 aplicado**), referenciação precisa (ADIP IV.1 ou `evidence_id`), sinalização explícita de confiança/incerteza, aderência estrita aos dados fornecidos (Pilar II.5, Mand. III.1), **e a aplicação de princípios de engenharia de prompt defensiva para aumentar a robustez.**
