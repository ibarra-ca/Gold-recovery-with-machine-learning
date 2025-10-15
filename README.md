# 🪙 Gold Recovery with Machine Learning

El objetivo fue **simular y optimizar el proceso de recuperación de oro a partir del mineral**, aplicando técnicas de machine learning para mejorar la eficiencia del proceso industrial.

👉 [**Ver análisis completo**](https://ibarra-ca.github.io/Gold-recovery-with-machine-learning/)

---

## 🎯 Objetivo del proyecto
Predecir con la mayor precisión posible:
1. **La recuperación del concentrado "rougher"**, etapa intermedia del proceso.  
2. **La recuperación final del concentrado**, etapa final del proceso.

Estas predicciones permiten identificar ineficiencias en la planta y optimizar la recuperación de oro, reduciendo pérdidas y mejorando la rentabilidad del proceso.

---

## 🧪 Metodología y pasos realizados

### 1️⃣ Preparación y exploración de datos
- Limpieza y transformación de datos con `pandas` y `numpy`.
- Análisis exploratorio para comprender las etapas del proceso y la relación entre las variables físicas y químicas.
- Evaluación de la calidad de los datos y tratamiento de valores faltantes.

### 2️⃣ Feature Engineering
- Selección de variables relevantes de los datasets *train*, *test* y *full*.
- Normalización de columnas numéricas.
- Análisis de correlaciones y reducción de variables redundantes.
- División temporal de los datos para evitar fugas de información.

### 3️⃣ Modelado predictivo
- Entrenamiento de modelos de regresión para estimar las tasas de recuperación:
  - **Regresión Lineal**
  - **Random Forest Regressor**
  - **Gradient Boosting Regressor**
- Comparación del desempeño de los modelos mediante validación cruzada.

### 4️⃣ Métrica de evaluación
Se utilizó la métrica **sMAPE** (*Symmetric Mean Absolute Percentage Error*) como indicador principal del rendimiento.  
Esta métrica es especialmente útil en contextos donde los valores pueden variar en órdenes de magnitud, ya que equilibra el error relativo en ambas direcciones.

### 5️⃣ Resultados
- El modelo de **Random Forest** obtuvo los mejores resultados en términos de precisión y estabilidad.
- Se logró reducir significativamente el error de predicción en comparación con el baseline.
- Se generaron visualizaciones para comparar los valores reales y predichos en cada etapa del proceso.

---

## 📊 Tecnologías utilizadas
| Categoría | Herramientas |
|------------|---------------|
| Lenguaje principal | Python |
| Librerías de análisis | Pandas · NumPy · Matplotlib · Seaborn |
| Modelado predictivo | Scikit-learn · XGBoost |
| Métricas y evaluación | sMAPE · MAE · R² |
| Entorno | Jupyter Notebook |

---

## 📈 Visualizaciones
El análisis incluye gráficos interactivos que permiten explorar:
- Distribuciones de recuperación de oro.
- Comparaciones entre etapas rougher y final.
- Evaluación del desempeño de los modelos.  

🔗 Puedes visualizarlo en: [**ibarra-ca.github.io/Gold-recovery-with-machine-learning**](https://ibarra-ca.github.io/Gold-recovery-with-machine-learning/)

---

## 🧩 Conclusiones
- Se demostró que los modelos de *machine learning* pueden **predecir eficientemente la recuperación de oro** con base en parámetros físicos y químicos del proceso.  
- Las técnicas de ingeniería de características y evaluación de modelos fueron clave para optimizar los resultados.
- El enfoque es escalable a otros procesos metalúrgicos o de extracción.

---

## 🚀 Aprendizajes clave
- Implementación práctica de métricas personalizadas (sMAPE).  
- Manejo de datos industriales con múltiples fuentes y etapas.  
- Comparación de diferentes algoritmos de regresión bajo un marco de validación consistente.  
- Presentación clara de resultados mediante dashboards y visualizaciones.

---

📘 **Autor:** Carlos Ibarra  
🔗 [Perfil de GitHub](https://github.com/ibarra-ca) · [LinkedIn](https://www.linkedin.com/in/carlos-armado-ibarra-del-ángel)  
🗺️ *Proyecto desarrollado como parte del programa de Ciencia de Datos de TripleTen.*
