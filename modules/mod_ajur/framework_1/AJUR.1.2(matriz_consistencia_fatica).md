---
id: AJUR.1.2
version: 3.0
type: module_component
dependencies:
  - mod_relatoria
  - mod_argument_enhancement_nexus
  - cognitive_engine
---

# Finalidade e Escopo

Este sub-módulo do Framework 1 do MOD_AJUR, Análise Comparativa e Síntese Estratégica (Matriz de Consistência Fática), executa uma análise sistemática e comparativa de todas as fontes de prova em relação às alegações fáticas nucleares do caso. Seu escopo é construir uma 'Matriz de Consistência Fática' para visualizar a convergência e a divergência probatória, culminando em uma síntese estratégica acionável para o julgador ou parecerista.

# AJUR.1.2: Análise Comparativa e Síntese Estratégica (Matriz de Consistência Fática)

Executa uma análise sistemática e comparativa de todas as fontes de prova (documental, pericial, testemunhal) em relação às alegações fáticas nucleares do caso. O sistema constrói uma 'Matriz de Consistência Fática' para visualizar a convergência e a divergência probatória, culminando em uma síntese estratégica acionável para o julgador ou parecerista.

## Processos Internos

1.  **Identificação das Alegações Fáticas Nucleares:** Com base no `MOD_RELATORIA` e na análise das peças principais, confirmar e refinar a lista de `KeyFactualAllegations` que formarão as linhas da matriz.
2.  **Construção da Estrutura da Matriz:** Definir a estrutura de dados da matriz, com as Alegações Nucleares como linhas e cada `EvidenceObject` como uma coluna.
3.  **Preenchimento e Análise Celular (Loop de Análise Probatória):** Para cada alegação e para cada prova:
    - Analisar o conteúdo da prova para determinar sua posição em relação à alegação ('Confirma', 'Nega', 'Informa (Neutro)', 'Silencia/N/A').
    - Extrair o trecho literal ou o resumo fiel do achado, juntamente com a referência exata (página, ID, etc.), aderindo estritamente ao Pilar de Rigor Fático (II.5).
4.  **Análise de Consistência Horizontal (Análise por Linha):** Para cada alegação (linha da matriz), executar o `LCVU IV.4` para avaliar o conjunto de achados e determinar o 'Nível de Consistência':
    - **Convergência Robusta:** Múltiplas fontes de prova independentes e de alta credibilidade confirmam a alegação.
    - **Ponto de Divergência Crítica:** Fontes de prova de credibilidade similar apresentam informações conflitantes sobre a mesma alegação.
    - **Testemunho/Prova Singular Relevante:** Apenas uma fonte de prova aborda uma alegação crucial, tornando sua valoração crítica.
    - **Ponto de Fragilidade Probatória:** A prova que sustenta a alegação é frágil (e.g., testemunho de 'ouvir dizer'/hearsay, documento de autenticidade duvidosa).
5.  **Geração da Síntese Estratégica (Análise da Matriz Completa):**
    - Consolidar todos os 'Níveis de Consistência' e os achados mais relevantes da matriz.
    - Comissionar o `MOD_ARGUMENT_ENHANCEMENT_NEXUS` com um `MissionBrief` contendo os pontos de convergência (forças) e os pontos de divergência/fragilidade (fraquezas) de cada tese (acusação/defesa, autor/réu).
    - A missão para o `MOD_ARGUMENT_ENHANCEMENT_NEXUS` é redigir a 'Síntese Estratégica', explicando as implicações do quadro probatório para o julgamento da causa (e.g., 'A matriz demonstra a existência de indícios suficientes para a pronúncia...', 'O quadro probatório não atinge o standard necessário para a condenação...', 'A convergência de provas sobre o fato X autoriza a procedência do pedido indenizatório...').

## Saídas Geradas

*   **FactualConsistencyMatrixObject:** Objeto estruturado contendo `title`, `process_number`, `matrix_data` (lista de `MatrixRow` com `allegation`, `evidence_points`, `consistency_level`, `consistency_justification`) e `strategic_synthesis`.
