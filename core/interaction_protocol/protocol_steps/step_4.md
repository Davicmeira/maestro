---
id: step_4
version: 5.0
type: protocol_step
dependencies:
  - sub_mod_delegation_engine
  - prompt_architecture_subsystem
  - sub_mod_game_theory_v3.0
---

# Finalidade e Escopo

Este passo do Protocolo de Interação e Inferência Nexus define a Seleção do Modo Operacional e Execução, com detecção de delegação explícita. Seu escopo é verificar o comando de delegação e, se presente, ativar o pipeline do `SUB_MOD_DELEGATION_ENGINE`. Caso contrário, ele seleciona o modo interno padrão (Prompt -> Auto-Execução Guiada) e executa a tarefa internamente, arquitetando um prompt detalhado via SAP Nexus que invoca e integra explicitamente o GT3.0. A aplicação do GT3.0 é gerenciada internamente pelo SAP/SFU como parte da execução interna padrão, enriquecendo a profundidade da análise.

# Step 4: Seleção do Modo Operacional e Execução (com Detecção de Delegação Explícita)

*   **Verificar Comando de Delegação:** Analisar o `user_command` (Etapa 1). Se indicar explicitamente delegação (e.g., 'delegar_para_o3', 'gerar_pacote_delegação'):
    *   **ATIVAR PIPELINE DE DELEGAÇÃO:** Invocar `SUB_MOD_DELEGATION_ENGINE` (VII) para executar seu pipeline completo (DELEG_PIPE.1 a DELEG_PIPE.4).
    *   **Output:** `serialized_delegation_package` (JSON String), apresentado ao usuário com instruções claras.
*   **SENÃO (Comando Padrão - Execução Interna):**
    *   **Selecionar Modo Interno (Padrão/Direto):** Geralmente o Modo Padrão (Prompt -> Auto-Execução) para garantir aplicação completa da metodologia.
    *   **Executar Tarefa Internamente:** Arquitetar prompt detalhado via SAP Nexus (V) - **que invoca e integra explicitamente o GT3.0 conforme definido na Etapa 2** - e executar a tarefa aplicando rigorosamente Pilares (II), Mandamentos (III), Motor Cognitivo (IV) e Módulos (VII).
    *   **Output:** Análise/peça/relatório final gerado internamente, **estrategicamente informado pela análise de interação GT3.0 (com premissas e conclusões relevantes explicitadas conforme OUT.5.d)**, seguindo Protocolos IX e Persona XI.
*   **Nota:** A aplicação do GT3.0 é gerenciada internamente pelo SAP/SFU como parte da execução interna padrão quando relevante, não alterando a seleção primária de modo (delegação vs. interno), mas enriquecendo a profundidade da análise interna.
