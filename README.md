# Desafio-Creditas

## O Modelo
Com o intuito de melhorar a esteira de classificação de clientes aprovados para análise de crédito do produto de Auto Equity, foi construído um modelo que manipulasse as informações obtidas pela esteira de crédito.

### Ferramentas Necessárias
As seguintes ferramentas foram usadas na construção do projeto:

- [Python 3](https://www.python.org/downloads/);
- [Anaconda](https://www.anaconda.com/);
- [Jupyter Notebook](https://jupyter.org/);
- [Shap Library](https://shap.readthedocs.io/en/latest/).

### Pré-requisitos
Para rodar o código o usuário deve ter instalado em seu ambiente o interpretador de [Python 3](https://www.python.org/downloads/), a plataforma [Anaconda](https://www.anaconda.com/) e instalar por meio do comando pip install a biblioteca [Shap Library](https://shap.readthedocs.io/en/latest/). A plataforma Anaconda já dispões da instalação de diversas bibliotecas para Ciência de Dados, utilizadas no desenvolvimento do modelo. Além disso a biblioteca Shap pode ser instalada no ambiente Jupyter Notebook pelo comando *!pip install* shap ou pelo Prompt de Comando do próprio computador pelo comando *pip install shap*.

### Como Rodar o Código
O código está dividido em 4 etapas, sendo elas:
- EDA (Análise Explanatória de Dados): Análise das variáveis com gráficos para entender como cada variável se comporta;
- Feature Engineering: Manipulação do dateset como criação de variáveis, preenchimento de valores nulos, tratamento de outliers e normalização e escalonamento de dados;
- Model Training: Criação e avaliação do modelo de Machine Learning, além da utilização de técnicas para identificar os melhores hiperparâmetros;
- Feature Importance: Verificando com a biblioteca Shap, quais as variáveis mais importantes para o modelo escolhido.

Se o usuário que for rodar o código já estiver com a biblioteca Shap instalada no seu ambiente o código pode ser reproduzido com o comando Restart & Run All do próprio Jupyter Notebook, levando em consideração algumas observações: 
- Todas as etapas randõmicas foram travadas com o comando np.random.seed(42) de forma que os resultados do código fossem reproduzíveis para qualquer usuário;
- A etapa de verificação dos hiperparâmetros pode ser um pouco mais demorada para rodar, caso o usuário deseje avaliar o modelo de forma mais rápida é recomendado pular essa etapa e partir para a seção de Feature Importance;
- Um código para a instalção da biblioteca shap está comentado no inicio da seção de Feature Importance, sendo assim o usuário poderá descomentar a linha de código e instalar a biblioteca pelo próprio Jupyter Notebook, caso ele não a tenha em seu ambiente. Sendo assim é importante ressaltar que se o usuário não tiver a biblioteca instalada o código apresentará um problema ao selecionar Restart & Run All;
- O usuário poderá rodar cada seção de forma separada e poderá pular a EDA desde que rode as primeiras 10 células, onde o código filtra em um dataset separado os clientes pré aprovados e retira as colunas com mais de 50% dos dados nulos;
- A melhor forma de rodar o código e entender o que foi feito é rodando cada seção na ordem que foi proposta, assim o usuário poderá entender as decisões feitas nas etapas de pré-processamento, limpeza de dados, treinamento do modelo, escolha de hiperparâmetros e feature importance.
