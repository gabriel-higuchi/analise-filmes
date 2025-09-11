Análise Exploratória de Filmes do IMDb
1. Descrição do Projeto
Este projeto consiste em uma Análise Exploratória de Dados (EDA) de um conjunto de dados de filmes do IMDb. O objetivo principal é investigar a relação entre o sucesso financeiro e o sucesso de crítica, além de analisar o impacto de diretores e atores e construir um modelo preditivo para a nota do IMDb.

O projeto utiliza dados de bilheteria fornecidos e os enriquece com dados de orçamento e receita global de uma API externa (TMDB).

2. Pré-requisitos
Certifique-se de ter o Python 3.7 ou superior instalado em sua máquina. Além disso, as seguintes bibliotecas Python são necessárias:

pandas

numpy

matplotlib

requests

scikit-learn

jupyter

3. Instalação
Siga os passos abaixo para configurar o ambiente do projeto.

Passo 1: Clonar o Repositório
Primeiro, clone este repositório do Git para a sua máquina:

Bash

git clone https://github.com/seu-usuario/seu-repositorio.git
cd seu-repositorio
Passo 2: Instalar as Dependências
Instale as bibliotecas necessárias usando o pip. Crie um arquivo requirements.txt com o seguinte conteúdo:

pandas
numpy
matplotlib
requests
scikit-learn
jupyter
Então, execute o comando:

Bash

pip install -r requirements.txt
Passo 3: Configurar a Chave da API do TMDB
Para enriquecer os dados com o orçamento e a receita global dos filmes, o projeto utiliza a API do TMDB. Você precisará de uma chave de API para fazer as requisições.

Crie uma conta em https://www.themoviedb.org/.

Obtenha sua chave de API (v3).

Abra o arquivo cienciadedados.ipynb e substitua a chave de API na célula correspondente:

Python

api_key = "SUA_CHAVE_AQUI"
4. Como Executar o Projeto
Para executar a análise, basta iniciar o Jupyter Notebook e abrir o arquivo do projeto.

Inicie o Jupyter Notebook no terminal:

Bash

jupyter notebook
No seu navegador, abra o arquivo cienciadedados.ipynb.

Execute cada célula de código sequencialmente, de cima para baixo, para replicar todas as análises.

5. Análises Realizadas
O notebook cienciadedados.ipynb contém as seguintes análises:

Análise de Correlação: Mede a relação entre o sucesso financeiro (Gross) e as notas de crítica e público (IMDB_Rating e Meta_score).

Impacto de Diretores e Atores: Analisa a média de receita e notas para identificar os profissionais mais influentes.

Análise de Gênero: Compara o lucro médio de diferentes gêneros de filme, usando dados globais da API para uma análise mais precisa.

Previsão de Nota do IMDB: Demonstra a criação de um modelo de machine learning para prever a nota de um filme.

Exportação de Dados: Inclui um exemplo de como exportar uma tabela de dados para um arquivo PDF.
