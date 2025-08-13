---
id: MTCAE-06
version: 3.0
type: module_component
dependencies:
  - cognitive_engine
---

# Finalidade e Escopo

Este sub-módulo do Framework 2 do MOD_AJUR, Ponderação da Relevância Argumentativa, classifica os argumentos para focar a energia analítica nos pontos que efetivamente podem decidir a causa. Seu escopo é analisar a conexão direta de cada argumento com o pedido principal ou com a causa de pedir central, e classificar o argumento como 'Estrutural', 'Acessório' ou 'Periférico'. O output da análise deve ser um relatório que orienta o julgador a focar sua resposta nos argumentos 'Estruturais'.

# MTCAE-06: Ponderação da Relevância Argumentativa

Classifica os argumentos para focar a energia analítica nos pontos que efetivamente podem decidir a causa.

## Processos Internos

1.  Para cada argumento, analisar sua conexão direta com o pedido principal ou com a causa de pedir central.
2.  Classificar o argumento como: (a) 'Estrutural': ataca ou defende o núcleo da causa; (b) 'Acessório': reforça um argumento estrutural mas não se sustenta sozinho; (c) 'Periférico': de natureza retórica ou fática secundária.
3.  O output da análise deve ser um relatório que orienta o julgador a focar sua resposta nos argumentos 'Estruturais'.

## Saídas Geradas

*   **ArgumentRelevanceMap:** Objeto contendo `structural_arguments`, `accessory_arguments` e `peripheral_arguments`.
