# Análisis de Morosidad Bancaria — Sistema Financiero

## Descripción

Este proyecto analiza datos históricos de clientes bancarios del sistema financiero peruano con el objetivo de identificar patrones asociados a la morosidad crediticia. A través de un proceso de limpieza, preprocesamiento y modelamiento de datos, se construye un modelo de clasificación capaz de predecir si un cliente es propenso a caer en mora, aportando una herramienta objetiva para la toma de decisiones crediticias.

## Objetivo

Desarrollar un modelo de Machine Learning que permita al banco anticipar la morosidad de un cliente a partir de sus características financieras y demográficas, reduciendo el riesgo crediticio y optimizando la asignación de créditos.

## Dataset

El dataset fue obtenido de [BankDefaultAnalysis](https://www.kaggle.com/datasets/luishcaldernb/morosidad) y contiene 14 variables con información financiera, demográfica y crediticia de clientes bancarios peruanos, entre las que destacan el score crediticio, nivel de ahorro, atraso histórico, clasificación SBS y nivel educativo.

## Tecnologías y Librerías

- **Pandas** — manipulación y análisis de datos
- **Matplotlib / Seaborn** — visualización de datos
- **KNNImputer** — imputación de valores faltantes
- **OneHotEncoder / StandardScaler** — preprocesamiento de variables
- **RandomForestClassifier** — modelo de clasificación
- **Scikit-learn Metrics** — evaluación del modelo (Accuracy, Precision, Recall, F1, ROC-AUC)

## Modelo Final

Se entrenó un modelo de **Random Forest** con `class_weight='balanced'` para compensar el desbalance moderado de clases (~7:3), garantizando que el modelo no favorezca la clase mayoritaria durante el entrenamiento.