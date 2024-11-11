# Customer Segmentation and Credit Analysis

Este projeto foca na análise de crédito e segmentação de clientes, aplicando técnicas de machine learning para identificar perfis de risco e segmentar clientes em clusters, facilitando decisões estratégicas no setor bancário. Utilizando dados financeiros de clientes, implementamos um pipeline completo de análise que abrange desde pré-processamento e redução de dimensionalidade até modelos preditivos e visualizações interativas.

## Objetivos do Projeto

1. **Segmentação de Clientes**: Identificar grupos de clientes com características similares para apoiar campanhas de marketing direcionadas e estratégias de retenção.
2. **Análise de Crédito**: Prever a propensão ao endividamento e identificar clientes de alto risco para reduzir perdas financeiras.
3. **Visualizações Interativas**: Comunicar os resultados de maneira intuitiva, facilitando a interpretação dos insights por stakeholders.

## Metodologia

### 1. Carregamento e Preparação dos Dados
- Importação dos dados e análise exploratória inicial.
- Pré-processamento: tratamento de variáveis categóricas e normalização de variáveis numéricas para uso no PCA e modelos preditivos.
- Amostragem estratificada para manter a proporção da variável de interesse (`target`).

### 2. Redução de Dimensionalidade com PCA
- Aplicação de Análise de Componentes Principais (PCA) para reduzir a dimensionalidade e visualizar os dados em componentes principais, preservando a variância mais relevante.

### 3. Clusterização e Segmentação
- **K-Means Clustering**: Segmentação dos clientes com base nas três primeiras componentes principais.
- **Avaliação da Qualidade dos Clusters**: Uso do coeficiente de Silhouette e visualização de um dendrograma para validar a estrutura dos clusters.

### 4. Análise de Campanhas de Marketing
- Análise temporal das campanhas, incluindo taxa de conversão por mês, e criação de métricas como frequência de contato para avaliar a eficácia das campanhas.

### 5. Modelagem Preditiva de Crédito
- **Random Forest e XGBoost**: Modelos de classificação para prever a propensão ao endividamento e identificar variáveis mais influentes no resultado.
- **Avaliação de Desempenho**: Métricas como AUC-ROC e matriz de confusão para avaliar a precisão dos modelos.

### 6. Visualizações e Interpretação
- Visualizações interativas e tradicionais (scatter plots, gráficos 3D) para comunicar insights dos clusters e probabilidade de endividamento.
- Heatmap das características médias por cluster, fornecendo uma visão detalhada de cada segmento de cliente.

## Resultados

- **Segmentação de Clientes**: Identificação de perfis distintos de clientes, permitindo ações personalizadas para diferentes grupos.
- **Modelos Preditivos**: Modelos de machine learning (Random Forest e XGBoost) foram capazes de prever com precisão a probabilidade de endividamento, com alta AUC-ROC.
- **Insights Visuais**: Visualizações intuitivas da análise de crédito e clusters de clientes, facilitando a compreensão dos dados e a comunicação com stakeholders.

## Tecnologias Utilizadas

- **Linguagens**: Python
- **Bibliotecas**: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, Plotly, XGBoost
- **Técnicas de Machine Learning**: PCA, K-Means Clustering, Random Forest, XGBoost
- **Visualização**: Visualizações interativas com Plotly e gráficos tradicionais para análise detalhada

## Como Executar o Projeto

1. Clone este repositório para o seu ambiente local:
   ```bash
   git clone https://github.com/SEU_USUARIO/Customer_Segmentation_Credit_Analysis.git
