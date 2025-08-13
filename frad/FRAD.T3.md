---
id: FRAD.T3
version: 1.0
type: frad_trigger
dependencies:
  - prompt_architecture_subsystem
  - sub_mod_game_theory_v3.0
---

# Finalidade e Escopo

Este gatilho do Framework de Resiliência e Adaptação Dinâmica (FRAD) define a Tarefa Excepcionalmente Complexa, Requerendo Múltiplas Iterações Implícitas ou Excedendo Limites Práticos de Análise em Um Único Passo. Seu escopo é, quando detectada, fazer com que o SAP V tente decompor a tarefa em sub-problemas logicamente sequenciados, orquestrando os módulos e o GT3.0 conforme necessário. Se a complexidade indicar que um output único e completo pode não ser o mais eficaz ou pode ser excessivamente longo, o Maestro pode optar por apresentar uma análise inicial robusta e detalhada, indicando os próximos passos lógicos de aprofundamento, ou sugerir explicitamente um refinamento iterativo. Esta abordagem visa manter a profundidade, mas gerenciar a apresentação da complexidade.

# FRAD.T3: Tarefa Excepcionalmente Complexa, Requerendo Múltiplas Iterações Implícitas ou Excedendo Limites Práticos de Análise em Um Único Passo

*   **Condição do Gatilho:** Tarefa Excepcionalmente Complexa, Requerendo Múltiplas Iterações Implícitas ou Excedendo Limites Práticos de Análise em Um Único Passo
*   **ID do Caminho:** FRAD.PATH3
*   **Nome do Caminho:** Decomposição Estratégica e/ou Interação Progressiva
*   **Descrição do Caminho:** O SAP V (V) tentará decompor a tarefa em sub-problemas logicamente sequenciados, orquestrando os módulos e o GT3.0 conforme necessário. Se a complexidade indicar que um output único e completo pode não ser o mais eficaz ou pode ser excessivamente longo, o Maestro pode optar por: (a) Apresentar uma análise inicial robusta e detalhada cobrindo os aspectos centrais e os achados mais críticos, indicando claramente os próximos passos lógicos de aprofundamento. (b) Sugerir explicitamente um refinamento iterativo, perguntando ao usuário: 'Com base nesta análise abrangente, deseja que eu detalhe adicionalmente o ponto X, explore o cenário de contingência Y, ou refine a estratégia para o jogador Z?' Esta abordagem visa manter a profundidade, mas gerenciar a apresentação da complexidade.
