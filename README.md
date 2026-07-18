# House Price Prediction Project

## Projeto de Previsão de Preços de Imóveis com Machine Learning

Projeto desenvolvido no curso **Desenvolvimento de IA para Análise Preditiva – Módulo 1**.

Este projeto tem como objetivo desenvolver um modelo de Aprendizado de Máquina capaz de prever preços de imóveis utilizando características físicas e informações de localização.

A solução aplica um fluxo completo de Ciência de Dados, envolvendo análise exploratória, tratamento de dados, engenharia de atributos, treinamento, avaliação e versionamento do modelo.

---

# Objetivo do Projeto

O objetivo deste projeto é desenvolver um modelo preditivo capaz de estimar o valor de venda de imóveis do condado de **King County, Estados Unidos**.

A variável-alvo utilizada no modelo é:

- **price** – valor de venda do imóvel em dólares.

A previsão de preços pode auxiliar imobiliárias, compradores, vendedores e instituições financeiras na tomada de decisão baseada em dados.

---

# Dataset Utilizado

**Dataset:**

- `kc_house_data.csv`

**Fonte:**

King County House Sales Dataset

O conjunto de dados contém aproximadamente **21 mil registros** de vendas de imóveis residenciais, incluindo informações como:

- Número de quartos;
- Número de banheiros;
- Área construída;
- Tamanho do terreno;
- Número de andares;
- Vista para água;
- Condição do imóvel;
- Grau de qualidade;
- Localização;
- Ano de construção.

---

# Tecnologias Utilizadas

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-Learn
- Google Colab
- GitHub

---

# Etapas Desenvolvidas

O projeto foi desenvolvido seguindo um pipeline de Machine Learning:

- Análise Exploratória dos Dados (EDA);
- Tratamento e limpeza dos dados;
- Identificação e tratamento de valores ausentes;
- Análise de outliers;
- Engenharia de atributos (Feature Engineering);
- Preparação dos dados para modelagem;
- Treinamento do modelo;
- Avaliação das métricas;
- Versionamento do modelo treinado.

---

# Modelo de Machine Learning

**Algoritmo utilizado:**

- Regressão Linear

Para avaliação do modelo, os dados foram divididos da seguinte forma:

- **80%** para treinamento;
- **20%** para teste.

Essa divisão permitiu avaliar o desempenho do modelo em dados que não participaram do treinamento, verificando sua capacidade de generalização.

Após a validação do modelo utilizando a divisão de 80% para treinamento e 20% para teste, foi realizado um treinamento final com **100% da base de dados disponível**, visando gerar a versão definitiva do modelo para disponibilização no repositório.

O modelo treinado foi salvo e versionado na pasta:

```text
models/v1/
```

---

# Avaliação do Modelo

O modelo foi avaliado utilizando as seguintes métricas:

- MAE (Erro Absoluto Médio);
- MSE (Erro Quadrático Médio);
- RMSE (Raiz do Erro Quadrático Médio);
- R² (Coeficiente de Determinação).

## Resultados Obtidos

| Métrica | Resultado |
|---------|----------:|
| MAE | 126.904,31 |
| MSE | 44.964.934.559,27 |
| RMSE | 212.049,37 |
| R² | 0,70 |

O modelo apresentou um coeficiente de determinação (**R²**) de aproximadamente **0,70**, indicando que consegue explicar cerca de **70% da variação dos preços dos imóveis** utilizando as características disponíveis no dataset.

---

# Estrutura do Projeto

```text
house_price_prediction_project/
│
├── data
│   └── raw
│       └── kc_house_data.csv
│
├── models
│   └── v1
│       ├── modelo_regressao_v1.pkl
│       └── metricas_v1.json
│
├── notebooks
│   └── house_price_prediction_project.ipynb
│
├── README.md
├── requirements.txt
├── LICENSE
└── .gitignore
```

---

# Arquivos do Repositório

O repositório contém:

- Notebook com todas as etapas do desenvolvimento;
- Dataset bruto utilizado no projeto;
- Modelo de Machine Learning treinado;
- Arquivo JSON contendo as métricas de avaliação;
- Arquivo `requirements.txt` com as bibliotecas utilizadas;
- Documentação completa do projeto.

---

# Como executar o projeto

1. Clone este repositório.
2. Instale as dependências utilizando o arquivo `requirements.txt`.
3. Abra o notebook `house_price_prediction_project.ipynb` no Google Colab ou Jupyter Notebook.
4. Execute as células na ordem apresentada.

---

# Melhorias Futuras

Como evolução para próximas versões do modelo, podem ser aplicadas melhorias como:

- Aplicação de One-Hot Encoding para variáveis categóricas, como `zipcode`;
- Análise de multicolinearidade utilizando VIF (Variance Inflation Factor);
- Seleção das variáveis com maior impacto no preço dos imóveis;
- Teste de algoritmos mais robustos, como Random Forest, Decision Tree e XGBoost;
- Otimização de hiperparâmetros;
- Aplicação de validação cruzada (Cross Validation);
- Desenvolvimento de uma interface para utilização do modelo por usuários finais.

---

# Autora

**Samira Salema**

Projeto desenvolvido para o curso **Desenvolvimento de IA para Análise Preditiva – Módulo 1 (SCTEC)**.

**Ciência de Dados | Inteligência Artificial | Machine Learning**
