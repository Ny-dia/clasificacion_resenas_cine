# 📽️ Clasificación de Reseñas de Cine - Análisis de Sentimiento

Repositorio: https://github.com/Ny-dia/clasificacion_resenas_cine
Notebook Principal: Modelo_de_clasificacion_de_reseñas_de_cine.ipynb

## 📌 Descripción

Este repositorio contiene un modelo de análisis de sentimiento entrenado para clasificar reseñas de cine como positivas (👍) o negativas (👎). El proyecto incluye:

Preprocesamiento de texto (limpieza, tokenización)

Modelos de redes neuronales (LSTM)

Evaluación de métricas (accuracy, F1-score)

Visualizaciones interactivas

## 🛠️ Tecnologías
Python

TensorFlow

Keras

Pandas

NLTK

## 📊 Dataset
Se utilizó el IMDB Dataset de 50K reseñas con etiquetas balanceadas:

25,000 reseñas positivas

25,000 reseñas negativas

## 🚀 Resultados
El modelo alcanzó un 86% de precisión con la siguiente distribución:

Métrica	Negative	Positive

Precision	0.86	0.86

Recall	0.86	0.87

F1-Score	0.86	0.86

## 🧠 Arquitectura del Modelo
python
model = Sequential([
    Embedding(5000, 256, input_length=100),
    LSTM(128, return_sequences=True, dropout=0.2),
    LSTM(64),
    Dense(64, activation='relu'),
    Dropout(0.5),
    Dense(1, activation='sigmoid')
])

## 📋 Cómo Usar
Clona el repositorio:

bash
git clone https://github.com/Ny-dia/clasificacion_resenas_cine.git
Instala dependencias:

bash
pip install -r requirements.txt
Ejecuta el notebook:

bash
jupyter notebook Modelo_de_clasificacion_de_reseñas_de_cine.ipynb

## 🌟 Mejoras Futuras
Implementar BERT para mayor precisión

Desplegar modelo como API

Añadir análisis por género de película

## 🤝 Contribuciones
¡Contribuciones son bienvenidas! Abre un issue o envía un pull request.

Autora-Nydia Mejía Zavala
