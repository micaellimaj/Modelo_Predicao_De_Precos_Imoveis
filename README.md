# 🌃 Análise e Predição de Preços de Imóveis de NY 

![banner](Imagens/Banner.jpeg)

## 👀 Introdução: 

Esse projeto traz dados sobre aluguéis de Imóveis em Nova York com o objetivo principal de criar um modelo de predição de preço. Os dados atrás diferentes atributos que impactam no preço dos imóveis, e com esses dados foi passado por etapas de pré-processamento de dados , análise exploratória e criação de modelos preditivos (regressão, classificação e agrupamento) para geração de insights.

## 💡 Estrutura:

![estrutura_projeto](Imagens/Estrutura_projeto_price.gif)


## 🕵🏾‍♂️ Justificativa:

Alocação para um time que está trabalhando atualmente junto a um cliente no processo de criação de uma plataforma de aluguéis temporários na cidade de Nova York. Para o desenvolvimento de sua estratégia de precificação, pediu para que fizesse uma análise exploratória dos dados de seu maior concorrente, assim como um teste de validação de um modelo preditivo.

<p align="center">
    <img src = "https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExZXYxcmxpMjQxbzVuZ3psbGNxNWN5anBjNTR5aDFma3F0dWpvMnhxbyZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/sdT5XG0EAqUuGi0UJZ/giphy.gif" />
</p>

## 🪄 Tecnologias:

<div align="center" style="display: inline_block">
<img align="center" alt="github" src="https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white" />
<img align="center" alt="vscode" src="https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white" /> 
<img align="center" src="https://img.shields.io/badge/Jupyter_Notebook-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="icon jupyter notebook">
<img align="center" src="https://img.shields.io/badge/Python-133DAB?style=for-the-badge&logo=python&logoColor=y1CC0C0" alt="icon python" >
<img align="center" src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="icon pandas">
<img align="center" src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="icon numpy">
<img align="center" src="https://img.shields.io/badge/Matplotlib-0B2C4A?style=for-the-badge&logo=python&logoColor=white" alt="icon matplotlib">
<img align="center" src="https://img.shields.io/badge/Seaborn-4C4C4C?style=for-the-badge&logo=python&logoColor=white" alt="icon seaborn">
<img align="center" src="https://img.shields.io/badge/Scikit--learn-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="icon scikit-learn">
    
</div>

## 📋 Atributos: 

| **Variável**                  | **Descrição**                                             | **Tipo**         | **Subtipo**       |
|-------------------------------|-----------------------------------------------------------|------------------|-------------------|
| id                            | Identificador Único                                       | Quantitativa     | Discreta          |
| nome                          | Título do anúncio                                         | Qualitativa      | Nominal           |
| host_id                       | Identificador Único do anfitrião                          | Quantitativa     | Discreta          |
| host_name                     | Nome do anfitrião                                         | Qualitativa      | Nominal           |
| bairro_group                  | Grupo ou região do bairro onde o imóvel está localizado   | Qualitativa      | Nominal           |
| bairro                        | Nome do bairro onde o imóvel está localizado              | Quantitativa     | Contínua          |
| latitude                      | Coordenada geográfica de latitude do imóvel                | Quantitativa     | Contínua          |
| longitude                     | Coordenada geográfica de longitude do imóvel               | Quantitativa     | Contínua          |
| room_type                     | Tipo de acomodação                                        | Qualitativa      | Nominal           |
| price                         | Preço por noite em dólares                                | Quantitativa     | Contínua          |
| minimo_noites                 | Número mínimo de noites exigido para reserva              | Quantitativa     | Discreta          |
| numero_de_reviews             | Número total de avaliações do anúncio                     | Quantitativa     | Discreta          |
| ultima_review                 | Data da última avaliação recebida                         | Qualitativa      | Ordinal           |
| reviews_por_mes               | Média de avaliações recebidas por mês                     | Quantitativa     | Contínua          |
| calculado_host_listings_count | Quantidade de anúncios ativos do anfitrião                | Quantitativa     | Discreta          |
| disponibilidade_365           | Número de dias disponíveis para reserva no ano           | Quantitativa     | Discreta          |

## 🚧 Etapas do Projeto:

1. **Pré-Processamento dos dados**:
    * **Criação do dicionário de dados**: Criação de um dicionário sobre os dados importados, trazendo informações como descrição e tipo dos dados.
    * **Tratamento de dados incorretos**: Garantia de que os dados estarão prontos para a análise exploratória e para os modelos de Machine Learning.
    * **Preparação dos dados para Modelos de ML**: Preparação adicional para que os modelos de Machine Learning funcionem sem problemas.

2. **Análise Exploratória de Dados (EDA)**:

    * **Perguntas de Partida e Hipóteses**: São feitas perguntas sobre os dados e, com base neles, hipóteses são formuladas com o objetivo de gerar insights sobre esses dados.
    * **Resolução das Perguntas**: Manipulação e visualização de dados para responder às perguntas de partida e, com base nelas, validar as hipóteses e gerar insights.
    * **Insights**: Resumo dos insights gerados durante a resolução das perguntas.

3. **Aplicação de Modelos de Machine Learning**:

    * **Transformação dos dados**: Preparação dos dados para o modelo, envolvendo etapas com normalização, codificação de variáveis categóricas, dentre outras.
    * **Modelos de Regressão**: Diferentes modelos de regressão (LinearRegressiom, KNeighborsRegressor, DummyRegressor) são treinados, avaliados e usados para fazer predição de dados. São calculados métricas como MAE, MDE e R².
    * **Modelos de Classificação**: Diferentes modelos de Classificação (LogisticRegression, KNeighborsClassifier) são treinados, avaliados e udados para fazer predição. São calculados métricas como precisão, recall, F1-score.
    * **Modelo de Agrupamento**: Uso do K-Médias para agrupar os dados ao seu grupo mais próximo e identificação do perfil dos dados.Uso do método do cotovelo, centroídes e estudo de clusters.
    * **Insights**: Resumo dos insights gerados durante a desenvolvimento dos modelos.

## 🗂️ Diretórios:

```
.
├── data/              # Diretório contendo todos os arquivos de dados
│
├── Imagens/           # Contém imagens e gifs utilizados no readme
│
├── docs/              # Documentação do projeto
│
├── models/            # Modelos treinados e serializados, predições ou resumos de modelos
│
├── notebooks/         # Diretório contendo todos os notebooks utilizados nos passos
│
├── README.md          # Informações gerais do projeto
│
└── riqueriments.txt

```

## 🛑 Conclusão:

Este projeto passou por etapas fundamentais e comuns na área de ciências de dados, em que foi necessário passar por etapas de processamento, modelagem e análise exploratória de dados. E com base nessas etapas foi possível a criação de modelos de Machine e geração de insights, ajudando a tomar decisões mais informadas e acertivas na criação da plataforma de aluguéis.
