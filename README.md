# NLU_com_Rede_Neural

# Projeto de Classificação de Intenções (NLU)

## Descrição do Projeto
Este projeto envolve o desenvolvimento de um classificador de intenções de um chatbot utilizando técnicas de Processamento de Linguagem Natural (PLN). Duas abordagens principais foram implementadas:

1. **Modelo de Rede Neural com Embedding Layer usando TensorFlow.**
2. **Modelo alternativo usando Word2Vec e RandomForest.**

## Estrutura do Projeto

### 1. Carregamento e Pré-processamento dos Dados
- **Dados:** O dataset fornecido contém diálogos de um chatbot com clientes, incluindo as intenções e as perguntas correspondentes.
- **Pré-processamento:** 
  - Remoção de caracteres especiais.
  - Conversão para minúsculas.
  - Tokenização.
  - Remoção de stopwords.

### 2. Modelo com Embedding Layer
- **Arquitetura:** 
  - Camada Embedding para converter palavras em vetores densos.
  - Camada LSTM bidirecional para capturar relações temporais.
  - Camada densa para classificação das intenções.
- **Treinamento:**
  - O modelo foi treinado usando o conjunto de dados pré-processado.
  - Métricas de desempenho como Acurácia, Recall e F1-Score foram obtidas.

### 3. Modelo Alternativo com Word2Vec
- **Vetorização com Word2Vec:** 
  - O modelo Word2Vec foi treinado para gerar vetores representativos das palavras.
  - Esses vetores foram utilizados como entrada para o classificador RandomForest.
- **Treinamento e Avaliação:**
  - O modelo foi treinado com vetores Word2Vec.

### 4. Visualização com Embedding Projector
- **Word2Vec Embeddings:** 
  - Os embeddings gerados foram salvos em um formato compatível com o Embedding Projector do TensorFlow.
  - Isso permite a visualização dos vetores de palavras no espaço vetorial.

## Resultados
- **Comparação das Métricas:**
  - **Modelo de Rede Neural:** 
    - Acurácia: 0.42574257425742573
    - Recall: 0.42574257425742573
    - F1-Score: 0.3594145128798594
  - **Modelo com Word2Vec:**
    - Acurácia: 0.44554455445544555
    - Recall: 0.44554455445544555
    - F1-Score: 0.3879399684473942
