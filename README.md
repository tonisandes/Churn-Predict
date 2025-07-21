Exercício para Encontrar Churn
Este projeto tem como objetivo construir um modelo preditivo para identificar clientes com alta probabilidade de churn (desistência ou cancelamento de serviço) a partir de um conjunto de dados. O pipeline inclui análise exploratória, pré-processamento, modelagem e avaliação de desempenho.
Descrição do Projeto
O projeto utiliza um conjunto de dados contendo informações sobre clientes para prever o churn. As etapas incluem importação de dados, limpeza, transformação, aplicação de um modelo de aprendizado de máquina (Regressão Logística) e avaliação do desempenho com métricas como acurácia, relatório de classificação e matriz de confusão.
Pré-requisitos
Para executar este projeto, você precisará instalar as seguintes bibliotecas Python:
pip install pandas numpy scikit-learn

Além disso, é necessário ter um conjunto de dados data.csv na pasta Data/ com informações sobre os clientes, incluindo a coluna Churn (alvo) e outras variáveis relevantes.
Estrutura do Projeto

Data/: Pasta contendo o arquivo data.csv com os dados dos clientes.
Código: O código principal está descrito no notebook ou script Python, com as seguintes etapas:
Importação de Bibliotecas: Importação de pandas, numpy, sklearn para manipulação de dados e modelagem.
Carregamento dos Dados: Leitura do arquivo data.csv em um DataFrame.
Exploração dos Dados: Análise inicial para verificar colunas, tipos de dados, valores ausentes e estatísticas descritivas.
Pré-processamento:
Conversão da coluna TotalCharges para formato numérico.
Remoção de valores ausentes.
Exclusão da coluna customerID (se presente).
Transformação da coluna Churn em binária (0 para 'No', 1 para 'Yes').
Codificação de variáveis categóricas usando one-hot encoding (get_dummies).
Divisão dos dados em treino (70%) e teste (30%).
Normalização das variáveis numéricas com StandardScaler.


Modelagem: Treinamento de um modelo de Regressão Logística.
Avaliação: Avaliação do modelo com acurácia, relatório de classificação e matriz de confusão.



Como Executar

Clone este repositório ou copie o código fornecido.
Certifique-se de que o arquivo data.csv está na pasta Data/.
Instale as dependências listadas acima.
Execute o script Python ou notebook para realizar as etapas de análise, pré-processamento, modelagem e avaliação.

python churn_prediction.py

Resultados
O modelo treinado fornece:

Acurácia: Percentual de previsões corretas no conjunto de teste.
Relatório de Classificação: Métricas como precisão, recall e F1-score para as classes Churn (0 e 1).
Matriz de Confusão: Distribuição das previsões corretas e incorretas.

Exemplo de saída:
Tamanho do treino: (n_samples, n_features)
Tamanho do teste: (n_samples, n_features)
Acurácia: X.XX
Relatório de classificação:
              precision    recall  f1-score   support
           0       X.XX      X.XX      X.XX      XXX
           1       X.XX      X.XX      X.XX      XXX
Matriz de confusão:
[[TN  FP]
 [FN  TP]]
