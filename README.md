# LH_CD_LUCASPAULINO
Este projeto visa prever as notas do IMDb para filmes utilizando um modelo de Machine Learning.
## Estrutura do Projeto

- `desafio_indicium_imdb.csv`: Arquivo CSV contendo os dados dos filmes.
- `main.py`: Script principal para carregar os dados, treinar o modelo e fazer previsões.
- `requirements.txt`: Arquivo com todas as dependências do projeto.

## Requisitos

- Python 3.7 ou superior
- Pip (gerenciador de pacotes do Python)

## Instalação

1. Clone o repositório para sua máquina local:

``bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

2. Crie um ambiente virtual (opcional, mas recomendado):

python -m venv venv
source venv/bin/activate  # No Windows use `venv\Scripts\activate`

3. Instale as dependências:

pip install -r requirements.txt

## Execução:

1. Coloque o arquivo desafio_indicium_imdb.csv na raiz do projeto.
2. Execute o script principal:

python main.py

### requirements.txt

``plaintext
pandas==1.3.5
scikit-learn==1.0.2

Uso
O script principal (main.py) carrega os dados, realiza o pré-processamento, treina um modelo de regressão RandomForest e faz previsões. Os resultados incluem a avaliação do modelo (Mean Absolute Error) e uma previsão de nota IMDb para um filme específico.

Detalhes Técnicos
Variáveis Utilizadas
- Numéricas: Released_Year, Runtime, Meta_score, No_of_Votes, Gross
- Categóricas: Certificate, Genre, Director, Star1, Star2, Star3, Star4

Transformações
   Imputação de Valores Ausentes: mean para variáveis numéricas, most_frequent para categóricas.
- Codificação: OneHotEncoder para variáveis categóricas.

Modelo
- RandomForestRegressor
-- Prós: Lida bem com dados categóricos e numéricos, robusto a outliers, não requer normalização dos dados.
-- Contras: Pode ser computacionalmente intensivo, menos interpretável.

Medida de Performance
- Mean Absolute Error (MAE): Mede a média dos erros absolutos entre as previsões e os valores reais.

Licença
Este projeto está licenciado sob a licença MIT.

### requirements.txt

``plaintext
pandas==1.3.5
scikit-learn==1.0.2
