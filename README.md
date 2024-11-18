# Predicción de Abandono de Clientes en el Banco

El objetivo de este proyecto fue entrenar un modelo de *machine learning* para predecir el posible abandono de clientes del banco, alcanzando un *score* F1 de al menos 0.59.  

## Descripción del Proyecto

El proyecto incluyó el preprocesamiento de datos, la evaluación de diferentes modelos de clasificación y la optimización de un modelo seleccionado. Las tareas realizadas fueron:  

1. **Preprocesamiento de Datos:**  
   - Estandarización de las columnas de características utilizando `StandardScaler`.  
   - Codificación de columnas categóricas mediante técnicas como *One-Hot Encoding (OHE)* y *Ordinal Encoder*.  

2. **Evaluación Inicial de Modelos:**  
   - Comparación del rendimiento de diferentes algoritmos de clasificación, incluyendo:  
     - Árbol de Decisión  
     - Bosque Aleatorio  
     - Regresión Logística  
   - Métrica principal evaluada: Exactitud de la predicción (*accuracy*).
   - Pruebas de Cambio de Umbral, Sbmuestreo y Sobre Muestreo para verificar Recall y F1.  

3. **Optimización del Modelo Seleccionado:**  
   - Uso de un modelo de Bosque Aleatorio con técnicas de balanceo de clases:  
     - Submuestreo (*undersampling*).      
   - Análisis y mejora del *score* F1 en el conjunto de validación.  

## Resultados Principales

- Se logró un *score* F1 de **0.59** en el conjunto de validación utilizando un Bosque Aleatorio con submuestreo, cumpliendo con el objetivo planteado.  
- Complementariamente, se evaluó el modelo utilizando el *Area Under ROC Curve (AUC-ROC)* para analizar su desempeño.  

## Herramientas y Tecnologías Utilizadas

El proyecto fue desarrollado en Python utilizando las siguientes bibliotecas:  

- **Pandas:** Manipulación y limpieza de datos.  
- **NumPy:** Operaciones matemáticas y manejo de matrices.  
- **Scikit-learn:**  
  - Algoritmos de clasificación.  
  - Técnicas de preprocesamiento (escaladores y codificadores).  
  - Evaluación de modelos mediante métricas como F1, Recall, y AUC-ROC.  

## Cómo Ejecutar el Proyecto

1. Clonar este repositorio:  
   ```bash
   git clone https://github.com/dsc530/banco.git
