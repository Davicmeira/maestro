---
id: SAP.W4
version: 5.0
type: sap_workflow_step
dependencies:
  - cognitive_engine
  - sub_mod_game_theory_v3.0
  - mod_argument_enhancement_nexus
  - sub_mod_delegation_engine
---

# Finalidade e Escopo

Este passo do fluxo de trabalho do SAP, Formulação de Instruções Granulares / Geração de Especificações para Delegação, define a criação das diretivas detalhadas para a execução interna do Maestro ou para a delegação a LLMs externos. Seu escopo é escrever instruções precisas usando técnicas avançadas de engenharia de prompt, incluindo diretivas explícitas para invocar e integrar o GT3.0, e para ativar o MOD_ARGUMENT_ENHANCEMENT_NEXUS quando aplicável. Para delegação, ele instrui o Delegation Engine sobre como traduzir a lógica Nexus em diretivas acionáveis, garantindo a ancoragem em evidências e um fluxo de raciocínio explícito.

# SAP.W4: Formulação de Instruções Granulares / Geração de Especificações para Delegação

*   **Para Execução Interna:** Escrever as instruções detalhadas para a execução interna usando técnicas avançadas de engenharia de prompt (Role Assignment Explícito, **aplicação explícita ou implícita das técnicas de prompting selecionadas em SAP.W2, como Chain-of-Thought Detalhado e Demonstrado no Output, RAG Ativo e Demonstrado, Chain-of-Verification interna quando aplicável, etc.**, Constraint Layering, **Output Formatting Control (Ênfase em Profundidade, Extensão, Impessoalidade, 3ª Pessoa, Referenciação Inline, Sem Vocativos)**, Few-Shot Interno para exemplos complexos, Perguntas de Auto-Reflexão). **Incluir diretivas explícitas para o SFU IV.5 invocar o GT3.0 com os parâmetros definidos em SAP.W2 e para as etapas posteriores utilizarem o `strategic_recommendations_package` de forma fundamentada e, se pertinente, com raciocínio explicitado, seguindo o fluxo da técnica de prompting escolhida.** Incluir diretivas explícitas para o SFU IV.5 invocar o GT3.0 e, se aplicável, para que o MOD_ARGUMENT_ENHANCEMENT_NEXUS seja ativado para refinar argumentos específicos com base nos outputs do GT3.0 e no contexto fático-processual consolidado.
*   **Para Delegação:** Instruir o `SUB_MOD_DELEGATION_ENGINE` sobre: como traduzir a lógica Nexus identificada (SAP.W2) em diretivas acionáveis e detalhadas (`DELEG_PIPE.3.2` - **incorporando insights chave do GT3.0 e estruturando as instruções para incentivar comportamentos análogos às técnicas de prompting eficazes, como CoT funcional, RAG funcional e CoVe funcional implícito, por meio de perguntas, checklists ou mini-frameworks**), a importância crítica da ancoragem em evidências (`DELEG_PIPE.3.3`), a necessidade de um fluxo CoT explícito e detalhado (`DELEG_PIPE.3.4`), e as especificações rigorosas de formato e conteúdo do output (`DELEG_PIPE.3.5`).
