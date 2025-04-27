# Temperature_Prediction
Este proyecto implementa un modelo de red neuronal LSTM (Long Short-Term Memory) para predecir la temperatura promedio diaria en Nueva York utilizando datos históricos.
El modelo es entrenado con datos desde el año 2000 hasta aproximadamente 2022, utilizando PyTorch y PyTorch Lightning.
Características principales

Preprocesamiento de datos:

Carga y limpieza de datos de temperaturas históricas.
Creación de secuencias temporales para el entrenamiento (ventanas de 7 días para predecir el día siguiente).
División en conjuntos de entrenamiento (70%) y prueba (30%) preservando el orden temporal.

Modelo LSTM:

Arquitectura simple con una capa LSTM y una capa lineal para la predicción.
Pérdida MSE (Error Cuadrático Medio) como métrica de optimización.
Optimizador Adam con tasa de aprendizaje de 0.001.

Entrenamiento:

100 épocas de entrenamiento.
Batch size de 64.
Semilla fijada para reproducibilidad (42).


Mejoras futuras:
Ajuste de hiperparámetros
Incorporación de más características meteorológicas
Implementación de atención para mejorar las predicciones

Archivos necesarios:
temperaturas_NEWYORK_2.csv: Dataset de temperaturas
