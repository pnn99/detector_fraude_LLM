# Detector de Fraude em Transações de Cartão de Crédito

Este repositório contém o código de um projeto de detecção de fraudes em transações de cartão de crédito, utilizando um pipeline completo de machine learning. O trabalho foi iniciado na disciplina optativa **Tópicos em Novas Tecnologias I** e foi aprofundado e refinado para a disciplina de **Inteligência Artificial**, ministrada pelo professor **Carlos Alexandre** no curso de Sistemas de Informação no IFMG Campus Sabará.

O projeto também serve como base para um **minicurso** sobre o tema, demonstrando um fluxo de trabalho realista, desde a análise básica até a otimização de modelos complexos.

## Descrição do Projeto

O projeto tem como objetivo aplicar e comparar múltiplos modelos preditivos para identificar transações fraudulentas. Para isso, foram empregadas as seguintes etapas:

- **Análise Exploratória:** Inspeção dos dados, verificação de tipos e identificação do forte desbalanceamento entre as classes.
- **Balanceamento de Dados:** Uso da técnica de *undersampling* para criar um dataset balanceado e justo para o treinamento dos modelos.
- **Aplicação de Múltiplos Algoritmos:** Foram testados e comparados diversos modelos de classificação, incluindo:
    - Regressão Logística (como linha de base obrigatória)
    - Árvore de Decisão
    - Support Vector Machine (SVM)
    - Random Forest
    - Gradient Boosting
- **Ensemble Learning:** Implementação de um modelo `StackingClassifier` como método exclusivo, combinando as predições dos algoritmos de base.
- **Otimização de Hiperparâmetros:** Uso de `GridSearchCV` para encontrar as melhores configurações para os modelos de base, buscando maximizar a performance.
- **Avaliação Completa e Visualização:** Análise de performance com métricas como acurácia, F1-score e **Matriz de Confusão**. Foram gerados gráficos para comparar os modelos ("antes e depois" da otimização) e interpretar a importância das features.

## Dependências

O projeto foi desenvolvido em Python e utiliza as seguintes bibliotecas:

- [Pandas](https://pandas.pydata.org/)
- [NumPy](https://numpy.org/)
- [scikit-learn](https://scikit-learn.org/)
- [Matplotlib](https://matplotlib.org/)
- [Seaborn](https://seaborn.pydata.org/)

## Base de Dados

A base de dados utilizada para este projeto deve ser baixada separadamente. Você pode baixá-la neste [link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud?resource=download).

Após o download, salve o arquivo CSV com o nome `creditcard.csv` na raiz do repositório para que o script possa carregá-lo corretamente.