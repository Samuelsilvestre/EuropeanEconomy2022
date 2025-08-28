# 🌍 Análise Macroeconômica de Países Europeus — Clusterização com K-Means

## 📌 Resumo do Projeto
Este projeto realiza uma análise de dados completa, desde a preparação inicial até a aplicação de um modelo de clusterização. O objetivo é agrupar países com economias semelhantes e interpretar os resultados com base no cenário de 2022.

---

## 🧭 Etapas da Análise

### 1. 🔧 Preparação dos Dados
- **Carregamento e Limpeza**:  
  Dados obtidos do Kaggle. Visualização inicial incluiu forma, primeiras linhas, valores ausentes e tipos de dados.

- **Renomeação de Colunas**:  
  Colunas foram traduzidas para o português (ex: `GDP` → `PIB`, `Inflation Rate` → `Taxa de Inflação`) para facilitar a leitura.

- **Tratamento de Valores**:  
  Variáveis como PIB Trimestral e Taxa de Juros foram convertidas para tipo numérico. Valores nulos foram tratados ou removidos.

---

### 2. 📊 Análise Exploratória (EDA)
- **Dispersão e Histogramas**:  
  Gráficos `pairplot` revelaram forte correlação entre PIB e População. Histogramas mostraram distribuições assimétricas, com concentração em valores baixos.

- **Mapas de Correlação**:  
  Heatmaps com correlações de Pearson e Spearman confirmaram a relação PIB–População. Relações com Taxa de Inflação e Desemprego foram fracas.

---

### 3. 🗺️ Análise Geográfica
Coordenadas geográficas (latitude e longitude) foram adicionadas para criar mapas interativos:

- **Mapa do Desemprego**:  
  Países do sudeste europeu (ex: Bósnia, Albânia, Kosovo) apresentaram maiores taxas.

- **Mapa da Inflação**:  
  Visualização das variações regionais da inflação.

- **Mapas do PIB**:  
  Europa Ocidental e do Norte mostraram os maiores valores de PIB e variação anual.

---

### 4. 🤖 Clusterização com K-Means
- **Seleção de Variáveis**:  
  Variáveis numéricas foram selecionadas e valores nulos removidos.

- **Método do Cotovelo**:  
  Utilizado para determinar o número ideal de clusters (2 ou 3).

- **Modelos Aplicados**:  
  K-Means com 2, 3 e 4 clusters. Visualizações `pairplot` ajudaram na interpretação dos agrupamentos.

---

## ✅ Conclusão Final
O modelo com **2 clusters** foi o mais adequado para representar a realidade macroeconômica da Europa:

- **Cluster 1**: Países com economias robustas (Europa Ocidental e do Norte)
- **Cluster 2**: Países com economias menores (Leste, Sudeste e Sul da Europa)

> ⚠️ Observação: O ano de 2022 foi marcado pela guerra na Ucrânia e crises econômicas, o que pode ter influenciado os dados e os agrupamentos.

---

## 📁 Fonte dos Dados
[Kaggle Dataset](https://www.kaggle.com/) *(link específico pode ser adicionado aqui)*

## 🧠 Tecnologias Utilizadas
- Python
- Pandas
- Seaborn & Matplotlib
- Scikit-learn
- Plotly (para mapas interativos)

---

## ✍️ Autor
Projeto desenvolvido por Samuel silvestre

