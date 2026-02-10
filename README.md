# 📈 Análisis y Predicción de Stock de Apple (AAPL) mediante Machine Learning

Este proyecto aborda el ciclo de vida completo de un problema de **Data Science** aplicado a mercados financieros. El objetivo principal ha sido desarrollar un pipeline robusto de extracción, transformación y modelado de datos para predecir el comportamiento de las acciones de Apple.

## 👥 Autores
Proyecto realizado en el Grado de **Ciencia e Ingeniería de Datos** por:
* **Raúl Sánchez Ibáñez**
* **Juan José Pérez Romero**

## 🎯 Objetivo
Construir un modelo predictivo capaz de anticipar la tendencia de cierre (Subida/Bajada) de AAPL basándose estrictamente en patrones históricos y variables técnicas derivadas.

## ⚙️ Arquitectura y Metodología
El proyecto se estructura en fases clave de ingeniería de datos:

1.  **Extracción de Datos (Data Gathering):**
    * Automatización de descarga de datos bursátiles históricos mediante APIs financieras (`yfinance`).
    * Integración de datasets macroeconómicos y sectoriales.

2.  **Limpieza y Tratamiento (Data Wrangling):**
    * Detección y tratamiento de valores nulos y outliers en series temporales.
    * Normalización de datos para mejorar la convergencia de los modelos.
    * Gestión de tipos de datos y indexación temporal.

3.  **Feature Engineering (Ingeniería de Características):**
    * Creación manual de indicadores técnicos avanzados para enriquecer el dataset:
        * **Tendencia:** Medias Móviles Exponenciales (EMA), MACD.
        * **Momento:** RSI (Relative Strength Index).
        * **Volatilidad:** Bandas de Bollinger (BB_High, BB_Low).
    * Cálculo de lags (retardos) y deltas para capturar la temporalidad del mercado.

4.  **Modelado y Evaluación:**
    * Comparativa de algoritmos de clasificación: **Random Forest**, **Gradient Boosting** y **Support Vector Machines (SVM)**.
    * Validación cruzada (Time Series Split) para respetar la cronología de los datos.
    * Optimización de hiperparámetros para maximizar la precisión sin caer en *look-ahead bias*.

## 📊 Resultados
* Se identificaron las variables técnicas (RSI y MACD) con mayor poder predictivo sobre la acción.
* El modelo final logra generalizar el comportamiento del stock en periodos de volatilidad estándar, superando a estrategias base.

## 📂 Estructura del Repositorio
* `Preparación_datos.ipynb`: Scripts de ETL (Extracción, Transformación y Carga).
* `Análisis_Apple.ipynb`: Análisis Exploratorio de Datos (EDA), correlaciones y visualización de velas japonesas.
* `Entregable_Final.ipynb`: Entrenamiento de modelos, métricas de desempeño y backtesting.
* `MemoriaEML.pdf`: Documentación técnica detallada del proceso.

---
*Grado en Ciencia e Ingeniería de Datos - 2026*
