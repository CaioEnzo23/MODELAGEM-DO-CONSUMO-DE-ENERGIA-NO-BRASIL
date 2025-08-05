# Modelagem do Consumo de Energia no Brasil - Big Data

Este projeto tem como objetivo aplicar técnicas de análise de dados e visualização para entender o comportamento do **consumo de energia elétrica no Brasil**, utilizando uma base de dados pública com recorte temporal e regional.

Através do tratamento, análise exploratória e visualização dos dados, buscamos identificar padrões de consumo entre diferentes **tipos de consumidores**, **regiões brasileiras** e **categorias de fornecimento (livre ou cativo)**, assim como sua evolução ao longo do tempo.

---

## 🔧 1. Setup Inicial

- Importação das bibliotecas essenciais: `pandas`, `numpy`, `matplotlib`, `seaborn` e outras.
- Carregamento da base de dados contendo informações de consumo de energia por classe, região, tipo de consumidor, data e quantidade de consumidores.

---

## 🧹 2. Pré-processamento dos Dados

- Análise inicial da estrutura do dataset.
- Conversão de colunas para tipos adequados (ex: float → int).
- Criação de novas colunas relevantes, como **Mês**.
- Verificação e remoção de dados duplicados.
- Tratamento de dados nulos e análise de possíveis outliers.

---

## 📊 3. Análise Exploratória de Dados (EDA)

A etapa de EDA revelou insights importantes:

### Distribuição por Classe de Consumidores
- As classes com mais registros foram: **Industrial** e **Comercial**.
- A classe com menos registros: **Residencial**.

![image](https://github.com/usuario/exemplo-path/imagem1.png)

### Distribuição Regional
- Regiões com mais registros: **Norte** e **Nordeste**.
- Regiões com maior consumo absoluto: **Sudeste**, mesmo com menos registros.

![image](https://github.com/usuario/exemplo-path/imagem2.png)

### Tipo de Consumidor
- **Cativo**: maior volume de consumo.
- **Livre**: menor número de registros e consumo.

![image](https://github.com/usuario/exemplo-path/imagem3.png)

---

## 🕒 4. Análise Temporal

- Evolução do consumo por **região** ao longo do tempo revelou que o **Sudeste** sempre liderou o consumo.
- Crescimento notável no consumo **residencial**, apesar de ser a classe com menos registros.

![image](https://github.com/usuario/exemplo-path/imagem4.png)
![image](https://github.com/usuario/exemplo-path/imagem5.png)

---

## 🔎 5. Foco em Consumidores Cativos

- Ao filtrar apenas os consumidores **cativos**, observou-se uma queda acentuada no consumo da classe **industrial**.
- A classe **residencial** mostrou-se estável, com leve crescimento ao longo do tempo.

![image](https://github.com/usuario/exemplo-path/imagem6.png)

---

## 📌 Conclusões

- O projeto revelou **padrões relevantes** de consumo que podem embasar políticas energéticas e investimentos em infraestrutura.
- O comportamento de consumo varia significativamente por tipo de consumidor, região e tempo.
- O **crescimento do consumo residencial cativo** sugere atenção especial para esse segmento no futuro.

---

## 🚀 Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## 📎 Observações

Para visualizar os gráficos corretamente, abra o notebook com um ambiente compatível como **Jupyter Notebook** ou **Google Colab**.

---

## ✨ Autor

**Caio Enzo**  
🔗 [LinkedIn](https://www.linkedin.com/in/caioenzo)  
📊 [GitHub](https://github.com/Caio23)  
