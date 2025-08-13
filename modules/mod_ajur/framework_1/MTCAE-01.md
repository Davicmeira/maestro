---
id: MTCAE-01
version: 3.0
type: module_component
dependencies:
  - cognitive_engine
---

# Finalidade e Escopo

Este sub-módulo do Framework 1 do MOD_AJUR, Geração de Hipóteses Fáticas Plausíveis (Raciocínio Abdutivo), gera as narrativas mais plausíveis que explicam o conjunto de fatos diante de lacunas ou contradições probatórias, aplicando a Inferência à Melhor Explicação (IME). Seu escopo é gerar N hipóteses narrativas, avaliar um 'Escore de Plausibilidade Jurídica' para cada uma e apresentar a(s) hipótese(s) mais plausível(is) como base para a análise subsequente.

# MTCAE-01: Geração de Hipóteses Fáticas Plausíveis (Raciocínio Abdutivo)

Diante de lacunas ou contradições probatórias, o sistema gera as narrativas mais plausíveis que explicam o conjunto de fatos, aplicando a Inferência à Melhor Explicação (IME).

## Processos Internos

1.  Gerar N hipóteses narrativas que conectem os fatos estabelecidos e tentem resolver as contradições e preencher as lacunas.
2.  Para cada hipótese, avaliar um 'Escore de Plausibilidade Jurídica' derivado de: (a) Coerência Lógica Interna (LCVU IV.4); (b) Simplicidade (requer menos inferências não suportadas por prova direta); (c) Poder Explicativo (cobre o maior número de fatos); (d) Consistência com o conhecimento jurídico e fático fundamental (KBI IV.3).
3.  Apresentar a(s) hipótese(s) mais plausível(is) como a base para a análise subsequente.

## Saídas Geradas

*   **PlausibleNarrativeSynopsis:** Objeto contendo `dominant_narrative` (texto e IDs de fatos de suporte) e `alternative_narratives`.
