# UCI Machine Learning Benchmark

Pipeline comparativo de algoritmos de classificação supervisionada em **Python** utilizando o ecossistema **Scikit-Learn** e a base de dados do repositório **UCI Machine Learning Repository** (Adult Census Income / ID 2).

## 📊 Algoritmos Comparados

O pipeline avalia e compara o desempenho dos seguintes classificadores:

- **Logistic Regression (LR)**
- **Support Vector Classifier (SVM / RBF)**
- **Random Forest Classifier (RFC)**
- **K-Nearest Neighbors (KNN)**

## ⚙️ Pré-processamento e Pipeline

O pré-processamento é construído de forma modular com `ColumnTransformer`:
- Variáveis Numéricas: Imputação pela média (`SimpleImputer`) e padronização (`StandardScaler`).
- Variáveis Categóricas: Imputação pela moda e codificação one-hot (`OneHotEncoder`).
- Avaliação: Métricas de Acurácia e Relatório Completo de Classificação (Precision, Recall, F1-Score).

## 🚀 Como Executar

```bash
# Instalar dependências
pip install -r requirements.txt

# Executar o pipeline de treinamento e benchmark
python main.py
```
