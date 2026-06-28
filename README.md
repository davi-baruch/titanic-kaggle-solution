# 🚢 Desafio Kaggle - Titanic: Machine Learning from Disaster

Este repositório contém a minha solução para o desafio do Titanic no Kaggle. O objetivo principal deste projeto é prever quais passageiros sobreviveram ao naufrágio utilizando técnicas de processamento de Dados e aprendizado de máquina.

## Tecnologias e bibliotecas utilizadas

O projeto foi desenvolvido em **Python 3** pelo jupyter notebook, utilizando as seguintes bibliotecas:
* **`pandas`**: Manipulação, estruturação e limpeza das bases de dados.
* **`numpy`**: Operações matemáticas em geral.
* **`seaborn` & `matplotlib.pyplot` (`plt`)**: Visualização de dados e gráficos.
* **`scikit-learn`**:
  * `RandomForestClassifier`: Algoritmo preditivo baseado em árvores de decisão.
  * `train_test_split`: Divisão dos dados para validação inicial.
  * `KFold`: Técnica robusta para validação cruzada.

---

## Ciclo de desenvolvimento do modelo

O projeto foi dividido nas seguintes etapas essenciais:

### 1. Limpeza de dados
Tratamento de valores ausentes (NaN) em colunas críticas (como `Age`, `Cabin` e `Embarked`), além de conversão de variáveis categóricas em formatos numéricos adequados para o modelo.

### 2. Validação cruzada com K-Fold
Para garantir a estabilidade do modelo e evitar o *overfitting*, foi aplicada a técnica de **Validação Cruzada (K-Fold)**. O dataset de treino foi dividido de forma iterativa, medindo a **precisão (accuracy)** do modelo em múltiplos cenários reais de teste.

### 3. Treinamento do modelo
Ajuste do algoritmo `RandomForestClassifier` para que o modelo crie múltiplos caminhos de decisão para classificar de forma otimizada se um passageiro sobreviveu ou não.

### 4. Análise de erros
Identificação de quais padrões e perfis de passageiros fizeram o algoritmo errar.

### 5. Predição nos dados de teste
Aplicação do modelo final sobre o arquivo `test.csv` salvas em `modelo.csv`.

---
## Fonte dos Dados
Os dados utilizados neste projeto foram extraídos diretamente do site oficial do Kaggle:
* **Dataset:** https://www.kaggle.com/c/titanic](https://www.kaggle.com/competitions/titanic/data

---
