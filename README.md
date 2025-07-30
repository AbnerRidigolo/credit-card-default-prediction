# 🧾 Previsão de Atraso em Pagamentos (Credit Card Default Prediction)

## 📌 Objetivo
Desenvolver um modelo de machine learning para prever se um cliente irá atrasar o pagamento da fatura do cartão de crédito, com base em seu perfil demográfico e histórico financeiro.

## 🗂️ Sobre o Projeto
Este projeto utiliza dados do UCI Machine Learning Repository para realizar previsões de inadimplência (default) por meio de técnicas supervisionadas de classificação. O pipeline contempla o pré-processamento, modelagem, avaliação e explicação dos resultados.

## 🔍 Etapas do Projeto
### 1. Análise e Pré-Processamento de Dados
- Limpeza e tratamento de valores inconsistentes.
- Engenharia de features baseada em variáveis de comportamento de crédito.
- Normalização e codificação das variáveis categóricas.

### 2. Modelagem Preditiva
- Algoritmos utilizados:
  - Regressão Logística
  - Random Forest
- Avaliação de performance:
  - AUC (Área sob a Curva ROC)
  - Recall
  - Precisão
  - Matriz de Confusão

### 3. Explicabilidade com SHAP
- Utilização de SHAP para interpretar o impacto de cada feature na decisão do modelo.
- Visualização dos atributos mais influentes na previsão de inadimplência.

## 📊 Dataset
- Nome: Default of Credit Card Clients Dataset  
- Fonte: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/default+of+credit+card+clients)

## 💡 Tecnologias Utilizadas
- Python 3.x
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn
- SHAP

## 📁 Estrutura dos Arquivos
📦credit-card-default-prediction  
 ┣ 📊 data/  
 ┃ ┗ credit_default.csv  
 ┣ 📈 notebooks/  
 ┃ ┣ 01_preprocessing.ipynb  
 ┃ ┣ 02_model_training.ipynb  
 ┃ ┗ 03_shap_explainability.ipynb  
 ┣ README.md  
 ┗ requirements.txt  

## ✅ Resultados
- Modelo com melhor desempenho: Random Forest
- AUC > 0.80, bom recall para identificação de inadimplentes.
- A variável mais influente foi o histórico de pagamentos recentes (`PAY_0` e `PAY_2`).
