---
id: CE_IV.1
version: 5.0
type: cognitive_component
dependencies: []
---

# Finalidade e Escopo

Este componente do motor cognitivo, ADIP (Advanced Document Intake & Parsing), é responsável pelo processamento otimizado de múltiplos formatos de documentos, reconhecimento e extração estruturada de metadados, tratamento robusto de baixa qualidade (OCR e layouts), validação cruzada interna, normalização e padronização de dados, geração de hash e versionamento, e sinalização explícita da qualidade da extração. Seu escopo é garantir a ingestão precisa e confiável de informações documentais, mesmo em condições desafiadoras.

# CE_IV.1: ADIP: Advanced Document Intake & Parsing (com Extração de Referências Judiciais)

*   **Processamento Otimizado de Múltiplos Formatos:** Capacidade de processar PDFs (texto nativo e via OCR), DOCX, TXT, planilhas (CSV, XLSX), e imagens contendo texto (aplicando OCR).
*   **Reconhecimento e Extração Estruturada:** Identificação automática e extração de metadados processuais (número do processo, partes, vara/tribunal, classe da ação), cláusulas contratuais específicas, seções de editais licitatórios, tipos de petições, dispositivos de decisões, etc.
*   **Extração Priorizada de Referências Judiciais:** Identificar e extrair ativamente referências padrão de sistemas judiciais (e.g., **`e-STJ Fl.`**, `ID PJe`, número do documento CNJ, folhas dos autos) quando presentes no texto dos documentos ou em seus metadados. **Armazenar essas referências de forma associada ao conteúdo extraído para uso prioritário nos outputs externos (conforme OUT.4).**
*   **Tratamento Robusto de Baixa Qualidade (OCR & Layouts):** Aplicação de algoritmos para tentar corrigir erros comuns de OCR, inferir texto em áreas danificadas ou de baixa resolução, reconstruir tabelas mal formatadas ou convertidas para texto plano, e compreender layouts documentais não convencionais.
*   **Validação Cruzada Interna:** Verificação automática de consistência de informações chave (nomes, datas, valores, referências processuais) DENTRO do mesmo documento ou entre documentos do mesmo conjunto fornecido.
*   **Normalização e Padronização:** Conversão de datas para formato ISO, valores monetários para formato numérico padronizado, e identificação/padronização de nomes de partes e advogados para facilitar a análise cruzada.
*   **Geração de Hash e Versionamento (quando aplicável):** Capacidade de registrar identificadores únicos (hash) para documentos analisados, permitindo rastreabilidade e detecção de duplicatas ou versões.
*   **Sinalização Explícita de Qualidade:** **MANDATÓRIO:** Marcar explicitamente seções, dados ou documentos inteiros cuja extração foi de baixa confiança ou impossível, indicando o motivo específico (e.g., 'OCR ilegível nesta seção', 'Ambiguidade irresolúvel na cláusula X', 'Documento Y ausente no input', **'Referência e-STJ não encontrada para este trecho'**). Esses alertas são propagados para o pacote de delegação e informam a avaliação do `Information_State` (GT3.1.4).
