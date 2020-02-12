# Introdução ao Aprendizado de Máquina Supervisionado com Python

[![Python](https://img.shields.io/badge/Python-3.6.8-blue)](https://www.python.org) [![Jupyter Notebook](https://img.shields.io/badge/Jupyter%20Notebook-6.0.2-orange)](https://jupyter.org/) [![VS Code](https://img.shields.io/badge/Visual%20Studio%20Code-1.42.0-purple)](https://code.visualstudio.com/)

Repositório com Materiais do Minicurso de Introdução ao Aprendizado de Máquina Supervisionado utilizando a linguagem Python.

## Estrutura do Minicurso

O minicurso é dividido em 4 partes, sendo elas:

### Parte 1

O Conjunto de Dados a ser utilizado durante o minicurso é uma cópia dos dados de Câncer de Mama do Estado de Wisconsin (EUA) de novembro de 1995, elaborado por: Dr. William H. Wolberg, W. Nick Street e Olvi L. Mangasarian. O Conjunto de Dados é carregado através da biblioteca `sklearn.datasets`.

Com o carregamento dos dados, eles serão divididos utilizando o método de Reamostragem _Holdout_ onde 60% dos dados são destinados para treino e 40% para teste dos algoritmos de Classificação.

No total, 4 algoritmos de Classificação são utilizados, sendo eles:
- [_Multinomial Naive Bayes_](https://scikit-learn.org/stable/modules/generated/sklearn.naive_bayes.MultinomialNB.html);
- [_Decision Tree_](https://scikit-learn.org/stable/modules/generated/sklearn.tree.DecisionTreeClassifier.html);
- [_Random Forest_](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html);
- [_Adaptive Boosting_](https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.AdaBoostClassifier.html).

Com o treinamento dos algoritmos e as previsões dos mesmos realizadas, os resultados são calculados a partir do acerto das previsões em relação as rótulos verdadeiros para os dados.

### Parte 2

Nesta Parte a Reamostragem Holdout é comparada com a Bootstrap, onde divide o Conjunto de Dados em dois subconjuntos (um para treino e outro para teste) com a reposição de dados, ou seja, um mesmo dado pode aparecer em ambos os subconjuntos.

Com a divisão dos dados utilizando duas Reamostragens, os algoritmos de classificação são iniciados utilizando parâmetros diferentes de seus padrões.

Já nos Resultados, as previsões dos algoritmos são comparadas com métricas estatísticas voltadas para os 4 possíveis valores de acordo com uma Matriz de Confusão de Classificação Binária.

### Parte 3

Nesta Parte a técnica _K-Fold_ de Validação Cruzada é utilizada para dividir o Conjunto de Dados em _k_ subconjuntos e execuções. Os algoritmos estão com os mesmos parâmetros informados na Parte 2.