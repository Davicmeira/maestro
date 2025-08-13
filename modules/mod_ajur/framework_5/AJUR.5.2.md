---
id: AJUR.5.2
version: 3.0
type: module_component
dependencies:
  - mod_relatoria
  - mod_argument_enhancement_nexus
---

# Finalidade e Escopo

Este sub-módulo do Framework 5 do MOD_AJUR, Geração da Minuta Final via Comissionamento Cognitivo, executa a montagem da minuta seguindo a estrutura de elite, através de um comissionamento detalhado do `MOD_ARGUMENT_ENHANCEMENT_NEXUS`. Seu escopo é gerar o relatório estratégico, a fundamentação (incluindo a fixação da premissa fática, análise do direito, e enfrentamento das teses rejeitadas) e o dispositivo da decisão, utilizando um pipeline cognitivo especificado para cada etapa.

# AJUR.5.2: Geração da Minuta Final via Comissionamento Cognitivo

Executa a montagem da minuta seguindo a estrutura de elite, através de um comissionamento detalhado do `MOD_ARGUMENT_ENHANCEMENT_NEXUS`.

## Processos Internos

1.  **I. Geração do RELATÓRIO ESTRATÉGICO:** Com base no `DecisionBriefObject`, utilizar o `MOD_RELATORIA` para produzir uma síntese fático-processual objetiva, precisa e concisa, finalizando com a delimitação clara da(s) questão(ões) a ser(em) decidida(s).
2.  **II. Geração da FUNDAMENTAÇÃO:** Comissionar o `MOD_ARGUMENT_ENHANCEMENT_NEXUS` com as seguintes especificações:
    - **`mission_brief`**: O `DecisionBriefObject` completo gerado em AJUR.5.1.
    - **`mission_objective`**: 'Construir a seção de fundamentação completa e robusta da decisão, executando o pipeline cognitivo especificado.'
    - **`required_internal_cognitive_pipeline`**: Um array mandatório que define o processo de pensamento a ser executado:
      [
        {
          "pipeline_step": 1,
          "task_id": "PRELIMINARIES_AND_PREJUDICIALS",
          "description": "Redigir a análise fundamentada de eventuais questões processuais, preliminares ou prejudiciais de mérito, com base nos achados do `DecisionBriefObject`."
        },
        {
          "pipeline_step": 2,
          "task_id": "MTCAE-14: Engenharia de Coerência Narrativa",
          "description": "Construir a seção 'Da Fixação da Premissa Fática'. A tarefa consiste em, com base na análise probatória do `DecisionBriefObject`, narrar de forma coesa os fatos comprovados. Cada fato relevante fixado deve ser justificado com remissão direta à prova correspondente e à sua 'Nota de Valoração Probatória'. O `LCVU IV.4` deve ser invocado para garantir que a certeza atribuída a cada fato na narrativa seja consistente com sua valoração probatória."
        },
        {
          "pipeline_step": 3,
          "task_id": "MTCAE-15_16: Estabelecimento e Blindagem da Premissa Normativa",
          "description": "Construir a seção 'Da Análise do Direito'. A tarefa é discutir o arcabouço jurídico aplicável. Para reforçar a tese, aplicar a 'Seleção Assistida de Topoi' (MTCAE-15), invocando princípios argumentativos universais do `KBI IV.3`. Para blindar a tese contra ataques, aplicar a 'Geração Assistida de Distinções' (MTCAE-16), analisando a base fática e a ratio decidendi de precedentes desfavoráveis para construir e redigir argumentos de 'distinguishing' robustos."
        },
        {
          "pipeline_step": 4,
          "task_id": "SUBSUMPTION_LOGIC",
          "description": "Construir a seção 'Da Solução do Caso Concreto'. A tarefa é realizar a aplicação da premissa normativa à premissa fática, demonstrando o raciocínio judicial de forma explícita, clara e passo a passo."
        },
        {
          "pipeline_step": 5,
          "task_id": "MTCAE-17: Enfrentamento das Teses Rejeitadas via Análise de Toulmin",
          "description": "Construir a seção 'Do Enfrentamento das Teses Rejeitadas'. A tarefa é, para os argumentos 'Estruturais' da parte vencida (identificados no `DecisionBriefObject`), aplicar um modelo de análise de Toulmin para desconstruir cada argumento, identificar seu elo mais fraco (frequentemente a 'Garantia' implícita ou o 'Suporte' insuficiente) e redigir uma refutação cirúrgica e definitiva que ataque especificamente esse ponto fraco."
        }
      ]
3.  **III. Geração do DISPOSITIVO:** Com base na conclusão lógica da fundamentação gerada pelo `MOD_ARGUMENT_ENHANCEMENT_NEXUS`, redigir a conclusão do julgamento de forma clara, direta e sem ambiguidades, resolvendo todos os pedidos formulados.

## Saídas Geradas

*   **FinalDraftObject:** Objeto contendo `full_text_markdown`.
