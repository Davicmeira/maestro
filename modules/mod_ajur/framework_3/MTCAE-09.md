---
id: MTCAE-09
version: 3.0
type: module_component
dependencies:
  - cognitive_engine
---

# Finalidade e Escopo

Este sub-módulo do Framework 3 do MOD_AJUR, Protocolo de Alertas de Risco Cognitivo, atua como um supervisor metacognitivo. Seu escopo é identificar potenciais riscos de vieses cognitivos (e.g., ancoragem, confirmação) no fluxo da análise e gerar alertas com reflexões acionáveis para o usuário, em vez de perguntas interativas. Ele detecta padrões de risco cognitivo no `WorkflowAnalysisPackage` e gera um objeto `CognitiveHazardAlert` para cada risco detectado.

# MTCAE-09: Protocolo de Alertas de Risco Cognitivo

Atua como um supervisor metacognitivo, identificando potenciais riscos de vieses cognitivos (e.g., ancoragem, confirmação) no fluxo da análise e gerando alertas com reflexões acionáveis para o usuário, em vez de perguntas interativas.

## Processos Internos

1.  **Detecção de Padrões de Risco Cognitivo:** O sistema analisa o `WorkflowAnalysisPackage` em busca de padrões que, com base em princípios de psicologia cognitiva do `KBI IV.3`, sugerem um risco de viés.
    - **Risco de Ancoragem:** Detectado se a `preliminary_hypothesis` se alinha excessivamente com a primeira peça processual analisada, ignorando contra-argumentos de peso.
    - **Risco de Confirmação:** Detectado se os `selected_evidence_ids` (provas consideradas mais relevantes) corroboram quase que exclusivamente a `preliminary_hypothesis`, enquanto provas contraditórias de alta credibilidade intrínseca foram classificadas como secundárias.
2.  **Geração do Alerta Cognitivo:** Para cada risco detectado, gerar um objeto `CognitiveHazardAlert` que não questiona, mas demonstra e sugere uma ação reflexiva.

## Saídas Geradas

*   **CognitiveHazardAlerts:** Lista de objetos `CognitiveHazardAlert` contendo `bias_type`, `detection_context`, `evidence_from_case` e `actionable_reflection_prompt`.
