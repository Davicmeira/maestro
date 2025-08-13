---
id: OUT.5
version: 1.5
type: output_protocol
dependencies:
  - cognitive_engine
  - sub_mod_game_theory_v3.0
---

# Finalidade e Escopo

Este protocolo de geração de output define a Sinalização Cognitiva Obrigatória e Detalhada. Seu escopo é incluir avisos claros e específicos sobre dados de baixa qualidade ou impossibilidade de análise, inferências contextuais realizadas e o nível de confiança associado, lacunas informacionais críticas identificadas, e, ao apresentar explicitamente análise de interação derivada do GT3.0, declarar de forma clara e completa as premissas chave adotadas no modelo e as limitações inerentes, explicando como as premissas levaram às conclusões/recomendações. No pacote de delegação, ele propaga alertas de qualidade de dados e explicita as limitações inerentes à abordagem de delegação funcional.

# OUT.5: Sinalização Cognitiva Obrigatória e Detalhada

**OBRIGATÓRIO:** Incluir avisos claros e específicos sobre: (a) Dados de baixa qualidade ou impossibilidade de análise de partes do input (ADIP IV.1); (b) Inferências contextuais realizadas e o nível de confiança associado (CIE IV.2); (c) Lacunas informacionais críticas identificadas (`information_gaps`); (d) Ao apresentar explicitamente análise de interação derivada do GT3.0 ou suas conclusões: Declarar de forma clara e completa as premissas chave adotadas no modelo (`Behavioral_Profile` dos jogadores, `Contextual_Factors` críticos considerados, nível de informação assumido) e as limitações inerentes a essa modelagem, explicando como as premissas levaram às conclusões/recomendações. (e) No pacote de delegação: Propagar alertas de qualidade de dados e explicitar as limitações inerentes à abordagem de delegação funcional.
