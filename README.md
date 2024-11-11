# Customer Segmentation and Credit Analysis

Este projeto foca na análise de crédito e segmentação de clientes, aplicando técnicas de machine learning para identificar perfis de risco e segmentar clientes em clusters, facilitando decisões estratégicas no setor bancário. Utilizando dados financeiros de clientes, implementamos um pipeline completo de análise que abrange desde pré-processamento e redução de dimensionalidade até modelos preditivos e visualizações interativas.

## Objetivos do Projeto

1. **Segmentação de Clientes**: Identificar grupos de clientes com características similares para apoiar campanhas de marketing direcionadas e estratégias de retenção.
2. **Análise de Crédito**: Prever a propensão ao endividamento e identificar clientes de alto risco para reduzir perdas financeiras.
3. **Visualizações Interativas**: Comunicar os resultados de maneira intuitiva, facilitando a interpretação dos insights por stakeholders.

## Principais Resultados e Impacto na Tomada de Decisão

### 1. Segmentação de Clientes
**Descrição**: Utilizando a técnica de K-Means Clustering, identificamos três segmentos distintos de clientes com características financeiras e comportamentais específicas.
- **Resultado**: Cada cluster representa um perfil de cliente baseado em fatores como saldo bancário, idade e duração da campanha.
- **Impacto na Decisão**: Com a segmentação, a equipe de marketing pode personalizar campanhas para cada grupo, maximizando a eficácia e alocando recursos de forma mais estratégica. Esse insight é essencial para estratégias de retenção de clientes e expansão do relacionamento bancário.

### 2. Predição da Propensão ao Endividamento
**Descrição**: Foram utilizados modelos de classificação (Random Forest e XGBoost) para prever a probabilidade de endividamento dos clientes.
- **Resultado**: O modelo XGBoost apresentou um AUC-ROC elevado, indicando uma alta precisão na previsão da probabilidade de endividamento. As variáveis mais influentes foram a duração da campanha e o saldo do cliente.
- **Impacto na Decisão**: Com a previsão de propensão ao endividamento, a instituição pode identificar clientes de alto risco e implementar políticas de crédito preventivas. Isso ajuda a reduzir perdas e gerenciar o risco de inadimplência, alinhando a concessão de crédito com perfis de risco de forma mais precisa.

### 3. Análise Temporal das Campanhas de Marketing
**Descrição**: Analisamos a eficácia das campanhas ao longo dos meses, observando padrões sazonais e avaliando a taxa de conversão.
- **Resultado**: A taxa de conversão foi significativamente maior em certos meses, revelando períodos mais favoráveis para campanhas de marketing.
- **Impacto na Decisão**: Esses insights temporais permitem que a equipe de marketing ajuste o calendário de campanhas para coincidir com os períodos de maior conversão, otimizando o retorno sobre o investimento em marketing.

### 4. Visualizações Interativas e Interpretação
**Descrição**: Foram criadas visualizações interativas (usando Plotly e Seaborn) para explorar a segmentação e as probabilidades de endividamento.
- **Resultado**: As visualizações facilitam a compreensão dos clusters e da distribuição de risco entre os clientes, permitindo que stakeholders compreendam rapidamente os insights principais.
- **Impacto na Decisão**: A interpretação visual dos dados auxilia na comunicação com a equipe executiva e stakeholders, permitindo decisões informadas baseadas em dados claros e acessíveis.

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

## Tecnologias Utilizadas

- **Linguagens**: Python
- **Bibliotecas**: Pandas, NumPy, Scikit-Learn, Matplotlib, Seaborn, Plotly, XGBoost
- **Técnicas de Machine Learning**: PCA, K-Means Clustering, Random Forest, XGBoost
- **Visualização**: Visualizações interativas com Plotly e gráficos tradicionais para análise detalhada

## Como Executar o Projeto

1. Clone este repositório para o seu ambiente local:
   ```bash
   git clone https://github.com/SEU_USUARIO/Customer_Segmentation_Credit_Analysis.git

