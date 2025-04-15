# Detector de Fraude em Transações de Cartão de Crédito

Este repositório contém o código desenvolvido para a detecção de fraudes em transações de cartão de crédito, utilizando técnicas de machine learning, especialmente regressão logística. O projeto foi realizado como trabalho final da disciplina optativa **Tópicos em Novas Tecnologias I**, ministrada pelo professor Carlos Severiano no curso de Sistemas de Informação no IFMG Campus Sabará.

## Descrição do Projeto

O projeto tem como objetivo aplicar um modelo preditivo para identificar transações fraudulentas. Para isso, foram empregadas as seguintes etapas:

- **Análise Exploratória:** Inspeção dos dados, verificação de tipos e identificação de dados nulos.
- **Balanceamento de Dados:** Uso de undersampling para balancear a classe majoritária e minoritária, combatendo o desbalanceamento típico em bases de dados de fraudes.
- **Divisão dos Dados:** Separação do dataset em dados de treinamento, teste e validação.
- **Treinamento do Modelo:** Utilização da regressão logística para construir o modelo preditivo.
- **Avaliação e Validação:** Cálculo de métricas de desempenho (como acurácia) e criação de um dataframe para comparar os resultados das predições com os valores reais.

## Dependências

O projeto foi desenvolvido em Python e utiliza as seguintes bibliotecas:

- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [scikit-learn](https://scikit-learn.org/)

## Base de Dados

A base de dados utilizada para este projeto deve ser baixada separadamente. Você pode baixá-la neste [link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?resource=download).

Após o download, salve o arquivo CSV com o nome `creditcard.csv` na raiz do repositório para que o script possa carregá-lo corretamente.

## Como Executar

O projeto foi originalmente desenvolvido e testado no Google Colab. Se você deseja executá-lo, basta importar este repositório e garantir que o arquivo `creditcard.csv` esteja disponível na raiz.
