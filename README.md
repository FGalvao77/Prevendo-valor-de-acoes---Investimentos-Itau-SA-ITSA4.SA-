# Prevendo valor de ações - Investimentos Itaú/SA (ITSA4.SA)

![image](https://user-images.githubusercontent.com/63373520/148662814-51c7b14a-a3af-4e34-8a7b-2f73801ca1cb.png)


**Introdução**

Criar um modelo de predição para estimar valores de ações. Nesse caso, as ações do [**ITSA4.SA**](https://finance.yahoo.com/quote/ITSA4.SA?p=ITSA4.SA&.tsrc=fin-srch), utilizaremos a biblioteca  [`yfinance`](https://pypi.org/project/yfinance/) para carregar os dados diretamente do site [**Yahoo! Finance**](https://finance.yahoo.com/).

Usaremos utilizar dois de modelos de regressão do [Scikit-learn](https://scikit-learn.org/stable/index.html). São eles:
- uma função simples de regressão linear, o [LinearRegression](https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LinearRegression.html?highlight=linear#sklearn.linear_model.LinearRegression) e,
- uma função de rede neural, o [MLPRegressor](https://scikit-learn.org/stable/modules/generated/sklearn.neural_network.MLPRegressor.html?highlight=mlp#sklearn.neural_network.MLPRegressor).
 - nessa função específica iremos ajustar os hiperparâmetros e encontrar os melhores ajustes.

Para aplicação mais próxima da realidade, o conjunto de dados será particionado em três partes - treino, validação e teste.
E realizar todas estapas necessárias com os dados de treino e validação:
- análise exploratória dos dados;
- tratamento dos dados;
- separação dos dados,
- avaliação do modelo.

Por fim, iremos aplicar o modelo que apresentou melhor _coeficiente de determinação_ e, realizar as predições com os dados de teste.

Link do [notebook](https://colab.research.google.com/drive/1Xde2j0A6CGRUE5-T4mT6OkqzlNZFdagf#scrollTo=9omfbKtovHb-).
