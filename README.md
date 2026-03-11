# Análise de Dados de Queimadas no Brasil (2024)

Este projeto contém uma análise exploratória e visualização de dados sobre focos de queimadas no Brasil, com informações atualizadas até o final de 2024. O objetivo principal é extrair insights sobre os estados e municípios mais afetados por meio de ferramentas de análise de dados e geoprocessamento em Python.

## 📂 Estrutura do Repositório

*   **`queimadas.ipynb`**: Um Jupyter Notebook contendo todo o código e análise passo a passo. O código inclui a importação de dados, exploração (describe, info, visualização do início e fim dos dados), conversão para formato geoespacial e a criação de gráficos analíticos (ex: Top 10 estados e cidades com mais queimadas).
*   **`queimadas_resumo.csv`**: Uma amostra/resumo do conjunto de dados original de focos de incêndio (que contém colunas como `lat`, `lon`, `data_hora_gmt`, `estado`, `municipio`, `bioma`, `risco_fogo`, etc.), usado para alimentar as análises no notebook.

## 💻 Tecnologias Utilizadas

Este projeto foi desenvolvido utilizando a linguagem **Python** e um conjunto robusto de bibliotecas para análise de dados, visualização e geoprocessamento:

*   **[Pandas](https://pandas.pydata.org/)**: Para manipulação e análise e limpeza estrutural dos dados tabulares.
*   **[NumPy](https://numpy.org/)**: Para operações matemáticas e suporte a arrays multidimensionais.
*   **[Matplotlib](https://matplotlib.org/) & [Seaborn](https://seaborn.pydata.org/)**: Para a criação de visualizações estáticas e gráficos estatísticos elegantes.
*   **[GeoPandas](https://geopandas.org/)**: Para adicionar suporte a dados geográficos, permitindo operações espaciais diretamente em DataFrames.
*   **[Folium](https://python-visualization.github.io/folium/)**: Para a criação de mapas interativos baseados em Leaflet.js.
*   **[Shapely](https://shapely.readthedocs.io/)**: Para a manipulação e análise de objetos geométricos (pontos, linhas, polígonos).

## 🚀 Como Executar o Projeto

1.  **Clone o repositório:**
    ```bash
    git clone https://github.com/LeoSousaJesus/dados_queimadas2024
    cd dados_queimadas2024
    ```

2.  **Ambiente Virtual (Recomendado):**
    É recomendado criar um ambiente virtual e instalar as dependências necessárias.
    ```bash
    python -m venv venv
    source venv/bin/activate  # No Windows: venv\Scripts\activate
    pip install pandas numpy matplotlib seaborn geopandas folium shapely jupyter
    ```

3.  **Inicie o Jupyter Notebook:**
    ```bash
    jupyter notebook
    ```
    Em seguida, abra o arquivo `queimadas.ipynb` no seu navegador.

*Alternativamente, como o notebook original foi desenvolvido no Google Colab, você pode simplesmente fazer upload do arquivo `.ipynb` e do `.csv` para o seu Google Drive e abri-lo via **Google Colab**, que já possui a maioria dessas bibliotecas pré-instaladas.*
