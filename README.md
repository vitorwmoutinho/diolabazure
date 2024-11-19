# Modelo de Previsão - Loja de Aluguel de Bicicletas #
### Objetivo
Criar um modelo de previsão de demanda para uma loja de aluguel de bicicletas utilizando Automated Machine Learning (AutoML) no Azure Machine Learning. Este projeto inclui a configuração de endpoints que permitem acesso ao modelo para previsão e integração com outras aplicações.

## Passo a Passo para Construção
### 1. Configuração do Ambiente no Azure
Criar uma conta no Azure Portal.
Configurar um Workspace de Machine Learning no Azure Machine Learning Studio.
Criar um Compute Instance para realizar o treinamento.
### 2. Preparação dos Dados
Dados históricos de aluguel de bicicletas contendo:
Data e hora do aluguel.
Condições climáticas (temperatura, umidade, velocidade do vento).
Indicador de feriado.
Dia da semana.
Quantidade de bicicletas alugadas.
Upload dos dados no Azure Blob Storage ou diretamente no Workspace do Azure.
### 3. Automated Machine Learning
Acessar o Azure Machine Learning Studio.
Criar um novo experimento AutoML:
Escolher o tipo de tarefa: Regressão.
Selecionar o conjunto de dados de entrada.
Configurar as métricas de avaliação (ex.: R², MAE).
Iniciar o treinamento para que o AutoML selecione automaticamente o melhor modelo com base nos dados fornecidos.
### 4. Implantação do Modelo
Após o treinamento, escolher o modelo com melhor desempenho.
Publicar o modelo como um endpoint de inferência no Azure:
Configurar os pontos de extremidade para permitir requisições via API REST.
Testar o endpoint diretamente no portal.
### 5. Integração com Aplicação
Utilizar o endpoint do modelo para previsões.
Criar uma API local com Flask para gerenciar as requisições do usuário e integrar ao modelo implantado.
