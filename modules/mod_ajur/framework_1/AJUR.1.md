---
id: AJUR.1
version: 3.0
type: module_component
dependencies:
  - mod_relatoria
  - mod_argument_enhancement_nexus
  - cognitive_engine
---

# Finalidade e Escopo

Este componente do módulo MOD_AJUR define o Framework 1: Construção da Premissa Fática sob Incerteza. Seu escopo é transformar um conjunto de evidências brutas em uma premissa fática justificada e ponderada, pronta para a aplicação do direito. Ele inclui sub-módulos para análise forense de prova técnica/pericial, análise comparativa e síntese estratégica (Matriz de Consistência Fática), geração de hipóteses fáticas plausíveis (raciocínio abdutivo), análise estruturada da força probatória, aplicação de standards de prova e articulação da dúvida, e aplicação autônoma de mecanismos de gestão da prova.

# AJUR.1: Framework 1: Construção da Premissa Fática sob Incerteza

Pipeline que transforma um conjunto de evidências brutas em uma premissa fática justificada e ponderada, pronta para a aplicação do direito.

## Sub-módulos

- **AJUR.1.1: Análise Forense de Prova Técnica/Pericial:** Realiza uma dissecação crítica e aprofundada de laudos periciais para avaliar sua validade, metodologia e coerência lógico-conclusiva.

- **AJUR.1.2: Análise Comparativa e Síntese Estratégica (Matriz de Consistência Fática):** Executa uma análise sistemática e comparativa de todas as fontes de prova (documental, pericial, testemunhal) em relação às alegações fáticas nucleares do caso. O sistema constrói uma 'Matriz de Consistência Fática' para visualizar a convergência e a divergência probatória, culminando em uma síntese estratégica acionável para o julgador ou parecerista.

- **MTCAE-01: Geração de Hipóteses Fáticas Plausíveis (Raciocínio Abdutivo):** Diante de lacunas ou contradições probatórias, o sistema gera as narrativas mais plausíveis que explicam o conjunto de fatos, aplicando a Inferência à Melhor Explicação (IME).

- **MTCAE-02: Análise Estruturada da Força Probatória:** Avalia cada prova individualmente e em conjunto, gerando uma nota de valoração textual e justificada que fundamenta a credibilidade atribuída.

- **MTCAE-03: Aplicação de Standards de Prova e Articulação da Dúvida:** Compara a força agregada das provas com o standard jurídico aplicável e, se insuficiente, gera o argumento explícito que fundamenta a dúvida.

- **MTCAE-04: Aplicação Autônoma de Mecanismos de Gestão da Prova:** Identifica em tempo real, com base no contexto do caso, a aplicabilidade de presunções ou da distribuição dinâmica do ônus da prova.
