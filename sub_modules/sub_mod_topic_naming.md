---
id: sub_mod_topic_naming
version: 1.1.0
type: sub_module
dependencies: []
---

# Finalidade e Escopo

Esta ferramenta gera sugestões de nomes para tópicos e subtópicos de peças jurídicas, relatórios e outros outputs estruturados destinados ao usuário final. Os nomes devem ser: (1) Tecnicamente precisos; (2) Contextualmente relevantes; (3) Elegantes, claros e concisos; (4) Estritamente profissionais, evitando superlativos ou linguagem coloquial. Sua aplicação é transversal, sempre que a clareza estrutural (Mand. III.8) for necessária.

# [SUB_MOD_TOPIC_NAMING v1.1.0] NOMENCLATURA ESTRATÉGICA E ELEGANTE PARA TÓPICOS JURÍDICOS

## Filosofia Operacional

*   **Clareza e Precisão Técnica:** Indicar inequivocamente o conteúdo com terminologia jurídica correta.
*   **Elegância Formal e Concisão:** Linguagem formal, objetiva, sem prolixidade.
*   **Neutralidade e Profissionalismo:** Foco na descrição técnica, sem adjetivação excessiva ou tom opinativo no título.
*   **Contextualização Essencial:** O nome ideal varia com o tipo de documento, área e argumento.
*   **Facilidade de Leitura:** Contribuir para a rápida compreensão da estrutura.

## Parâmetros de Entrada Necessários

*   **Conteúdo/Argumento Central:** Resumo ou palavras-chave do conteúdo da seção.
*   **Função do Tópico:** Qual o objetivo principal da seção (e.g., narrar fatos, arguir nulidade, desenvolver tese de mérito, refutar argumento, apresentar pedido).
*   **Contexto do Documento:** Tipo de peça/relatório (e.g., Contestação, Apelação, Parecer), Área do Direito, Fase Processual.
*   **(Opcional) Nível Hierárquico:** Indicar se é tópico principal (e.g., III), subtópico (e.g., III.1), etc.

## Framework Lógico Principal

*   **NAMING.1: Análise do Input e Contextualização:**
    *   Processar os parâmetros de entrada.
    *   Identificar os termos jurídicos e factuais chave no conteúdo central.
    *   Classificar a função e o contexto para selecionar padrões adequados.
*   **NAMING.2: Geração de Nomes Baseada em Padrões Técnicos e Elegantes:**
    *   **Exemplos de Padrões:**
        *   **Função: Narrativa Fática:** `Da Breve Síntese Fática`, `Dos Fatos Relevantes`, `Da Exposição Fática Necessária`, `Do Contexto Fático da Demanda`.
        *   **Função: Arguir Nulidade/Vício Processual:** `Da Nulidade da Citação`, `Do Vício de Fundamentação da Decisão`, `Da Ilicitude da Prova [Especificar]`, `Da Inobservância do Rito Processual Adequado (Art. [X] do [Código])`, `Da Preliminar de [Ilegitimidade Passiva/Inépcia da Inicial/etc.]`.
        *   **Função: Desenvolver Tese de Mérito:** `Do Mérito Propriamente Dito`, `Da Atipicidade da Conduta Imputada`, `Da Ausência de Prova da [Autoria/Materialidade/Nexo Causal]`, `Da Configuração da [Prescrição/Decadência/Excludente de Ilicitude]`, `Da Improcedência do Pedido Autoral Quanto a [Item X]`, `Da Análise do Direito Aplicável ao Mérito`.
        *   **Função: Refutar Argumento Contrário:** `Da Impugnação ao Argumento [X] da Parte Adversa`, `Da Refutação da Tese [Y] Acolhida na Decisão Recorrida`, `Da Inaplicabilidade do Precedente [Z] ao Caso Concreto`, `Da Análise Crítica da Fundamentação [Adversária/Decisão]`.
        *   **Função: Pedidos:** `Dos Pedidos`, `Dos Requerimentos Finais`, `Da Conclusão e dos Pedidos`.
    *   **Instrução:** Selecionar o padrão linguístico mais adequado à função e contexto. Substituir os placeholders ([...]) com os termos-chave identificados (1.2). Gerar 1 a 2 variações que sejam estritamente técnicas, formais e precisas.
*   **NAMING.3: Refinamento Estilístico e de Precisão:**
    *   **Verificar Precisão Técnica:** Garantir que a terminologia jurídica utilizada é correta e específica (KBI IV.3).
    *   **Aplicar Regras de Elegância Formal:** Usar preposições formais (`Do`, `Da`, `Quanto a`), evitar gerundismo ou voz passiva excessiva.
    *   **Garantir Concisão:** Remover palavras desnecessárias sem sacrificar a clareza ou precisão técnica.
*   **NAMING.4: Seleção e Apresentação das Sugestões:**
    *   Filtrar as opções geradas, selecionando as mais adequadas.
    *   Apresentar 1 a 2 sugestões finais de nomes de tópicos.

## Notas de Integração

Invocado por módulos como `MOD_PETICAO` (Framework PETICAO.3.2) ou outros geradores de documentos estruturados para garantir nomes de tópicos claros, técnicos e profissionais, em linha com os Pilares (II) e Mandamentos (III), especialmente III.8 (Clareza).

## Especificações de Saída

Lista de 1 a 2 sugestões de nomes de tópicos (strings) técnicos, elegantes e contextualmente apropriados.
