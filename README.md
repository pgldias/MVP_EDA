# MVP de Análise de Dados - CS:GO Round Snapshots

Este projeto é um MVP de Análise de Dados desenvolvido como parte de uma disciplina de pós-graduação em Ciência de Dados. O objetivo foi aplicar boas práticas de exploração, pré-processamento e documentação de dados, utilizando um conjunto de dados do jogo Counter-Strike: Global Offensive (CS:GO).

[![Abrir no Google Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/pgldias/MVP_EDA/blob/main/MVP_EDA.ipynb)

---

## Objetivo

Investigar quais variáveis influenciam o resultado de uma rodada de CS:GO com base em dados reais de partidas competitivas. O foco está em realizar uma análise exploratória completa e preparar os dados para futuras etapas de modelagem preditiva.

---

## Dataset

- **Fonte:** [Kaggle - CS:GO Round Winner Classification](https://www.kaggle.com/datasets/christianlillelund/csgo-round-winner-classification)
- **Descrição:** Snapshots extraídos de partidas profissionais entre 2019 e 2020, capturados a cada 20 segundos durante rodadas válidas.
- **Atributos:** Informações sobre jogadores, economia, equipamentos, granadas, mapas e status da bomba.

---

## Etapas Desenvolvidas

### 1. Definição do Problema
- Formulação de hipóteses sobre variáveis que influenciam o vencedor do round.
- Definição do tipo de problema: aprendizado supervisionado (classificação).

### 2. Análise Exploratória de Dados (EDA)
- Identificação de valores inválidos e inconsistências.
- Visualizações com histogramas, boxplots, gráficos de barras e correlação.
- Validação e discussão de hipóteses com base em evidências visuais e estatísticas.

### 3. Limpeza e Balanceamento
- Remoção de valores fora dos limites plausíveis (ex: saúde > 500).
- Balanceamento da distribuição de mapas por downsampling estratificado.

### 4. Engenharia de Atributos
- Criação de novas variáveis como "vida efetiva", "diferença de granadas", entre outras, com base em conhecimento do jogo.

### 5. Encoding e Padronização
- Aplicação de One-Hot Encoding em variáveis categóricas.
- Padronização de variáveis numéricas com `StandardScaler`, evitando vazamento de dados.

---

## Hipóteses Investigadas

- O número de jogadores vivos tem forte influência sobre o resultado da rodada.
- Ter a bomba plantada tende a favorecer a equipe Terrorista.
- Ter uma AWP no time pode ser decisivo.
- A economia da equipe (dinheiro disponível) impacta nas chances de vitória.
- A quantidade de granadas no final da rodada pode ser um fator tático decisivo.
- Alguns mapas oferecem vantagem tática para um dos lados (CT ou T).

---

## Próximos Passos

- Treinamento e avaliação de modelos de classificação.
- Interpretação de importância das variáveis.
- Ajuste de hiperparâmetros e seleção de algoritmos.
- Análise de desempenho com métricas como acurácia, F1-score e matriz de confusão.

---

## Autor

Pedro Gateira L. Dias  
[LinkedIn](https://www.linkedin.com/in/pedrogldias/)
