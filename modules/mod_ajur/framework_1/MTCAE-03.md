---
id: MTCAE-03
version: 3.0
type: module_component
dependencies:
  - mod_argument_enhancement_nexus
  - cognitive_engine
---

# Finalidade e Escopo

Este sub-módulo do Framework 1 do MOD_AJUR, Aplicação de Standards de Prova e Articulação da Dúvida, compara a força agregada das provas com o standard jurídico aplicável e, se insuficiente, gera o argumento explícito que fundamenta a dúvida. Seu escopo é inferir se o conjunto probatório atinge a certeza exigida pelo standard e, caso contrário, comissionar o `MOD_ARGUMENT_ENHANCEMENT_NEXUS` com a missão de 'Gerar Argumento de Insuficiência Probatória', utilizando os fatores atenuantes e as provas de baixa credibilidade como premissas.

# MTCAE-03: Aplicação de Standards de Prova e Articulação da Dúvida

Compara a força agregada das provas com o standard jurídico aplicável e, se insuficiente, gera o argumento explícito que fundamenta a dúvida.

## Processos Internos

1.  Com base nas `credibility_level_inferred` das provas que suportam a narrativa dominante, inferir se o conjunto probatório atinge a certeza exigida pelo standard (identificado no `KBI IV.3`).
2.  Se o standard não for atingido, comissionar o `MOD_ARGUMENT_ENHANCEMENT_NEXUS` com a missão de 'Gerar Argumento de Insuficiência Probatória', utilizando os `attenuating_factors` e as provas de baixa credibilidade como premissas.

## Saídas Geradas

*   **ProofStandardAnalysisResult:** Objeto contendo `standard_met` (booleano), `conclusion_summary` e `reasoned_doubt_argument` (se `standard_met` for falso).
