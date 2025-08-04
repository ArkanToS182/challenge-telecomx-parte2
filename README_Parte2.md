
# 📘 Challenge TelecomX - Parte 2
## Modelos Preditivos para Churn

Este documento resume a segunda parte do projeto Challenge TelecomX, focada na construção de **modelos preditivos** para identificar clientes com maior risco de evasão (churn).

---

## 📌 Etapas do Projeto

1. **Importação dos Dados Tratados**  
   - Utilização do dataset `dados_tratados.csv` gerado na Parte 1.  

2. **Pré-Processamento**
   - Remoção de colunas irrelevantes (ex.: `customerid`).
   - Encoding de variáveis categóricas via One-Hot Encoding (se necessário).
   - Verificação e balanceamento de classes (SMOTE e class_weight).
   - Normalização / padronização (quando aplicável).

3. **Análise Exploratória**
   - Verificação da proporção de churn.
   - Análise de correlação das variáveis.
   - Análises direcionadas: `tenure` x churn e `charges.total` x churn.

4. **Modelagem Preditiva**
   - **Regressão Logística (com normalização)**: interpretável e eficaz para classificação binária.
   - **Random Forest (sem normalização)**: robusto e capaz de lidar com não linearidades.
   - Comparação das métricas principais: Acurácia, Precisão, Recall e F1-score.

5. **Avaliação e Interpretação**
   - Matrizes de confusão e relatórios de métricas.
   - Comparação gráfica das métricas entre os modelos.
   - Importância das variáveis com Random Forest e análise de coeficientes com Regressão Logística.

6. **Conclusões e Recomendações**
   - Clientes com contratos curtos e baixo gasto apresentam maior risco de churn.
   - Contratos mensais e pagamentos via cheque eletrônico estão associados a maior evasão.
   - Random Forest apresentou melhor desempenho geral, embora com leve indício de overfitting.
   - Regressão Logística mostrou resultados equilibrados e interpretáveis.

---

## 💡 Recomendações de Negócio

1. **Retenção de clientes novos**: foco em contratos nos primeiros meses.
2. **Incentivo a contratos de longo prazo**.
3. **Pacotes especiais para clientes de baixo gasto**.
4. **Estímulo a métodos de pagamento automáticos**.
5. **Monitoramento contínuo do churn** via modelos preditivos.

---

## ⚙️ Próximos Passos Técnicos

- Testar modelos avançados como **XGBoost** ou **LightGBM**.  
- Realizar **tuning de hiperparâmetros** (GridSearchCV/RandomizedSearchCV).  
- Implementar o modelo em pipeline de monitoramento contínuo.

---

📌 **Autor:** arkantos182  
📅 **Ano:** 2025  
