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

```bash
git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio

python -m venv venv
source venv/bin/activate  # No Windows use `venv\Scripts\activate`

pip install -r requirements.txt

## Execução
Coloque o arquivo desafio_indicium_imdb.csv na raiz do projeto.
Execute o script principal:
python main.py

### requirements.txt

```plaintext
pandas==1.3.5
scikit-learn==1.0.2
