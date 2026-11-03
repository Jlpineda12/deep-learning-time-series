# 📈 Time Series Forecasting with Recurrent Neural Networks (RNN & LSTM)

<div align="center">
  <img src="https://img.shields.io/badge/Domain-Deep%20Learning-blueviolet?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Framework-TensorFlow%20%2F%20Keras-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white" />
  <img src="https://img.shields.io/badge/Architecture-LSTM%20%26%20Bi--LSTM-3b82f6?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Notebook-Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" />
</div>

<br/>

Este proyecto implementa y compara experimentalmente diversas arquitecturas de **Redes Neuronales Recurrentes y Convolucionales** para la predicción de secuencias temporales multivariables en datos climáticos (Jena Climate Dataset). El objetivo es modelar dependencias a corto y largo plazo para pronosticar variaciones de temperatura.

---

## 🔬 Arquitecturas Comparadas

1. **Perceptrón Multicapa (MLP)**:
   - Modelo base (Baseline) con capas densas para cuantificar la capacidad de representación sin memoria temporal explícita.
2. **LSTM Estándar (Long Short-Term Memory)**:
   - Dos capas LSTM apiladas (`64` y `32` unidades) con **Recurrent Dropout (0.3)** para mitigar el sobreajuste en secuencias largas.
3. **LSTM Bidireccional Optimizado**:
   - Integración de capas `Bidirectional(LSTM)` con **Batch Normalization** y regularización por Dropout para procesar secuencias en ambas direcciones temporales (pasado y futuro contextual).

---

## 📊 Métricas de Evaluación

Los modelos fueron entrenados y validados utilizando:
- **Función de Pérdida**: Mean Squared Error (MSE)
- **Métrica Principal**: Mean Absolute Error (MAE)
- **Optimizador**: Adam con ajuste adaptativo de tasa de aprendizaje.

Curvas de entrenamiento y validación completas disponibles en el notebook.

---

## 🚀 Requisitos y Reproducción

1. Abre el notebook en Google Colab o entorno local:
   ```bash
   jupyter notebook HomeworkDeep6.ipynb
   ```

2. Dependencias requeridas:
   ```bash
   pip install tensorflow numpy pandas matplotlib
   ```
