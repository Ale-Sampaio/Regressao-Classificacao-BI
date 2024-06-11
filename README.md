# Regressao-Classificacao-BI
from sklearn.naive_bayes import GaussianNB

# Dados de exemplo
X = [[100, 20], [150, 30], [120, 25], [140, 28]]
y = ['Não Spam', 'Spam', 'Não Spam', 'Spam']

# Treinando o modelo
model = GaussianNB()
model.fit(X, y)


# Previsão para um novo e-mail
novo_email = [[130, 22]]
resultado = model.predict(novo_email)
print(f"Previsão para o novo e-mail: {resultado[0]}")
