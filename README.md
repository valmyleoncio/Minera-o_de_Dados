# Algortimo de Agrupamento

Este repositório apresenta o projeto final desenvolvido como parte da disciplina de Mineração de Dados. O foco do projeto é a implementação de um algoritmo de agrupamento aplicado a um conjunto de dados de notícias. O objetivo principal é identificar padrões e agrupar notícias semelhantes com base no conteúdo de seus títulos. O desenvolvimento abrange desde o carregamento do dataset até a visualização dos resultados, englobando etapas como pré-processamento, treinamento utilizando K-means e análise das métricas

## Bibliotecas

O projeto faz uso das seguintes bibliotecas:

- `numpy` e `pandas` para manipulação de dados.
- `nltk` para processamento de linguagem natural.
- `matplotlib` e `seaborn` para visualização de dados.
- `re`, `json` e `BeautifulSoup` para limpeza e pré-processamento de texto.
- `umap` para redução de dimensionalidade.
- `wordcloud` para criação de nuvem de palavras.
- `sklearn` para implementação do algoritmo K-means e métricas.
- `prettytable` para exibição tabular de dados.

## Carregamento do Dataset

O conjunto de dados utilizado é proveniente do arquivo 'uci-news-aggregator.csv', contendo informações sobre notícias, como título, URL, editor, categoria, entre outras. O dataframe foi carregado utilizando a biblioteca `pandas`.

## Pré-processamento

O pré-processamento dos dados inclui a remoção de caracteres indesejados, eliminação de stopwords, lematização de palavras e transformação para letras minúsculas.

## Treinamento (Kmeans)

O algoritmo K-means foi aplicado ao conjunto de dados após a vetorização dos títulos utilizando a técnica TF-IDF. O número de clusters escolhido foi 5.

## Visualização

A visualização dos resultados inclui a listagem das notícias em cada cluster, a lista de palavras mais frequentes em cada cluster e uma demonstração gráfica utilizando a técnica de redução de dimensionalidade SVD.

## Métricas

As métricas utilizadas para avaliação do modelo incluem o Silhouette score e a Inércia.

## Demonstração Gráfica

O projeto oferece uma demonstração gráfica através da criação de uma nuvem de palavras para cada cluster, proporcionando uma visão mais intuitiva dos temas predominantes em cada agrupamento.
