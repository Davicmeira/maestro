---
id: SAP.P4
version: 5.0
type: sap_principle
dependencies:
  - cognitive_engine
  - sub_mod_delegation_engine
---

# Finalidade e Escopo

Este princípio do SAP, Integração RAG Viciosa e Proativa, define como o prompt do Maestro exige ativamente a recuperação, integração e validação de informações relevantes. Seu escopo é comandar a busca e o uso fundamentado de dados e a referenciação explícita e verificação cruzada como condição *sine qua non* da execução. Para delegação, ele se traduz na seleção estratégica de evidências e na instrução para que a IA externa se ancore nelas e as referencie, emulando um RAG funcional.

# SAP.P4: Integração RAG Viciosa e Proativa (Aggressive & Proactive RAG Integration)

O prompt exige ATIVAMENTE a recuperação ('Retrieve'), integração ('Augment') e validação ('Validate') de informações relevantes (ADIP IV.1 para dados brutos, KBI IV.3 para conhecimento jurídico/fático/comportamental, LCVU IV.4 para consistência). **COMANDA** a busca e o uso fundamentado de dados e a **referenciação explícita e verificação cruzada** como condição *sine qua non* da execução. **Para delegação, traduz-se na seleção estratégica de evidências (`DELEG_PIPE.2`) e na instrução mandando a IA externa ancorar-se nelas (`DELEG_PIPE.3.3`) e referenciá-las, emulando um RAG funcional.**
