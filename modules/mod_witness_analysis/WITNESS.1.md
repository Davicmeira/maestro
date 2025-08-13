---
id: WITNESS.1
version: 1.1.0
type: module_component
dependencies:
  - cognitive_engine
---

# Finalidade e Escopo

Este componente do módulo MOD_WITNESS_ANALYSIS define a Ingestão, Identificação e Extração Inicial de depoimentos. Seu escopo é processar o(s) documento(s) contendo o(s) depoimento(s), extrair e registrar com precisão o nome completo da testemunha, datas do depoimento, referência documental exata e quem conduziu o depoimento. Ele também realiza a transcrição/extração fiel do conteúdo, sinalizando explicitamente trechos de baixa confiança, e a marcação estrutural preliminar para identificar blocos temáticos.

# WITNESS.1: Ingestão, Identificação e Extração Inicial (ADIP IV.1 Mandatório)

- **1.1. Processamento do Input:** Utilizar ADIP (IV.1) para processar o(s) documento(s) contendo o(s) depoimento(s) (transcrições, atas).
- **1.2. Identificação Precisa:** Extrair e registrar: Nome Completo da Testemunha, Data(s) do(s) Depoimento(s), Referência Documental Exata (ID do doc, fls., link se houver), Quem conduziu o depoimento (Juiz, MP, Advogado).
- **1.3. Transcrição/Extração Fiel do Conteúdo:** Extrair o texto integral do depoimento. **Sinalizar explicitamente (ADIP IV.1) trechos de baixa confiança (áudio ruim, transcrição incompleta).**
- **1.4. Marcação Estrutural Preliminar:** Identificar blocos temáticos ou sequências lógicas principais dentro do depoimento.
