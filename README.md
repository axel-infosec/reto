# 📊 Challenge: Análisis de Riesgo Crediticio y Algoritmia

Este repositorio contiene la solución técnica para el desafío de Datos y Lógica. El proyecto está dividido en la resolución de problemas de algoritmia/SQL y la implementación de un *pipeline* completo de Machine Learning para predecir el riesgo crediticio de una cartera de clientes.

## 🎯 Objetivo del Proyecto
Desarrollar un sistema de evaluación de riesgo robusto utilizando el dataset *Statlog (German Credit Data)*, minimizando el impacto financiero de los falsos negativos (aprobar créditos a clientes morosos) mediante la optimización de umbrales en modelos de clasificación, y descubrir perfiles de clientes ocultos en los datos mediante aprendizaje no supervisado.

## 🗂️ Estructura del Análisis

El proyecto (desarrollado en Jupyter Notebook) se divide en dos secciones principales:

### Sección 1: Lógica Babilónica y Consultas SQL
* **Algoritmia:** Implementación y análisis de complejidad ($O(g)$) del Algoritmo Babilónico para el cálculo de raíces.
* **Recursividad:** Desarrollo comparativo de algoritmos factoriales (iterativo vs. recursivo) priorizando la eficiencia de memoria.
* **Integridad de Datos (SQL):** Diseño de consultas transaccionales (`HAVING COUNT`) para la identificación y depuración de registros duplicados en bases de datos.

### Sección 2: Machine Learning y Visión de Negocio
* **Análisis No Supervisado (Segmentación):** * Reducción de dimensionalidad con **PCA**.
  * Creación de perfiles de clientes con **K-Means**, identificando 3 segmentos clave de negocio: *Jóvenes/Iniciación, Estabilidad Intermedia y Premium/Alto Valor*.
* **Análisis Supervisado (Predicción de Riesgo):** * Entrenamiento y comparativa entre **Regresión Logística** y **Random Forest**.
  * Optimización estratégica del umbral de decisión (*threshold* a 0.7) en Random Forest, logrando un **Recall del 80%** en la detección de posibles morosos, priorizando la protección del capital de la empresa.

## 🛠️ Stack Tecnológico
* **Lenguaje:** Python 3.12+
* **Manipulación de Datos:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Visualización:** Matplotlib, Seaborn
* **Entorno:** Jupyter Notebook

## 🚀 Cómo ejecutar el proyecto

1. Clona este repositorio:
   ~~~bash
   git clone https://github.com/axel-infosec/reto.git
   ~~~
2. Instala las dependencias necesarias:

    ~~~Bash
    pip install pandas numpy scikit-learn matplotlib seaborn jupyter
    ~~~
3. Ejecuta Jupyter Notebook y abre el archivo principal:

    ~~~Bash
    jupyter notebook reto.ipynb
    ~~~

🧠 Hallazgos Clave para Negocio
La vulnerabilidad está en la exposición: El plazo (Duration) y el monto (Credit amount) son los factores predictivos más fuertes de morosidad.

Priorización de Liquidez: El modelo final sacrifica exactitud global (Accuracy) para maximizar la detección preventiva de riesgo, funcionando como un escudo financiero para el otorgamiento de créditos.

Autor: Axel Emmanuel Angeles Rodriguez

Contacto: axel.emmanuel.angeles.rodriguez@gmail.com
