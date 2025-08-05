# Análise de Consumo de Energia no Brasil

Este projeto tem como objetivo analisar dados de consumo de energia elétrica por região e tipo de consumidor no Brasil, utilizando ferramentas de Big Data e Ciência de Dados.

## 📁 Estrutura do Projeto

O projeto é implementado em um notebook Jupyter, contendo as seguintes etapas:

### 🔧 Setup
- Importação das bibliotecas principais utilizadas (`pandas`, `numpy`, `matplotlib`, `seaborn`, entre outras).
- Carregamento da base de dados para análise.

### 🧹 Pré-processamento dos Dados
- Identificação de colunas, tipos de dados e estatísticas descritivas.
- Verificação de nulos, valores duplicados e inconsistências.
- Conversão de tipos de dados para otimização de performance.
- Criação de nova coluna de mês para análise temporal mais detalhada.

### 📊 Análise Exploratória
- Distribuição dos consumidores por tipo (residencial, industrial, comercial, etc.).
- Distribuição do consumo por região geográfica (Norte, Nordeste, Sul, Sudeste, Centro-Oeste).
- Comparação entre consumidores cativos e livres.
- Análises temporais de consumo por região e por tipo de consumidor.
- Utilização de histogramas, gráficos de barras e outras visualizações.

<img width="1489" height="790" alt="Image" src="https://github.com/user-attachments/assets/226e0999-3769-4bb9-a672-c228caf45641" />

<img width="1189" height="590" alt="Image" src="https://github.com/user-attachments/assets/6516e4ee-c75c-414b-bb1c-ab43054c2121" />

<img width="989" height="590" alt="Image" src="https://github.com/user-attachments/assets/a8a7b4d4-9f9f-4a12-aecc-7dcf5927ae4a" />

## 🧠 Estruturação do Modelo

Após a análise exploratória, foi realizada a modelagem preditiva para estimar o consumo energético com base nos dados históricos.

- As variáveis categóricas foram transformadas em numéricas com `get_dummies`.
- A coluna de data também foi convertida para formato numérico.
- A base foi dividida em variáveis de entrada (`X`) e saída (`Y`) e separada em conjuntos de treino e teste.
- Modelos aplicados:
  - **Random Forest Regressor**
  - **Regressão Linear**
  - **Árvore de Decisão (Decision Tree Regressor)**

## 📈 Construção dos Resultados

Cada modelo foi treinado e avaliado com base no conjunto de teste:

- Avaliação dos modelos feita por métricas como:
  - R² (Coeficiente de Determinação)
  - Erro Médio Absoluto (MAE)
  - Erro Quadrático Médio (MSE)

- Comparação do desempenho entre os modelos mostrou que o **Random Forest** apresentou melhor resultado geral na predição do consumo.

- Além disso, foram geradas previsões e visualizações para validar a performance e aderência dos modelos aos dados reais.

<img width="640" height="251" alt="Image" src="https://github.com/user-attachments/assets/71924210-32fa-4957-97ed-34afc8af39d7" />

<img width="1580" height="525" alt="Image" src="https://github.com/user-attachments/assets/58ffd900-fd0c-4bc2-8709-9934570f3780" />

## 🔍 Principais Descobertas
- As regiões Norte e Nordeste concentram mais registros, mas a região Sudeste lidera em volume total de consumo.
- Houve crescimento no consumo residencial ao longo do tempo.
- Queda no consumo cativo industrial e crescimento correspondente no tipo livre.
- O modelo Random Forest obteve melhor desempenho preditivo.

## 🛠️ Tecnologias Utilizadas
- Python
- Jupyter Notebook
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- NumPy

## 📌 Requisitos
- Python 3.8+
- Ambiente Jupyter Notebook
- Instalar dependências com:
  ```bash
  pip install -r requirements.txt
