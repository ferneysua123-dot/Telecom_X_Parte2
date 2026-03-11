# Telecom_X_Parte2
Machine_Learning
# 📊 Predicción de Abandono de Clientes (Churn) - TelecomX

Este proyecto aplica técnicas de **Machine Learning** para predecir la cancelación de servicios en una empresa de telecomunicaciones. El objetivo principal es identificar proactivamente a los clientes en riesgo para ejecutar estrategias de retención efectivas.

## 🚀 Resumen del Proyecto
El abandono de clientes (Churn) es uno de los mayores desafíos en el sector telco. En este análisis, procesamos datos de comportamiento contractual y financiero para construir un modelo predictivo capaz de detectar fugas antes de que ocurran.

### 🛠️ Tecnologías Utilizadas
*   **Lenguaje:** Python 3.x
*   **Librerías Clave:** `pandas`, `scikit-learn`, `imblearn` (SMOTE), `seaborn`, `matplotlib`.
*   **Modelos Evaluados:** Regresión Logística (Normalizada) y Random Forest.

## 📈 Hallazgos Principales (Insights)
Tras el Análisis Exploratorio de Datos (EDA) y la evaluación de importancia de variables, determinamos que:
1.  **Tipo de Contrato:** Los clientes con contrato **Mes a mes** tienen la correlación positiva más alta con el abandono (**0.39**).
2.  **Permanencia:** La antigüedad del cliente actúa como un factor protector; a mayor permanencia, menor riesgo de fuga.
3.  **Cargos Mensuales:** El gasto elevado es un disparador secundario de abandono, especialmente si el cliente no cuenta con servicios de valor agregado como Soporte Técnico.

## 🧪 Metodología y Modelado
Dado que el dataset presentaba un fuerte desbalance de clases, se aplicaron las siguientes estrategias:
*   **Balanceo de Datos:** Se utilizó **SMOTE** (Synthetic Minority Over-sampling Technique) para equilibrar la clase minoritaria (clientes que abandonan).
*   **Preprocesamiento:** Se aplicó **StandardScaler** para normalizar variables numéricas, permitiendo que modelos lineales como la Regresión Logística compitieran equitativamente.
*   **Optimización de Umbral:** Se ajustó el umbral de decisión a **0.3** para priorizar el **Recall**, capturando así la mayor cantidad de desertores posibles.

## 🏆 Resultados del Modelo Ganador
El modelo de **Regresión Logística con Normalización** superó al Random Forest en la detección de fugas:


| Métrica | Resultado |
| :--- | :--- |
| **AUC (Área bajo la curva)** | **0.79** |
| **Recall (Sensibilidad)** | **74%** |
| **F1-Score** | **0.60** |

> **Conclusión técnica:** El modelo es capaz de identificar correctamente al 74% de los clientes que realmente abandonarán, permitiendo al equipo de ventas actuar a tiempo.

## 📂 Estructura del Repositorio
*   `TelecomX_PARTE__II.ipynb`: Notebook principal con el flujo completo de limpieza, balanceo, modelado y evaluación.
*   `data/`: (Opcional) Dataset utilizado para el entrenamiento.

---
Generado como parte del análisis avanzado de Machine Learning para TelecomX.
