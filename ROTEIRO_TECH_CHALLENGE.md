# Roteiro do Tech Challenge - Fase 3 (Machine Learning)

Este roteiro divide o desafio em 6 fases lógicas, baseadas no pipeline de Data Science e nos conteúdos estudados. Utilize esta estrutura para criar cards no Trello, Jira ou GitHub Projects.

---

## 📋 1. Setup e Entendimento do Problema
*Fase inicial para organizar o ambiente e compreender os dados disponíveis.*

- [ ] **Configuração do Ambiente e Repositório**
    - Criar repositório no GitHub (requisito de entrega).
    - Configurar ambiente Python (Jupyter Notebook/Lab ou Google Colab).
    - Criar arquivo `requirements.txt` com as bibliotecas iniciais (`pandas`, `numpy`, `matplotlib`, `seaborn`, `scikit-learn`).

- [ ] **Carga e Fusão de Dados (Data Ingestion)**
    - Carregar `flights.csv`, `airlines.csv` e `airports.csv`.
    - Consultar o `dicionario.png` para entender as colunas (identificar numéricas, categóricas e targets como `DEPARTURE_DELAY`).
    - Realizar o merge dos datasets:
        - Unir `flights` + `airlines` (para obter nomes das companhias).
        - Unir `flights` + `airports` (para obter dados de origem/destino).

- [ ] **Definição do Escopo (Supervisionado)**
    - Decidir o objetivo principal (conforme `TECH CHALLENGE.txt`):
        - **Opção A (Classificação):** Prever SE vai atrasar (`SIM`/`NAO`). Sugestão: Criar coluna binária `is_delayed` (ex: atraso > 15 min = 1).
        - **Opção B (Regressão):** Prever O TEMPO do atraso (em minutos).

---

## 🔍 2. Análise Exploratória de Dados (EDA) e Pré-processamento
*Baseado em: `Aprendizado Supervisionado.txt` (Preparação de Dados) e `TECH CHALLENGE.txt` (Obrigatório).*

- [ ] **Limpeza de Dados (Data Cleaning)**
    - Verificar e tratar valores nulos (Missing Values).
    - Verificar duplicatas.
    - Analisar Outliers (ex: atrasos irreais ou erros de digitação) e decidir estratégia (remover/tratar).

- [ ] **Análise Estatística e Visualização**
    - Plotar distribuição da variável alvo (verificar balanceamento de classes).
    - Analisar correlações (Heatmap): Quais variáveis impactam mais (`TAX_OUT`, `WHEELS_OFF`, etc)?
    - Responder perguntas do desafio:
        - Quais aeroportos têm mais atrasos?
        - Existe sazonalidade (dias da semana, meses)?
        - Quais companhias aéreas atrasam mais?

- [ ] **Feature Engineering (Engenharia de Atributos)**
    - Criar variáveis derivadas (ex: "fim de semana", "período do dia").
    - Aplicar Encoding em categóricas (One-Hot Encoding, Label Encoding).
    - Aplicar Escalonamento (StandardScaler/MinMaxScaler) em numéricas.

---

## 🤖 3. Aprendizado Não Supervisionado
*Baseado em: `Aprendizado Nao Supervisionado.txt` e `TECH CHALLENGE.txt` (Obrigatório).*

- [ ] **Aplicação de PCA (Redução de Dimensionalidade)**
    - Aplicar PCA para visualização (2D/3D).
    - Analisar a variância explicada pelos componentes.
    - (Opcional) Usar dataset reduzido para modelos supervisionados.

- [ ] **Clusterização (K-Means)**
    - Definir objetivo: Agrupar Aeroportos, Rotas ou Companhias.
    - Aplicar Método do Cotovelo (Elbow Method) para definir `K`.
    - Rodar K-Means.
    - **Interpretação:** Analisar os centroides e dar "nomes" aos clusters (ex: "Aeroportos de Alto Tráfego e Atraso").

---

## 🧠 4. Aprendizado Supervisionado (Modelagem)
*Baseado em: `Aprendizado Supervisionado.txt` e `ML Avançado.txt`.*

- [ ] **Setup de Treino/Teste**
    - Dividir dados (`train_test_split`).
    - Definir Baseline (modelo simples para comparação).

- [ ] **Treinamento de Modelos (Mínimo 2)**
    - Treinar Modelo 1 (Ex: Regressão Logística ou Árvore de Decisão).
    - Treinar Modelo 2 (Ex: Random Forest, XGBoost ou SVM).
    - (Opcional) Redes Neurais (MLP).

- [ ] **Otimização e Validação Robusta**
    - Aplicar **Validação Cruzada (Cross-Validation)**.
    - Otimizar Hiperparâmetros (Grid Search/Random Search).

---

## 📊 5. Avaliação e Diagnóstico
*Baseado em: `ML Avançado.txt` (Diagnóstico) e `Aprendizado Supervisionado.txt` (Métricas).*

- [ ] **Análise de Métricas**
    - Classificação: Acurácia, Precision, Recall, F1-Score, Matriz de Confusão.
    - Regressão: RMSE, MAE, R².
    - Criar tabela comparativa.

- [ ] **Diagnóstico do Modelo**
    - Analisar Curvas de Aprendizado (Overfitting vs Underfitting).
    - Analisar Feature Importance (quais variáveis pesaram mais).

---

## 🏁 6. Entrega Final (Storytelling)
*Baseado em: `TECH CHALLENGE.txt` (Entregáveis).*

- [ ] **Consolidação das Conclusões**
    - Escrever conclusões no Notebook.
    - Discutir limitações e propor melhorias.
    - (Opcional) Mencionar como Sistemas de Recomendação poderiam ser aplicados futuramente.

- [ ] **Gravação e Entrega**
    - Gravar vídeo (5-10 min) explicando o pipeline e resultados.
    - Limpar e revisar o código final.
    - Submeter link do GitHub e Vídeo.

