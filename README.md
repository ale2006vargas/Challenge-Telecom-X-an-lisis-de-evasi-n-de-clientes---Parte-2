# Challenge-Telecom-X-an-lisis-de-evasi-n-de-clientes---Parte-2

# 📊 Análisis de Cancelación de Clientes - Telecom X

Este proyecto analiza los factores que más influyen en la cancelación (*churn*) de clientes de una empresa de telecomunicaciones y propone estrategias de retención basadas en modelos de *machine learning*.

## 📌 Objetivo
Identificar patrones en los datos que permitan:
- Predecir qué clientes tienen alta probabilidad de cancelar.
- Comprender qué variables impulsan esta decisión.
- Implementar acciones para reducir la tasa de churn.

## 📂 Contenido del repositorio
- `datos_tratados.csv`: Dataset preprocesado para entrenamiento y evaluación.
- `notebooks/`: Jupyter Notebooks con el flujo de análisis.
- `modelos/`: Scripts de entrenamiento y evaluación de distintos algoritmos.
- `README.md`: Este documento.

## ⚙️ Metodología
1. **Preprocesamiento**:  
   - Balanceo de clases con SMOTE.  
   - Codificación One-Hot para variables categóricas.  
   - Escalado de variables numéricas.
   
2. **Modelos aplicados**:
   - Regresión Logística.
   - Random Forest.
   - (Opcional) SVM, KNN, XGBoost.

3. **Evaluación**:
   - Métricas: Accuracy, Precision, Recall, F1, ROC AUC.
   - Análisis de importancia de variables: coeficientes estandarizados, permutación, Gini.

## 📈 Resultados clave
- Tasa de churn: **25,7 %**.
- Variables más influyentes:
  - **Positivas (aumentan churn)**: `ServicioInternet_fiber optic`, `MetodoPago_electronic check`, `CobroMensual`.
  - **Negativas (reducen churn)**: `AntiguedadMeses`, `TipoContrato_two year`, `MetodoPago_credit card (automatic)`.

## 🎯 Estrategias de retención sugeridas
1. Fidelización temprana en contratos mensuales.
2. Incentivos para migrar a pagos automáticos.
3. Optimización de planes de clientes de fibra óptica.
4. Programas de lealtad por antigüedad.
5. Alertas preventivas para cargos altos.

