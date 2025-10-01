# scoring_crediticio

## Proyecto 3: Scoring Crediticio con Redes Neuronales Profundas (DNN)

### Descripción General:
* Diseño y evaluación de un Sistema Inteligente de Scoring Crediticio utilizando Redes Neuronales Profundas (DNN). El objetivo es predecir la probabilidad de impago de clientes bancarios, enfocándose en la eficiencia predictiva, la interpretación de resultados financieros y el uso de técnicas de Deep Learning tabulares.

### Objetivos del Proyecto:
* Implementar un pipeline completo de preprocesamiento de datos financieros (codificación, normalización).
* Diseñar y entrenar dos arquitecturas de redes neuronales: una DNN simple y un modelo inspirado en ResNet tabular.
* Optimizar el entrenamiento mediante el uso de callbacks (Early Stopping, ReduceLROnPlateau).
* Evaluar el rendimiento con métricas financieras clave (Curva ROC, Matriz de Confusión).
* Aplicar SHAP para asegurar que el modelo sea explicable, identificando los factores más influyentes en el riesgo crediticio.

### Tecnologías Clave:
* Lenguaje	Python
* Deep Learning	TensorFlow/Keras
* ML & Análisis	scikit-learn, pandas, numpy
* Visualización	matplotlib.pyplot, seaborn
* Explicabilidad	SHAP

### Características Destacadas:
* Arquitecturas de DL Tabular: Desarrollo y comparación de dos arquitecturas de DNN, explorando modelos más avanzados como el ResNet tabular para datos estructurados.
* Optimización del Entrenamiento: Uso de callbacks para un entrenamiento eficiente, previniendo el sobreajuste y ajustando dinámetros de aprendizaje.
* Explicabilidad Financiera: Aplicación de SHAP para proporcionar justificaciones claras y auditables para las decisiones de otorgamiento o denegación de crédito.

### Reflexión: Desafíos y Aprendizaje:
* El principal desafío en la modelización fue la detección de sesgos inherentes en el dataset histórico ("german.data"). Aunque se implementó un preprocesamiento riguroso, se aprendió que la falta de exploración explícita de sesgos podría perpetuar patrones de discriminación histórica. Técnicamente, la codificación de variables categóricas (usando LabelEncoder) y la inversión de la variable objetivo (0=Buen crédito, 1=Malo) son elecciones de diseño que deben ser rigurosamente documentadas y justificadas. El aprendizaje clave es que en el sector financiero, un alto rendimiento predictivo debe ir intrínsecamente ligado a la transparencia y justicia algorítmica.

[Ir al Código en Colab] → https://colab.research.google.com/drive/1jELwCwH9inAOttuuogUIP4ugBrMic-qr?usp=sharing

