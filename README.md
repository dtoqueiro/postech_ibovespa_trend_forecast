# POSTECH - Tech Challenge - Fase 2: Previsão do IBOVESPA
## Sobre o Projeto
Este repositório contém o desenvolvimento do Tech Challenge da Fase 02 do curso de Pós-Graduação em Data Analytics da POSTECH FIAP. O projeto consiste na criação de um modelo preditivo para o Índice Ibovespa. 


## O Desafio
A missão principal é desenvolver um modelo preditivo que seja capaz de prever a tendência de fechamento do índice IBOVESPA para o dia seguinte, ou seja, se o índice fechará em alta (valor maior que o do dia atual) ou em baixa (valor menor que o do dia atual). 
 

## Requisitos do Projeto
Para a conclusão do desafio, os seguintes requisitos foram estabelecidos:

- Fonte de Dados: Utilizar os dados históricos do índice IBOVESPA, disponíveis publicamente. 

- Período dos Dados: Selecionar o período "diário" e utilizar um intervalo de, no mínimo, 2 anos de dados históricos. 

- Pré-processamento: Realizar o tratamento e a preparação necessários nos dados para que possam ser utilizados no modelo preditivo. 

- Conjunto de Teste: O conjunto de dados para teste deve obrigatoriamente conter os últimos 30 dias de dados disponíveis. 

- Acuracidade Mínima: O modelo deve atingir uma acuracidade mínima de **75%** no conjunto de teste. 

## Metodologia Aplicada
O desenvolvimento do projeto seguiu as seguintes etapas:

Aquisição e Exploração dos Dados: Coleta dos dados históricos do IBOVESPA e análise exploratória para entendimento das características e padrões da série temporal. 

Engenharia de Atributos: Criação de novas features a partir dos dados brutos para enriquecer o modelo, como médias móveis, variações percentuais e indicadores técnicos. 

Preparação da Base: Estruturação da base de dados para o problema de previsão, incluindo a definição da variável alvo (target - alta ou baixa) e o tratamento da natureza sequencial dos dados, possivelmente utilizando janelas deslizantes (sliding windows) ou features defasadas (lagged features). 

Escolha e Treinamento do Modelo: Seleção de um ou mais algoritmos de Machine Learning (ex: Regressão Logística, Árvores de Decisão, LSTM) e justificativa da escolha.  O modelo foi treinado com os dados históricos, excluindo o período reservado para teste.

Avaliação de Resultados: Análise das métricas de performance do modelo no conjunto de teste para garantir sua confiabilidade e discutir os trade-offs entre acuracidade e overfitting. 

## Entregas
Este repositório contém:

Código-fonte: Uma pasta com todos os arquivos do projeto, incluindo notebooks, scripts e dados. 

Apresentação (Storytelling): Um arquivo em PDF com a apresentação do projeto, detalhando todas as etapas da metodologia. 

Vídeo Gerencial: Link para um vídeo de no máximo 5 minutos com uma explicação gerencial de como interpretar os resultados obtidos. 

## Como Executar o Projeto
Para replicar os resultados, siga os passos abaixo:

Clone o repositório:

``` Bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio 
```

## Instale as dependências:

``` Bash
uv init -p 3.13
uv venv -p 3.13
# Ative o ambiente virtual
# Instale as dependências
uv sync 
Execute o notebook principal:
Abra e execute o notebook desafio.ipynb em um ambiente como Jupyter Notebook ou Google Colab para ver todo o processo de análise e modelagem.
```

## Equipe
Daniel Lins Toqueiro
- Grupo 35
- GitHub: [Link do GitHub do Projeto](https://github.com/dtoqueiro/postech_ibovespa_trend_forecast)