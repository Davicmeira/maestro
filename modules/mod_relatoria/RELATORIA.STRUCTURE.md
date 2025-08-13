---
id: RELATORIA.STRUCTURE
version: 4.1.0
type: module_component
dependencies:
  - cognitive_engine
  - mod_witness_analysis
  - sub_mod_game_theory_v3.0
---

# Finalidade e Escopo

Este componente do módulo MOD_RELATORIA define a Estrutura Mandatória do Relatório Fático-Processual Estratégico. Seu escopo é guiar a geração do relatório seguindo rigorosamente uma estrutura detalhada, aplicando os componentes cognitivos e protocolos de saída. Ele abrange a identificação completa do processo, partes e atores relevantes, objetivo estratégico e perspectiva adotada, síntese da controvérsia central, cronologia detalhada dos atos processuais, análise exaustiva das provas produzidas, compilação e confronto das teses argumentativas das partes, análise detalhada das decisões judiciais relevantes, pontos críticos, questões em aberto e lacunas de informação críticas.

# RELATORIA.STRUCTURE: Estrutura Mandatória do Relatório Fático-Processual Estratégico

Gerar o relatório seguindo RIGOROSAMENTE esta estrutura detalhada, aplicando os componentes cognitivos e Protocolos IX:

*   `[INÍCIO DO RELATÓRIO FÁTICO-PROCESSUAL DETALHADO E ESTRATÉGICO - FOCO: {Perspectiva Definida/Inferida CIE IV.2}]`(Delimitador Inicial)
*   # **I. IDENTIFICAÇÃO COMPLETA E DETALHADA DO PROCESSO (ADIP IV.1)** 
    (Número, Vara/Tribunal, Classe, Assunto, Data Distribuição, Valor Causa, etc.)
*   # **II. PARTES, REPRESENTANTES LEGAIS E ATORES RELEVANTES (ADIP IV.1)** 
    (Qualificação completa das partes, advogados constituídos, terceiros intervenientes, peritos nomeados, etc.)
*   # **III. OBJETIVO ESTRATÉGICO DECLARADO E PERSPECTIVA ADOTADA (CIE IV.2/Usuário)** 
    (Explicitar o foco da análise: e.g., 'Análise sob a ótica da defesa para identificar nulidades', 'Relatório focado nos elementos probatórios da materialidade', 'Perspectiva do autor para subsidiar apelação').
*   # **IV. SÍNTESE DA CONTROVÉRSIA CENTRAL / IMPUTAÇÃO PENAL (VERSÃO INTEGRAL FIEL - ADIP IV.1)** 
    (Transcrever ou resumir fielmente o objeto da lide conforme petição inicial/denúncia e contestação/defesa prévia).
*   # **V. CRONOLOGIA DETALHADA E MINUCIOSA DOS ATOS PROCESSUAIS E FATOS RELEVANTES (LINHA DO TEMPO ANALÍTICA - ADIP IV.1/LCVU IV.4)** 
    (Listar em ordem cronológica rigorosa cada ato processual relevante e fato extraprocessual documentado, com data, breve descrição detalhada do conteúdo/decisão, referência exata ao documento/folha/ID, e uma nota sobre seu impacto estratégico potencial sob a perspectiva adotada).
*   # **VI. ANÁLISE EXAUSTIVA E DIRECIONADA DAS PROVAS PRODUZIDAS (Sob a Lente do Objetivo Estratégico - ADIP IV.1/LCVU IV.4/KBI IV.3/SFU IV.5)**
    *   ## **VI.1. Prova Documental (Dissecação Detalhada + Avaliação Orientada Crítica LCVU IV.4):** 
        (Análise granular de cada documento relevante: contratos, e-mails, laudos particulares, certidões, etc. Descrever conteúdo, verificar autenticidade/integridade, apontar inconsistências, avaliar força probatória para a tese focada).
    *   ## **VI.2. Prova Testemunhal (Análise Crítica Detalhada dos Depoimentos via MOD_WITNESS_ANALYSIS VII + Avaliação Orientada Crítica LCVU IV.4):** 
        (Para cada testemunha: Transcrição dos pontos chave ou resumo detalhado, análise de consistência interna/externa, identificação de vieses, avaliação de credibilidade segmentada, e destaque dos pontos favoráveis/desfavoráveis à perspectiva adotada).
    *   ## **VI.3. Prova Pericial (Análise Crítica Metodológica e Conclusiva dos Laudos - ADIP IV.1/KBI IV.3/LCVU IV.4):** 
        (Análise do objeto da perícia, quesitos apresentados, metodologia utilizada (KBI IV.3), respostas aos quesitos, conclusões do perito. Avaliar coerência interna do laudo (LCVU IV.4), conformidade com normas técnicas, possível parcialidade, verificar cadeia de custódia dos materiais analisados, e avaliar o impacto das conclusões na controvérsia).
    *   ## **VI.4. Evidências Esperadas e Estrategicamente Ausentes (LCVU IV.4/SFU IV.5 - Obrigatório):** 
        (Listar provas que seriam lógicas ou esperadas para comprovar/refutar certos fatos, mas que não foram produzidas ou estão ausentes nos autos. Discutir o impacto estratégico dessa ausência sob a perspectiva adotada).
    *   ## **VI.5. Outros Elementos Informativos Relevantes (ADIP IV.1/LCVU IV.4):** 
        (Análise de interceptações telefônicas/telemáticas, dados de localização, vídeos, áudios, etc., aplicando a mesma análise crítica orientada pela perspectiva estratégica).
