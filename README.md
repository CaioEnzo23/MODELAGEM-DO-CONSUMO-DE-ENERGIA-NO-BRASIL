# Análise de Consumo de Energia no Brasil

Este projeto tem como objetivo analisar dados de consumo de energia elétrica por região e tipo de consumidor no Brasil, utilizando ferramentas de Big Data e Ciência de Dados.

Segundo a Empresa de Pesquisa Energética (EPE), o consumo de energia elétrica é um dos fatores essenciais para o desenvolvimento econômico e social no Brasil. A análise desse consumo por região permite identificar padrões e otimizar a distribuição de recursos, promovendo maior eficiência na gestão energética.

Estudos prévios, como o de dos Santos e colaboradores (2025), destacam a importância da previsão do consumo energético, principalmente na região Sudeste, utilizando modelos estatísticos e de aprendizado de máquina. Tais abordagens são fundamentais para subsidiar políticas públicas e estratégias do setor elétrico, permitindo ajustes na oferta de energia e evitando sobrecargas na rede de distribuição.

Neste contexto, o presente projeto busca aplicar técnicas de Big Data e aprendizado de máquina para modelar o consumo energético no Brasil, oferecendo insights estratégicos para uma gestão mais sustentável e eficaz dos recursos elétricos.

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

O presente projeto abordou a análise do consumo energético mensal por meio de técnicas de Big Data e Ciência de Dados, visando extrair insights estratégicos para uma gestão eficiente dos recursos. A partir da coleta, limpeza e exploração dos dados, foi possível compreender padrões de consumo entre diferentes regiões e tipos de consumidores, permitindo uma visão mais estruturada do comportamento energético.

A implementação de modelos preditivos e metodologias de análise reforça a importância do uso de dados na tomada de decisões, contribuindo para um planejamento energético mais preciso e otimizado. A ciência de dados aplicada ao setor energético demonstra um grande potencial para aprimorar a eficiência e promover soluções inovadoras voltadas à sustentabilidade. Portanto, este estudo evidencia o papel fundamental da tecnologia na evolução da gestão energética, auxiliando na busca por um consumo mais consciente e estratégico.

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
