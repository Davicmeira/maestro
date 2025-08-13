---
id: MTCAE-05
version: 3.0
type: module_component
dependencies:
  - cognitive_engine
---

# Finalidade e Escopo

Este sub-módulo do Framework 2 do MOD_AJUR, Identificação de Questão de Resolução Prioritária ('Nó Górdio'), identifica a questão prejudicial ou preliminar cuja análise prioritária tem o potencial de resolver a demanda ou tornar desnecessária a análise de mérito, otimizando o julgamento. Seu escopo é construir um modelo mental de dependências lógicas entre os argumentos, identificar argumentos do tipo 'preliminar' ou 'prejudicial' que, se acolhidos, resolvem o processo sem análise de mérito, e gerar um alerta estratégico recomendando a ordem de análise.

# MTCAE-05: Identificação de Questão de Resolução Prioritária ('Nó Górdio')

Identifica a questão prejudicial ou preliminar cuja análise prioritária tem o potencial de resolver a demanda ou tornar desnecessária a análise de mérito, otimizando o julgamento.

## Processos Internos

1.  Construir um modelo mental de dependências lógicas entre os argumentos.
2.  Identificar argumentos do tipo 'preliminar' ou 'prejudicial' (e.g., prescrição, decadência, ilegitimidade, inépcia) que, se acolhidos, resolvem o processo sem análise de mérito.
3.  Gerar um alerta estratégico recomendando a ordem de análise.

## Saídas Geradas

*   **AlertaDeEficienciaDecisoria:** Objeto contendo `is_applicable` (booleano), `recommendation` e `justification`.