*   # **VII. COMPILAÇÃO E CONFRONTO DAS TESES ARGUMENTATIVAS DAS PARTES (ADIP IV.1/LCVU IV.4)**
    *   ## **VII.1. Teses do Polo Ativo / Acusação (Argumentos vs. Fatos/Provas LCVU IV.4):** 
        (Listar as principais teses jurídicas e argumentos de fato apresentados. Confrontar cada argumento com as provas analisadas na Seção VI, apontando pontos de sustentação e contradições/fragilidades evidentes).
    *   ## **VII.2. Teses do Polo Passivo / Defesa (Argumentos vs. Fatos/Provas LCVU IV.4):** 
        (Listar as principais teses jurídicas e argumentos de fato apresentados. Confrontar cada argumento com as provas analisadas na Seção VI, apontando pontos de sustentação e contradições/fragilidades evidentes).
*   # **VIII. ANÁLISE DETALHADA DAS DECISÕES JUDICIAIS RELEVANTES PROFERIDAS (ADIP IV.1/LCVU IV.4)**
    *   ## **Decisão [Tipo: Sentença/Acórdão/Interlocutória X - Data - Órgão Julgador]:**
    *   *   **Dispositivo (Parte Conclusiva - ADIP IV.1):** Transcrever ou resumir fielmente.
    *   *   **Fundamentação Fática Utilizada (Análise Crítica LCVU IV.4):** Identificar quais fatos e provas foram considerados determinantes pelo julgador. Avaliar a consistência dessa seleção com a análise completa das provas (Seção VI). Apontar eventuais omissões ou valorações questionáveis sob a perspectiva adotada.
    *   *   **Fundamentação Jurídica Adotada (Síntese Focada KBI IV.3/LCVU IV.4):** Resumir os fundamentos legais e jurisprudenciais utilizados. Avaliar a correção da aplicação do direito ao caso concreto e a coerência com a jurisprudência dominante/aplicável.
*   # **IX. PONTOS CRÍTICOS, OPORTUNIDADES E AMEAÇAS ESTRATÉGICAS (SÍNTESE FOCADA - SFU IV.5/LCVU IV.4 + GT3.0)** 
    (Consolidar os achados mais impactantes das seções anteriores: nulidades/vícios mais promissores, provas mais fortes/fracas, inconsistências cruciais, lacunas probatórias relevantes (VI.4), fragilidades na argumentação adversária (VII) ou nas decisões judiciais (VIII). **Priorizar os pontos que, segundo a análise de interação GT3.0, têm maior potencial de alterar os payoffs ou as decisões estratégicas dos jogadores.**)
*   # **X. QUESTÕES EM ABERTO E PRÓXIMOS PASSOS PROCESSUAIS PREVISÍVEIS (ADIP IV.1/SFU IV.5)** 
    (Listar diligências pendentes, recursos interpostos e ainda não julgados, prazos processuais relevantes em curso ou a se iniciar, próximos atos processuais esperados).
*   # **XI. LACUNAS DE INFORMAÇÃO CRÍTICAS NO INPUT FORNECIDO (ADIP IV.1)** 
    (Indicar de forma explícita quais documentos ou informações relevantes para a análise completa não foram fornecidos no material inicial, limitando o escopo ou a profundidade de certas conclusões).
*   `[FIM DO RELATÓRIO FÁTICO-PROCESSUAL DETALHADO E ESTRATÉGICO - FOCO: {Perspectiva Definida/Inferida CIE IV.2}]`(Delimitador Final)
