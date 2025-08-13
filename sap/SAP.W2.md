---
id: SAP.W2
version: 5.0
type: sap_workflow_step
dependencies:
  - module_registry
  - foundational_architecture
  - operational_mandates
  - cognitive_engine
  - sub_mod_game_theory_v3.0
  - mod_argument_enhancement_nexus
  - sub_mod_delegation_engine
---

# Finalidade e Escopo

Este passo do fluxo de trabalho do SAP, Seleção e Mapeamento de Recursos Cognitivos e Técnicas de Prompting, define como o Maestro identifica e parametriza os recursos necessários para a missão. Seu escopo é determinar quais Módulos Específicos, Pilares Fundamentais, Mandamentos Operacionais e Componentes Cognitivos são cruciais, incluindo a potencial invocação do MOD_ARGUMENT_ENHANCEMENT_NEXUS e a parametrização para o GT3.0. Ele também seleciona as técnicas de prompting mais adequadas e, se o modo for delegação, gera os requisitos lógicos e de referências documentais para o pipeline de delegação.

# SAP.W2: Seleção e Mapeamento de Recursos Cognitivos e Técnicas de Prompting

Identificar quais Módulos Específicos (VII), Pilares Fundamentais (II), Mandamentos Operacionais (III) e Componentes Cognitivos (IV) são cruciais para a missão incluindo a potencial invocação do MOD_ARGUMENT_ENHANCEMENT_NEXUS para refinamento de teses ou argumentos chave, especialmente quando a análise GT3.0 indicar a necessidade de alta performance argumentativa. **Determinar explicitamente a necessidade, o escopo e os parâmetros de ativação para o `SUB_MOD_GAME_THEORY_V3.0` (via SFU IV.5), definindo o nível de detalhe da análise de interação requerido.** **Selecionar as técnicas de prompting (SAP.P9) mais adequadas para a tarefa e o modo de execução.** **Se o modo for delegação, gerar o `required_nexus_logic_set` (incluindo a necessidade de traduzir insights GT3.0 e a lógica das técnicas de prompting selecionadas) e o `required_document_references_with_priorities` como input para o `DELEG_PIPE.1`.**
