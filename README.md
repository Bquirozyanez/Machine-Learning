# Proyecto de Machine Learning

**Para una correcta visualización y revisión del proyecto, se recomienda seguir los siguientes pasos:**
1. Abrir el archivo "Examen_Machine.ipynb" disponible en este repositorio.
2. Utilizar el botón “Open in Colab” para visualizar el notebook en Google Colab, donde se encuentran los resultados, tablas y visualizaciones ya ejecutadas.


# Análisis de Comportamiento Comercial con Machine Learning

Este repositorio contiene un análisis exhaustivo de Machine Learning diseñado para identificar patrones y predecir comportamientos comerciales en una base de datos de clientes (*Base_clientes_Monopoly*).
El proyecto abarca el ciclo completo de ciencia de datos: desde la carga y limpieza, pasando por el preprocesamiento y codificación de variables, hasta la implementación y evaluación de modelos supervisados y no supervisados.

## Objetivo del Proyecto

El objetivo principal es aplicar técnicas de **Inteligencia Artificial** para segmentar clientes y predecir clasificaciones, permitiendo una toma de decisiones basada en datos. Se busca comparar el rendimiento de múltiples algoritmos para determinar cuál se ajusta mejor a la naturaleza del negocio.

## Tecnologías y Librerías

El proyecto fue desarrollado en **Python 3** utilizando las siguientes librerías clave:

* **Manipulación de Datos:** `Pandas`, `NumPy`.
* **Visualización:** `Matplotlib`, `Seaborn`.
* **Machine Learning:** `Scikit-learn`.
* **Preprocesamiento:** `Category Encoders` (Target Encoder), `SimpleImputer`.

## Modelos Implementados

Se exploraron diversos enfoques para asegurar la robustez del análisis:

### 1. Clasificación Supervisada
Se entrenaron y evaluaron modelos para predecir categorías objetivo:
* **K-Nearest Neighbors (KNN)**
* **Árboles de Decisión** (Criterios Gini y Entropía)
* **Random Forest**
* **Regresión Logística**

### 2. Clustering (No Supervisado)
Se aplicaron técnicas de agrupamiento para descubrir segmentos naturales en los datos:
* **K-Means** (Seleccionado como el mejor modelo).
* **DBSCAN**
* **Clustering Jerárquico**

Además, se utilizaron técnicas de reducción de dimensionalidad como **PCA** (Análisis de Componentes Principales).

## Resultados Destacados

Tras evaluar las métricas de desempeño (Inercia, Silhouette Score y el método del codo), se determinó que **K-Means** fue el algoritmo no supervisado más efectivo para este conjunto de datos, ofreciendo una segmentación clara y métricas cuantitativas superiores en comparación con DBSCAN y el Clustering Jerárquico.

## Estructura del Repositorio

* `Examen_Machine.ipynb`: Jupyter Notebook principal con todo el código, visualizaciones y análisis.
* `Base_clientes_Monopoly_fixed.csv`: Dataset utilizado para el entrenamiento y pruebas.

## Instalación y Uso

Para ejecutar este proyecto localmente, asegúrate de instalar las dependencias necesarias:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn category-encoders
