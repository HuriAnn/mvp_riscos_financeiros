# 📊 Projeto de Análise de Riscos Financeiros
📌 Descrição
Análise dos fatores que influenciam o risco financeiro de clientes, incluindo EDA, tratamento de dados, clusterização e um modelo preditivo simples para auxiliar decisões de crédito.

## 🗂️ Escopo do Trabalho

1️⃣ Carregamento dos Dados

2️⃣ Análise Exploratória (Distribuições, correlações, valores ausentes)

3️⃣ Tratamento de Valores Ausentes

4️⃣ Criação de Variáveis Derivadas

5️⃣ Clusterização K-Means + PCA

6️⃣ Modelagem Preditiva (Random Forest)


## 📚 Dados Utilizados

Origem: Dataset no GitHub

Registros: 15.000

Variável alvo: Classificação de Risco (High, Medium, Low)

## 📖 Dicionário de Dados

| 🏷️ Variável                  | 📊 Tipo    | 📝 Descrição                           |
| ----------------------------- | ---------- | -------------------------------------- |
| **Idade**                     | Numérica   | Idade do cliente                       |
| **Gênero**                    | Categórica | Gênero do cliente (Masculino/Feminino) |
| **Escolaridade**              | Categórica | Nível de escolaridade do cliente       |
| **Estado Civil**              | Categórica | Estado civil                           |
| **Renda**                     | Numérica   | Renda anual do cliente                 |
| **Score de Crédito**          | Numérica   | Pontuação de crédito                   |
| **Valor do Empréstimo**       | Numérica   | Valor solicitado no empréstimo         |
| **Finalidade do Empréstimo**  | Categórica | Motivo do empréstimo                   |
| **Situação de Emprego**       | Categórica | Status do emprego                      |
| **Anos no Emprego Atual**     | Numérica   | Tempo no emprego atual                 |
| **Histórico de Pagamento**    | Texto      | Texto livre sobre pagamentos           |
| **Razão Dívida/Renda**        | Numérica   | Proporção entre dívidas e renda        |
| **Valor dos Bens**            | Numérica   | Patrimônio declarado                   |
| **Número de Dependentes**     | Numérica   | Dependentes financeiros                |
| **Cidade / Estado / País**    | Categórica | Localização                            |
| **Inadimplências Anteriores** | Numérica   | Nº de inadimplências                   |
| **Mudança no Estado Civil**   | Categórica | Alteração recente no estado civil      |
| **Classificação de Risco**    | Categórica | Variável alvo (High, Medium, Low)      |


## 🧪 Variáveis Derivadas Criadas

| 🏷️ Variável                | 📊 Tipo        | 📝 Descrição                               |
| --------------------------- | -------------- | ------------------------------------------ |
| **Faixa de Idade**          | Categórica     | Agrupamento da idade em intervalos         |
| **Faixa de Renda**          | Categórica     | Agrupamento da renda em quintis            |
| **Faixa Score**             | Categórica     | Agrupamento do Score em quintis            |
| **Risco Estimado**          | Numérica       | Métrica calculada para estimar o risco     |
| **Faixa de Risco Estimado** | Categórica     | Classificação categórica do risco estimado |
| **Cluster**                 | Numérica (Int) | Cluster atribuído pelo K-Means             |
| **PCA1, PCA2**              | Numérica       | Componentes principais para visualização   |


## 🛠️ Ferramentas Utilizadas

🐍 Python • 📊 Pandas • ➗ NumPy • 🎨 Seaborn • 📈 Matplotlib • 🤖 Scikit-learn


## 📊 Principais Resultados

✅ Maioria dos clientes em faixas de renda mais baixas

👥 Clusterização identificou perfis distintos

🎯 Modelo classificou bem clientes de baixo risco, mas teve desafios em separar High/Medium

🔎 Variável Risco Estimado aproxima a classificação do risco percebido

## ⚠️ Limitações

🔀 Classes desbalanceadas

⚙️ Modelo inicial simples

📝 Variáveis textuais não usadas


## 🔎 Próximos Passos

⚖️ Técnicas de balanceamento (SMOTE, class weights)

🚀 Testar XGBoost / LightGBM

🧠 Ajustar métricas para melhor sensibilidade às classes minoritárias



## 🚀 Execute o Notebook no Google Colab

[![Abrir no Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/HuriAnn/mvp_riscos_financeiros/blob/main/MVP_An%C3%A1lise_Riscos_Financeiros.ipynb)

