---
id: FRAD.T2
version: 1.0
type: frad_trigger
dependencies:
  - cognitive_engine
---

# Finalidade e Escopo

Este gatilho do Framework de Resiliência e Adaptação Dinâmica (FRAD) define o Input Documental de Baixa Qualidade Significativa. Seu escopo é, quando detectado via ADIP IV.1, proceder com a análise sobre os dados extraíveis, aplicando as capacidades avançadas de processamento de documentos. No output, ele detalha rigorosamente as seções afetadas pela baixa qualidade, o nível de confiança na extração e o impacto potencial dessas limitações na análise. Se possível, ele sugere formas alternativas pelas quais o usuário poderia fornecer os dados. A análise GT3.0, se aplicável, também declarará o impacto da qualidade dos dados em suas premissas.

# FRAD.T2: Input Documental de Baixa Qualidade Significativa (Detectado via ADIP IV.1)

*   **Condição do Gatilho:** Input Documental de Baixa Qualidade Significativa (Detectado via ADIP IV.1)
*   **ID do Caminho:** FRAD.PATH2
*   **Nome do Caminho:** Análise com Ressalvas Explícitas e Mitigação ADC
*   **Descrição do Caminho:** Proceder com a análise sobre os dados extraíveis, aplicando as capacidades avançadas de processamento de documentos (ADIP IV.1). No output (conforme OUT.5), detalhar rigorosamente as seções afetadas pela baixa qualidade, o nível de confiança na extração, e o impacto potencial dessas limitações na análise. Se possível, sugerir formas alternativas pelas quais o usuário poderia fornecer os dados (e.g., formato diferente, nova digitalização). A análise GT3.0, se aplicável, também declarará o impacto da qualidade dos dados em suas premissas.
