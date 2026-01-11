# 📊 Predicción de cancelaciones de clientes con Machine Learning

Este proyecto presenta un modelo de clasificación diseñado para detectar cancelaciones de clientes, utilizando un enfoque de **Stacking** calibrado con **Regresión Logística** como meta-modelo.  
Se integraron algoritmos de última generación: **CatBoost, LightGBM y XGBoost**.

---

## 📐 Metodología
- **Preparación de datos**  
  - Limpieza de registros nulos y outliers.  
  - Codificación de variables categóricas con *One-Hot Encoding*.  
  - Normalización de variables numéricas para mejorar estabilidad.  

- **División del dataset**  
  - Train/Test split en proporción 80/20.  
  - Validación cruzada (*k-fold*) para asegurar robustez.  

- **Modelos base**  
  - CatBoost, LightGBM y XGBoost optimizados con *GridSearchCV*.  
  - Selección de hiperparámetros clave: learning rate, depth, n_estimators.  

- **Modelo final (Stacking)**  
  - Regresión Logística como meta-modelo.  
  - Combinación de predicciones para reducir sesgo y mejorar capacidad discriminativa.  

---

## 🚀 Resultados principales
- **AUC-ROC:** 0.8387 → Alta capacidad para distinguir clientes que cancelan vs. los que permanecen.  
- **Precisión:** 78.18% → Minimiza falsos positivos en campañas de retención.  
- **Recall:** 0.78 (umbral ajustado) → Detecta correctamente la mayoría de clientes que cancelan.  
- **F1-score:** 0.64 → Buen equilibrio entre precisión y recall.  

---

## ✨ Contribuciones del modelo
- Alta capacidad discriminativa en la detección de cancelaciones.  
- Equilibrio sólido entre precisión y sensibilidad.  
- Flexibilidad para adaptarse a distintas estrategias de retención.  
- Se consolidó como el modelo más robusto del proyecto, recomendado para implementación.  

---

## 📌 Interpretación técnica
El stacking permitió reducir sesgos individuales y mejorar la generalización.  
La calibración del umbral ajustó la sensibilidad del modelo según la estrategia de negocio, logrando un balance entre **detección temprana de cancelaciones** y **minimización de falsas alarmas**.  

---

⭐ **Conclusión:** Este trabajo demuestra cómo la integración de múltiples algoritmos potencia la efectividad en proyectos de predicción y retención de clientes.  

