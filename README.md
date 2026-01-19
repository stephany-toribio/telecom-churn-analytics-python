# 🐍 Telecom Churn Analytics: Python & Machine Learning Pipeline

![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit-Learn](https://img.shields.io/badge/Scikit_Learn-Machine%20Learning-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=black)
![Status](https://img.shields.io/badge/Status-Completed-success?style=for-the-badge)

## 💼 Business Case & Context
En el competitivo sector de las telecomunicaciones, retener clientes es más rentable que adquirirlos. Este proyecto analiza un dataset de **3,333 clientes** para identificar factores de riesgo y construir un modelo predictivo.

**El Hallazgo Crítico:** Se detectó una tasa de abandono global del **14.5%**. Sin embargo, mediante análisis estadístico, descubrimos que ciertos segmentos (como usuarios con plan internacional) tienen una tasa de fuga alarmante superior al **40%**, lo que sugiere problemas graves en la propuesta de valor de productos específicos.

---

## 🔬 Metodología Técnica 

Este repositorio contiene un flujo de trabajo de Data Science completo (`.ipynb`), desde la ingesta de datos hasta la validación del modelo:

### 1. Exploratory Data Analysis (EDA)
Análisis profundo utilizando **Pandas, Matplotlib y Seaborn** para entender la distribución de las variables.
* **Matriz de Correlación:** Análisis de multicolinealidad entre variables de consumo (minutos vs cargos).
* **Análisis Bivariado:** Segmentación del Churn por Estado, Área y Planes contratados.

### 2. Feature Engineering & Preprocessing
* **Transformación de Variables:** Conversión de variables categóricas binarias (`Yes`/`No`) a formato numérico/booleano para ingesta del modelo.
* **Creación de Features:** Generación de nuevas métricas de consumo total para simplificar la dimensionalidad del modelo.

### 3. Machine Learning & Validation
Se implementó un modelo de clasificación supervisada para predecir la fuga:
* **Algoritmo:** **Random Forest Classifier**. Seleccionado por su robustez frente al overfitting y su capacidad para manejar datos no lineales.
* **Validación Rigurosa:** Se utilizó **Stratified K-Fold Cross Validation** para asegurar que el modelo sea estable y generalizable, evitando sesgos por desbalance de clases.
* **Feature Importance:** Extracción de las variables más influyentes en la decisión de abandono.

---

## 💡 Top 3 Insights de Negocio

El análisis de datos reveló patrones de comportamiento cruciales para la estrategia de retención:

* 🚩 **La "Regla de las 4 Llamadas":** Existe una correlación directa y crítica entre las llamadas a servicio al cliente y la fuga. Los clientes que realizan **más de 3 llamadas** al soporte tienen una probabilidad de abandono exponencialmente más alta.
    * *Acción:* Implementar alertas automáticas al Call Center cuando un cliente llame por tercera vez.
* 🚩 **La Paradoja del Plan Internacional:** Los clientes con Plan Internacional tienen una tasa de churn mucho mayor (**~42%**) comparada con los que no lo tienen (**~11%**).
    * *Acción:* Revisar la competitividad de las tarifas internacionales o la calidad de la conexión en el extranjero.
* 🚩 **Consumo vs Fuga:** Los usuarios con mayor consumo de minutos diurnos (`Total day minutes`) mostraron una tendencia ligeramente mayor al abandono, sugiriendo que los "Heavy Users" podrían estar buscando mejores tarifas en la competencia.

---

## 🛠️ Stack Tecnológico

* **Lenguaje:** Python 3.x
* **Manipulación de Datos:** Pandas, NumPy
* **Visualización:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (RandomForest, StratifiedKFold)
* **Entorno:** Jupyter Notebook / Google Colab

---

### 👤 Autor

**Stephany Marilyn Toribio Alvarado**
* *Data Analyst & Scientist*
* [LinkedIn](https://www.linkedin.com/in/stephany-marilyn-toribio-alvarado-47080b303/) | [Portafolio](https://stephany-toribio.github.io/MWeb/)
