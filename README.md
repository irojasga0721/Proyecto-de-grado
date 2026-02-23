# ⚡ Predicción de la Demanda de Energía en Colombia (SIN) 2024-2030

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Econometría](https://img.shields.io/badge/Time%20Series-SARIMAX-success)
![Machine Learning](https://img.shields.io/badge/Machine%20Learning-Random%20Forest-orange)
![Status](https://img.shields.io/badge/Status-Completado-brightgreen)

## 📖 Descripción del Proyecto
Este repositorio contiene el trabajo de grado para la Especialización en Ciencia de Datos (UNAD). El proyecto aborda la necesidad crítica de proyectar la demanda de energía del Sistema Interconectado Nacional (SIN) en Colombia, un país con alta dependencia hidroeléctrica (70%).

Se realizó un análisis comparativo riguroso entre enfoques de **Machine Learning** (Random Forest, Gradient Boosting) y un modelo **Econométrico Multivariable** (SARIMAX), incorporando variables exógenas clave como la **Generación de Energía** y la **Precipitación**.

## 🛠️ Metodología Resumida
El proyecto se desarrolló en tres fases:
1. **Análisis Estructural (EDA):** Descomposición de la serie temporal, prueba Dickey-Fuller y análisis de correlación (Heatmap).
2. **Modelado:** Implementación de SARIMAX `(1, 0, 1) x (0, 0, 2, 12)` y modelos de Machine Learning con ingeniería de características (*Lags*).
3. **Evaluación Comparativa:** Medición del desempeño utilizando métricas de error (MAPE, R²) en validación cruzada temporal.

## 📊 Resultados Clave (El Ganador)
El modelo **SARIMAX** demostró una superioridad técnica abrumadora para capturar la estructura temporal y estacional frente a los modelos de caja negra, logrando un error porcentual mínimo:

| Modelo | MAPE (%) | R² |
| :--- | :---: | :---: |
| **SARIMAX (Ganador)** | **1.37%** | **0.992** |
| Random Forest | 3.43% | Negativo |
| Gradient Boosting | 3.04% | 0.095 |

### 📈 Pronóstico a 2030
Se proyecta un crecimiento sostenido de la demanda, estimando que superará la barrera de los **10,000 GWh mensuales** para el final de la década.

## 🚀 Cómo reproducir este proyecto
1. Clona este repositorio.
2. Instala las dependencias necesarias:
   `pip install -r requirements.txt`
3. Ejecuta el notebook principal: `Analisis_Prediccion_Demanda_SIN.ipynb`

## ✒️ Autor
* **Iván Darío Rojas Galvis** - *Estudiante Especialización en Ciencia de Datos - UNAD*
