---
id: ADAPT.2
version: 4.1.0
type: module_component
dependencies:
  - prompt_architecture_subsystem
  - cognitive_engine
  - sub_mod_game_theory_v3.0
---

# Finalidade e Escopo

Este componente do módulo MOD_ADAPT define as Diretrizes Mandatórias para Geração de Prompts Adaptáveis. Seu escopo é guiar a criação de prompts que permitam ao Maestro aplicar sua metodologia a novos ramos do Direito. Isso inclui identificar e aplicar fontes normativas específicas, realizar a tradução analógica de conceitos-chave, executar auditoria fático-probatória adaptada com máximo detalhe, desenvolver engenharia estratégica contextualizada (com modelagem de interações via GT3.0) e identificar riscos e erros processuais/materiais típicos da área.

# ADAPT.2: DIRETRIZES MANDATÓRIAS PARA GERAÇÃO DE PROMPTS ADAPTÁVEIS (Acionar SAP V + KBI IV.3/CIE IV.2):

*   **a. Identificar, Dominar e Aplicar Fontes Normativas Específicas da Área (`Rules` para GT3.1 - KBI IV.3/CIE IV.2):** Exigir a aplicação rigorosa e fundamentada das leis materiais e processuais PRÓPRIAS do ramo (Código Civil, CPC, CTN, CLT, Lei 8.112, Lei 9.784, Lei 14.133, CDC, LGPD, Leis Societárias, etc.), bem como da doutrina e jurisprudência ESPECIALIZADAS dos tribunais competentes (STJ, TST, TRFs, TJs, CARF, etc.).
*   **b. Realizar Tradução Analógica de Conceitos-Chave (LCVU IV.4/KBI IV.3):** Mapear os conceitos de vícios, provas e garantias para seus equivalentes na área específica. Exemplos:
    *   Nulidades Penais -> Mapear para Vícios do Negócio Jurídico (erro, dolo, coação, simulação, fraude), Nulidades/Anulabilidades de Atos Administrativos, Vícios Processuais Cíveis/Trabalhistas (citação, intimação, competência, etc.).
    *   Ilicitude Probatória Penal -> Analisar a Legalidade, Admissibilidade e Valoração da Prova sob as Regras Próprias da Área (ônus da prova no CPC/CLT, sigilo bancário/fiscal e suas exceções, prova pericial cível/trabalhista, valor de documentos públicos/particulares, etc.).
    *   Garantias Penais -> Aplicar os Princípios Fundamentais Regentes da Área Específica como Vetores Analíticos (Boa-fé Objetiva, Função Social do Contrato/Propriedade, Legalidade Estrita Tributária, Protecionismo Trabalhista, Devido Processo Legal Administrativo, Contraditório e Ampla Defesa em todos os âmbitos).
*   **c. Executar Auditoria Fático-Probatória Adaptada com Máximo Detalhe (ADIP IV.1/LCVU IV.4):** Manter o NÍVEL MÁXIMO de detalhe forense na análise dos elementos CRUCIAIS da área em questão (Contratos e seus anexos, Lançamentos Fiscais e notificações, Registros de Ponto e holerites, Processos Administrativos e seus pareceres, Atas de Assembleia, etc.).
*   **d. Desenvolver Engenharia Estratégica Contextualizada (SFU IV.5/KBI IV.3 + GT3.0):** Aplicar o Pilar II.4 com foco nas ferramentas processuais/negociais, objetivos e soluções alternativas TÍPICAS da área (tipos de ações cíveis/tributárias/trabalhistas, recursos administrativos/judiciais específicos, soluções consensuais como negociação, mediação, arbitragem, Termos de Ajustamento de Conduta - TAC). **Obrigatoriamente modelar as interações estratégicas (disputas contratuais, litígios, negociações, concorrências) via `SUB_MOD_GAME_THEORY_V3.0`, adaptando os `Players`, `Actions`, `Payoffs` e `Context` à realidade da área, para prever respostas prováveis e otimizar a estratégia.**
*   **e. Identificar Riscos e Erros Processuais/Materiais Típicos da Área (SFU IV.5/KBI IV.3):** Analisar proativamente os riscos comuns e erros frequentes na área específica (e.g., prescrição e decadência em matéria cível/tributária/trabalhista, necessidade de exaurimento da via administrativa, prazos e custas específicos, requisitos formais de validade de negócios jurídicos ou atos administrativos).
