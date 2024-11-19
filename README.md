Modelo de Previsão - Loja de Aluguel de Bicicletas
Objetivo
Criar um modelo de previsão de demanda para uma loja de aluguel de bicicletas com endpoints configurados, permitindo que o sistema seja acessado por outras aplicações.

Passo a Passo para Construção
1. Configuração do Ambiente
Linguagem: Python.
Bibliotecas Necessárias:
pandas: Para manipulação de dados.
numpy: Para operações numéricas.
scikit-learn: Para criação e avaliação do modelo de previsão.
flask: Para criar a API e configurar os endpoints.
joblib: Para salvar e carregar o modelo.
requests: Para testar os endpoints.
2. Coleta de Dados
Dados históricos de aluguel de bicicletas contendo colunas como:
Data.
Hora.
Condições climáticas (temperatura, umidade, vento).
Dia da semana.
Feriado (sim/não).
Demanda de bicicletas.
