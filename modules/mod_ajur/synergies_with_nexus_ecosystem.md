---
id: synergies_with_nexus_ecosystem
version: 3.0
type: module_component
dependencies:
  - mod_relatoria
  - cognitive_engine
---

# Finalidade e Escopo

Este componente do módulo MOD_AJUR define as Sinergias com o Ecossistema Nexus. Seu escopo é detalhar como o MOD_AJUR consome informações de outros módulos (MOD_RELATORIA, módulos de domínio, LCVU IV.4 e SFU IV.5), orquestra o `MOD_ARGUMENT_ENHANCEMENT_NEXUS` como seu principal motor de engenharia narrativa, e aprimora transversalmente as capacidades de outros módulos, especialmente a análise de vieses cognitivos e as heurísticas de eficiência.

# Sinergias com o Ecossistema Nexus

*   **Consome de:** `MOD_RELATORIA` (para a base fática imparcial), todos os módulos de domínio (`MOD_PENAL`, `MOD_CIVIL`, etc., para entender as teses), `LCVU IV.4` e `SFU IV.5` (que são fundamentalmente aprimorados por este módulo).
*   **Orquestra:** `MOD_ARGUMENT_ENHANCEMENT_NEXUS` (como seu principal motor de engenharia narrativa).
*   **Aprimora Transversalmente:** As capacidades do `MOD_AJUR`, especialmente a análise de vieses cognitivos (AJUR.3) e as heurísticas de eficiência (AJUR.2), podem ser invocadas por outros módulos para aprimorar suas próprias análises e outputs.
