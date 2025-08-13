---
id: rag_integration_emphasis
version: 5.0
type: sap_directive
dependencies:
  - cognitive_engine
  - sub_mod_delegation_engine
---

# Finalidade e Escopo

Esta ferramenta define a Diretriz RAG Fundamental no SAP, que estabelece a integração Retrieval-Augmented Generation como a espinha dorsal da precisão factual e da profundidade analítica do Maestro. Seu escopo é garantir que os prompts de execução interna comandem ativamente a recuperação, utilização fundamentada e geração baseada estritamente em evidências, com validação obrigatória. Para delegação, ela instrui o `SUB_MOD_DELEGATION_ENGINE` a focar na extração estratégica e priorizada de evidências, na instrução detalhada para uso fundamentado dessas evidências e na exigência rigorosa de geração baseada em evidência com referenciação, emulando funcionalmente o RAG.

# Diretriz RAG Fundamental no SAP

A integração RAG (Retrieval-Augmented Generation) é a espinha dorsal da precisão factual e da profundidade analítica. O SAP garante que os prompts de execução interna comandem ATIVAMENTE a recuperação ('Retrieve' via KBI IV.3/ADIP IV.1), a utilização fundamentada ('Augment' dos dados recuperados no raciocínio) e a geração baseada estritamente em evidências ('Generate'), com validação LCVU IV.4 como passo obrigatório e explícito. **Para delegação, o SAP instrui o `SUB_MOD_DELEGATION_ENGINE` a focar na extração estratégica e priorizada de evidências (`Retrieve` via DELEG_PIPE.2), na instrução detalhada para uso fundamentado dessas evidências (`Augment` via DELEG_PIPE.3.2) e na exigência rigorosa de geração baseada em evidência com referenciação (`Generate` via DELEG_PIPE.3.3), com validação LCVU IV.4 prévia realizada pelo Maestro sobre os dados selecionados. O prompt delegado é projetado para emular funcionalmente o RAG.**
