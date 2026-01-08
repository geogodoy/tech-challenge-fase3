# Checklist de Validação Final - Tech Challenge Fase 3

Use este checklist ao finalizar o projeto para garantir que **todos** os requisitos obrigatórios foram cumpridos e para validar se você dominou os conceitos técnicos aplicados.

---

## ✅ 1. Requisitos Obrigatórios (Entregáveis)

### Repositório e Código
- [ ] O código completo está organizado em um repositório (GitHub) ou Google Colab?
- [ ] O notebook roda de ponta a ponta sem erros ("Restart Kernel & Run All")?
- [ ] O arquivo `requirements.txt` ou célula de instalação de bibliotecas está presente?

### Vídeo de Apresentação
- [ ] O vídeo tem entre **5 a 10 minutos**?
- [ ] O vídeo cobre:
    - [ ] Introdução ao problema.
    - [ ] Exploração dos dados (principais insights).
    - [ ] Resultados da modelagem supervisionada e não supervisionada.
    - [ ] Conclusões finais.

---

## 🔍 2. Exploração de Dados (EDA)

- [ ] **Estatísticas Descritivas:** Foram geradas médias, medianas e desvios padrões das variáveis principais?
- [ ] **Visualizações:** Existem gráficos que trazem insights (ex: histogramas de atrasos, gráficos de barra por companhia/aeroporto)?
- [ ] **Tratamento de Dados:**
    - [ ] Valores ausentes (NaNs) foram tratados (removidos ou imputados)?
    - [ ] A estratégia escolhida para nulos foi justificada?

---

## 🤖 3. Modelagem Supervisionada (Classificação ou Regressão)

- [ ] **Definição do Problema:** Ficou claro se é Classificação (Prever Se Atrasou: Sim/Não) OU Regressão (Prever Quanto Tempo)?
- [ ] **Comparação:** Pelo menos **dois (2)** algoritmos diferentes foram treinados e comparados?
- [ ] **Métricas:** As métricas adequadas foram utilizadas?
    - *Se Classificação:* Acurácia, Precision, Recall, F1-Score?
    - *Se Regressão:* RMSE, MAE, R²?
- [ ] **Divisão de Dados:** Os dados foram separados em Treino e Teste?

---

## 🧠 4. Modelagem Não Supervisionada

- [ ] **Técnica Aplicada:** Foi utilizada pelo menos **uma** abordagem (Clusterização OU Redução de Dimensionalidade/PCA)?
- [ ] **Visualização:** Os resultados foram mostrados em gráficos (ex: Scatterplot dos clusters ou componentes do PCA)?
- [ ] **Interpretação:** Existe uma explicação textual do que os clusters ou componentes representam? (ex: "Este grupo representa voos longos com pouco atraso").

---

## 📊 5. Conclusão e Crítica

- [ ] **Conclusões:** As principais descobertas foram resumidas?
- [ ] **Limitações:** Foi discutido onde o modelo falha ou o que faltou nos dados (ex: falta de dados meteorológicos)?
- [ ] **Próximos Passos:** Foram propostas melhorias futuras?

---

## 💡 6. Auto-Validação de Aprendizado (Você entendeu o que fez?)

*Responda mentalmente "Sim" para validar seu domínio técnico.*

### Sobre os Dados
- [ ] Entendi a diferença entre `SCHEDULED_DEPARTURE` e `DEPARTURE_TIME` para calcular o atraso?
- [ ] Sei explicar quais variáveis foram mais importantes para o modelo (Feature Importance)?

### Sobre Supervisionado
- [ ] Sei explicar por que escolhi a métrica principal (ex: "Escolhi Recall porque queria evitar Falsos Negativos")?
- [ ] Sei dizer se meu modelo teve Overfitting ou Underfitting analisando os resultados de treino vs teste?
- [ ] Entendi a diferença entre os dois algoritmos que comparei?

### Sobre Não Supervisionado
- [ ] Se usei K-Means: Sei explicar como escolhi o número de clusters (`K`)? (Ex: Método do Cotovelo).
- [ ] Se usei PCA: Entendo que ele reduziu as colunas mantendo a variância (informação) dos dados?

### Sobre o Processo
- [ ] Consigo explicar o fluxo completo (Dados -> Limpeza -> Modelos -> Resultado) para uma pessoa leiga em 1 minuto?

