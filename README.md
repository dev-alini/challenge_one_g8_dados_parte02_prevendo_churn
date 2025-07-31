# challenge_one_g8_dados_parte02_prevendo_churn
Projeto criado para continuidade do Telecom X Evasão de Clientes

# 📘 Análise Preditiva de Evasão de Clientes

## 🎯 Missão
Antecipar a evasão de clientes usando modelos de machine learning, permitindo que a empresa aja proativamente para reduzir o churn e melhorar a retenção.

---

## 📌 Objetivos
- Preparação dos dados (limpeza, encoding, normalização).
- Análise de correlação e seleção de variáveis.
- Treinamento de modelos preditivos.
- Avaliação com métricas clássicas (accuracy, recall, f1-score, etc).
- Interpretação dos resultados e proposta de ações de retenção.

---

## 📊 Proporção de Classes

| Classe         | Quantidade | Proporção (%) |
|----------------|------------|----------------|
| Clientes Ativos (0) | 5174       | 73.46%         |
| Clientes Evadiram (1) | 1869       | 26.54%         |

> A proporção é levemente desbalanceada, o que requer atenção na modelagem.

---

## 📈 Modelos Treinados

| Modelo                     | Acurácia | Precisão (Churn) | Recall (Churn) | F1-score |
|---------------------------|----------|------------------|----------------|----------|
| Regressão Logística       | 0.7345   | 0.0000           | 0.0000         | 0.0000   |
| Regressão (com balanceamento) | 0.5000 | 0.27             | 0.53           | 0.36     |
| Random Forest             | 0.7071   | 0.27             | 0.06           | 0.10     |
| Random Forest (balanceado)| 0.7061   | 0.26             | 0.06           | 0.09     |

---

## 🔍 Variáveis Mais Relevantes

### 🎯 Top Variáveis - Random Forest

<img width="1979" height="1180" alt="image" src="https://github.com/user-attachments/assets/8395b9bb-a42a-46bd-b1e6-0f2b6babb0e8" />


### 🧠 Top Coeficientes - Regressão Logística

<img width="1981" height="1180" alt="image" src="https://github.com/user-attachments/assets/765d9363-132b-44a5-bc04-4605876ad320" />


---

## 🔑 Fatores que mais influenciam a evasão

- **Charges.Total**: Clientes com alto valor total gasto tendem a evadir mais.
- **Charges.Monthly**: Faturas mensais elevadas também indicam risco.
- **Tenure**: Clientes recentes são mais voláteis.
- **Contratos mensais**: Forte indicador de evasão.
- **Uso de serviços digitais (Streaming, Fiber Optic)**: Indica menor fidelização.

---

## 💡 Estratégias de Retenção

| Fator de Risco        | Estratégia de Retenção                                                |
|------------------------|----------------------------------------------------------------------|
| Contrato mensal        | Oferecer migração para contrato anual com benefícios.                |
| Alto valor de fatura   | Oferecer programas de fidelidade ou cashback.                        |
| Cliente novo (baixo tenure) | Ofertas especiais nos primeiros 3 meses, suporte proativo.           |
| Clientes digitais       | Programas de engajamento digital e satisfação com serviços.         |

---

## ✅ Conclusão
Os modelos revelaram padrões relevantes para identificar clientes propensos à evasão. Estratégias segmentadas podem ser aplicadas para reduzir o churn e aumentar o lifetime value dos clientes.


