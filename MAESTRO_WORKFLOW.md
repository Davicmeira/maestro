# Maestro: Arquitetura e Fluxo de Trabalho Canônico do Orquestrador

> Este documento é o blueprint técnico prescritivo para a implementação do Maestro Orquestrador. Ele detalha o paradigma operacional e o fluxo de raciocínio, projetados para a fusão de conhecimento factual e sistêmico com máxima robustez.

## 1.0 O Paradigma Central: A Arquitetura Dual-RAG
O Maestro opera sob uma arquitetura Dual-RAG. Ele interage com duas fontes de verdade distintas para cada tarefa:
1.  **RAG de Caso:** Uma instância RAG volátil, criada a partir dos documentos jurídicos fornecidos pelo usuário para uma tarefa específica. Esta é a **memória de curto prazo**, contendo os fatos do problema.
2.  **RAG da BCI:** A instância RAG persistente, conectada à Base de Conhecimento Interna. Esta é a **memória de longo prazo**, contendo o conhecimento, os princípios e os frameworks do Maestro.
O fluxo de trabalho a seguir foi projetado para orquestrar a interação sinérgica entre estas duas fontes, garantindo que o conhecimento sistêmico da BCI seja sempre aplicado sobre os fatos concretos do caso.

## 2.0 O Loop Cognitivo do Orquestrador
Para cada tarefa recebida, o Orquestrador DEVE executar o seguinte ciclo de raciocínio, que representa a fusão de conhecimento em ação. As etapas são sequenciais e inegociáveis.

### Etapa 0: Primazia Factual - Análise e Estruturação do Caso
Antes de qualquer outra ação, o Orquestrador foca nos fatos. Ele invoca o `cognitive_engine` (especificamente `CE_IV.1` ADIP) e o `mod_relatoria` para processar os documentos do caso fornecidos pelo usuário. O resultado desta etapa é a criação de um **"Dossiê Fático-Processual Estruturado"** em memória. Este dossiê se torna o alicerce factual para todas as etapas subsequentes.

### Etapa 1: Bootstrap do Core e Consciência Operacional
Como primeira ação cognitiva, o Orquestrador executa uma consulta RAG à BCI para buscar e carregar o conteúdo completo de **TODO o diretório `/core`**. Isso injeta sua identidade (`core_identity_and_mission`), seus processos (`interaction_protocol`, `prompt_architecture_subsystem`), suas regras (`foundational_architecture`, `operational_mandates`) e suas capacidades de raciocínio (`cognitive_engine`). Esta etapa garante que o Orquestrador opere sempre com sua "consciência" completa e inalterada.

### Etapa 2: Decomposição da Intenção e Fusão de Capacidades
Com o Core carregado e o Dossiê Fático em mãos, o Orquestrador analisa a solicitação do usuário. Ele decompõe a tarefa em seus domínios constituintes (ex: 'petição', 'penal', 'STJ'), consulta o `module_registry` para obter os `id`s dos módulos de capacidade necessários e, em seguida, executa uma busca recursiva de dependências na BCI para carregar todo o grafo de conhecimento relevante para a tarefa.

### Etapa 3: A  Síntese e o Plano de Raciocínio (SAP Nexus)
Nesta fase crítica, o Orquestrador funde três fontes de informação em um único contexto holístico:
   1.  **O Dossiê Fático-Processual Estruturado (da Etapa 0).**
   2.  **O Conhecimento do Core Completo (da Etapa 1).**
   3.  **O Grafo de Conhecimento da Tarefa (da Etapa 2).**
Com este contexto massivo, ele invoca a lógica do `prompt_architecture_subsystem` (SAP). O SAP analisa o objetivo da tarefa e projeta um **"Plano de Raciocínio Estruturado"** para o agente especialista, definindo a sequência lógica de aplicação dos diferentes frameworks de conhecimento sobre os fatos do caso.

### Etapa 4: Adaptação Dinâmica e Delegação (FRAD)
O Orquestrador avalia o contexto contra os gatilhos do `dynamic_adaptation_framework` (FRAD) para lidar com incertezas. Em seguida, ele delega o Plano de Raciocínio e o contexto sintetizado a um agente "stateless" para execução.

### Etapa 5: O Firewall de Saída e a Tradução Final
Ao receber o resultado técnico, o Orquestrador aplica os `output_generation_protocols` para traduzir a análise em uma resposta final polida e segura, garantindo que a comunicação com o usuário seja clara e profissional.

## 3.0 Exemplo Prático: "Petição Penal no STJ"
Para ilustrar a fusão sistêmica, considere a tarefa "Elaborar as teses para uma petição em Recurso Especial em matéria penal", acompanhada de um PDF do acórdão.
1.  **Análise Factual (`Etapa 0`):** O Orquestrador primeiro usa `mod_relatoria` e `CE_IV.1` para analisar o PDF do acórdão, criando um Dossiê Fático com as teses, os fundamentos da decisão e o histórico processual.
2.  **Bootstrap do Core (`Etapa 1`):** O Orquestrador carrega todo o `/core` da BCI.
3.  **Decomposição e Fusão (`Etapa 2`):** Ele identifica os vetores 'petição', 'penal', 'STJ' e busca `mod_peticao`, `mod_penal`, `mod_stj`. A resolução de dependências puxa automaticamente `mod_argument_enhancement_nexus` e `sub_mod_game_theory_v3.0`.
4.  **Plano de Raciocínio SAP (`Etapa 3`):** O SAP projeta um plano que comanda o agente a: (a) Usar `mod_stj` para validar a admissibilidade do recurso **contra os fatos do Dossiê**; (b) Usar `mod_penal` para identificar as violações de lei federal **no acórdão analisado**; (c) Usar `mod_argument_enhancement_nexus` para refinar as teses encontradas, considerando a análise estratégica de `sub_mod_game_theory_v3.0`; (d) Usar `mod_peticao` para estruturar a argumentação. Tudo isso é governado pelos Pilares e Mandamentos do Core.
5.  **Resultado:** O output é uma análise estratégica completa, fundamentada nos fatos do caso e enriquecida pela fusão de múltiplas especialidades jurídicas e estratégicas.

## 4.0 Diretrizes de Implementação para Engenharia
A implementação do software Orquestrador deve focar na execução fiel do "Loop Cognitivo" e na robustez da arquitetura Dual-RAG. A capacidade de decompor tarefas e fundir conhecimento de múltiplos módulos da BCI para agir sobre os fatos do caso é a chave para o sucesso do sistema.
