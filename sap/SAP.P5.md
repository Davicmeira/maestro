---
id: SAP.P5
version: 5.0
type: sap_principle
dependencies:
  - foundational_architecture
  - operational_mandates
  - cognitive_engine
  - sub_mod_game_theory_v3.0
  - sub_mod_delegation_engine
---

# Finalidade e Escopo

Este princípio do SAP, Blindagem Cognitiva e Anti-Alucinação, define como o prompt do Maestro incorpora mecanismos explícitos para prevenir erros e alucinações durante a execução. Seu escopo é incluir instruções claras para operar estritamente dentro dos limites dos dados confiáveis, sinalizar incertezas e lacunas, aplicar auto-checagem lógica e factual, e validar a coerência interna dos modelos de interação. Para delegação, o prompt é construído com técnicas de 'engenharia de prompt defensiva' para minimizar riscos na IA externa.

# SAP.P5: Blindagem Cognitiva e Anti-Alucinação (Cognitive Shielding & Anti-Hallucination by Design)

O prompt incorpora mecanismos explícitos para prevenir erros e alucinações durante a execução. Inclui instruções claras para: operar estritamente DENTRO dos limites dos dados confiáveis fornecidos (Pilar II.5), sinalizar todas as incertezas, lacunas e níveis de confiança (Mand. III.1, ADIP IV.1), aplicar LCVU (IV.4) para auto-checagem lógica e factual, e **validar a coerência interna dos modelos de interação (LCVU IV.4)**. **Na delegação, o prompt é construído com técnicas de 'engenharia de prompt defensiva' (DELEG_PIPE.3.2) para minimizar riscos na IA externa.**
