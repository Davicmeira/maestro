---
id: MTCAE-02
version: 3.0
type: module_component
dependencies:
  - cognitive_engine
---

# Finalidade e Escopo

Este sub-módulo do Framework 1 do MOD_AJUR, Análise Estruturada da Força Probatória, avalia cada prova individualmente e em conjunto. Seu escopo é gerar uma nota de valoração textual e justificada que fundamenta a credibilidade atribuída a cada prova relevante. Ele realiza uma análise baseada em primeiros princípios, avaliando a natureza da fonte, consistência interna, consistência externa (corroboração ou contradição por outras provas) e o interesse da fonte (vieses ou motivações).

# MTCAE-02: Análise Estruturada da Força Probatória

Avalia cada prova individualmente e em conjunto, gerando uma nota de valoração textual e justificada que fundamenta a credibilidade atribuída.

## Processos Internos

1.  Para cada prova relevante, realizar uma análise baseada em primeiros princípios, avaliando: (a) Natureza da Fonte (confiabilidade intrínseca, e.g., perícia vs. depoimento de parte); (b) Consistência Interna do conteúdo; (c) Consistência Externa (corroboração ou contradição por outras provas, validado via LCVU IV.4); (d) Interesse da Fonte (existência de vieses ou motivações, inferido via CIE IV.2).
2.  Consolidar a análise em uma 'Nota de Valoração Probatória' estruturada e textual para cada prova relevante.

## Saídas Geradas

*   **EvidentiaryValuationNotes:** Lista de objetos `NotaDeValoracaoProbatoria` contendo `evidence_id`, `reference`, `credibility_level_inferred`, `justification` (com `reinforcing_factors` e `attenuating_factors`) e `valuation_conclusion`.
