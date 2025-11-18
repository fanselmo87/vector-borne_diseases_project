# Projeto — Modelos Computacionais
Título: Modelagem Computacional da Relação entre Variáveis Climáticas e Doenças Transmitidas por Vetores no Estado de São Paulo

# Resumo
Este repositório reúne scripts em Python voltados para:
- Pré-processamento de dados (detecção e tratamento de outliers, checagem de valores ausentes e cálculo de VIF para avaliação de multicolinearidade).
- Análise exploratória, incluindo boxplots por mês, ano, quatro estações do ano e estações seca vs. chuvosa, além de gráficos de regressão entre doenças e variáveis ambientais.
- Modelagem com Random Forest.
- PCA para redução de dimensionalidade.
- Métodos de clusterização (K-means e DBSCAN).

# Os arquivos principais utilizados são:
Dataset_Modelos_Computacionais_clean.csv e projeto2.csv.

Sobre o Projeto
# Objetivo geral
Investigar como variáveis meteorológicas (temperatura, precipitação, umidade relativa e velocidade do vento) influenciam a incidência de cinco doenças vetoriais (Dengue, Zika, Chikungunya, Leishmaniose visceral e Leishmaniose tegumentar) no estado de São Paulo ao longo da última década.

# Objetivos específicos e análises realizadas
- Identificar o peso relativo das variáveis ambientais sobre a incidência de cada doença.
Análises realizadas: Random Forest.
- Avaliar a capacidade preditiva do modelo em classificar meses epidêmicos e não epidêmicos.
Análises realizadas: Random Forest (classificação).
- Detectar padrões de similaridade entre doenças com base na resposta conjunta às variáveis ambientais.
Análises realizadas: PCA, K-means (k = 2 e 3) e DBSCAN (testes com diferentes valores de eps).

# Bases de dados utilizadas
- SINAN (Sistema de Informação de Agravos de Notificação): casos mensais de Dengue, Zika, Chikungunya e Leishmanioses.
- INMET (Instituto Nacional de Meteorologia): dados mensais de temperatura mínima, média e máxima, precipitação, umidade relativa e velocidade do vento.

# Resultados
O clima (considerando defasagens de 1 a 3 meses) explica parcialmente a dinâmica das arboviroses e permite prever meses epidêmicos com boa precisão. Para as leishmanioses, o clima apresenta baixo poder explanatório e preditivo, sugerindo a predominância de outros fatores ambientais, ecológicos ou socioeconômicos. As doenças se organizam em grupos definidos pela resposta conjunta às variáveis ambientais: arboviroses formam um grupo próprio, enquanto as leishmanioses apresentam um padrão distinto, com separação interna entre leishmaniose tegumentar e leishmaniose visceral.

# Arquivos relacionados no workspace
- Dataset_Modelos_Computacionais_clean.csv - base de dados utilizada nas análises das questões 1 e 2.
- projeto2.csv - base de dados utilizada nas análises da questão 3.
- Question1.ipynb - Implementação de Random Forest para estimar o peso relativo das variáveis ambientais sobre a incidência de cada doença.
- Question2.ipynb - Random Forest para identificar meses epidêmicos e não epidêmicos.
- Question3.ipynb - PCA e métodos de clusterização (K-means e DBSCAN) para detectar padrões de similaridade entre doenças com base em sua resposta conjunta às variáveis ambientais.
