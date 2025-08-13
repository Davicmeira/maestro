---
id: MTCAE-04
version: 3.0
type: module_component
dependencies:
  - cognitive_engine
---

# Finalidade e Escopo

Este sub-módulo do Framework 1 do MOD_AJUR, Aplicação Autônoma de Mecanismos de Gestão da Prova, identifica em tempo real, com base no contexto do caso, a aplicabilidade de presunções ou da distribuição dinâmica do ônus da prova. Seu escopo é analisar o contexto fático e as alegações para identificar padrões que ativam mecanismos de gestão da prova e, para cada padrão identificado, gerar um alerta com a fundamentação jurídica e o impacto prático na análise do caso.

# MTCAE-04: Aplicação Autônoma de Mecanismos de Gestão da Prova

Identifica em tempo real, com base no contexto do caso, a aplicabilidade de presunções ou da distribuição dinâmica do ônus da prova.

## Processos Internos

1.  Analisar o contexto fático e as alegações para identificar padrões que, com base no conhecimento jurídico fundamental (`KBI IV.3`), ativam mecanismos de gestão da prova. Exemplos de padrões a serem detectados: (a) Relação de consumo evidente; (b) Hipossuficiência técnica ou econômica de uma parte; (c) Alegação de fato negativo (prova diabólica); (d) Fatos que se enquadram em presunções legais.
2.  Para cada padrão identificado, gerar um alerta com a fundamentação jurídica e o impacto prático na análise do caso.

## Saídas Geradas

*   **ProofManagementAnalysis:** Objeto contendo `is_applicable` (booleano) e `findings` (lista de objetos com `mechanism`, `legal_basis`, `factual_trigger` e `impact_on_analysis`).
