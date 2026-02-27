# 🥔 Clasificador de Enfermedades de la Papa

## 📌 Resumen

Este proyecto consiste en el desarrollo de una aplicación web interactiva construida con **Streamlit**, cuyo objetivo es permitir a agricultores, técnicos agrícolas e investigadores cargar imágenes de hojas de papa para detectar automáticamente enfermedades mediante un modelo de **Deep Learning (PyTorch)** previamente entrenado.

La aplicación se enfoca en la **detección temprana**, la **rapidez de diagnóstico** y el **apoyo a la toma de decisiones agrícolas**, reduciendo el margen de error humano en la inspección visual tradicional.

---

## 🎯 Problema y Solución

| Problema en el Cultivo de Papa | Solución Propuesta |
|--------------------------------|-------------------|
| Diagnóstico tardío de enfermedades | Detección automática en segundos mediante visión artificial |
| Confusión entre enfermedades similares | Clasificación precisa basada en CNN entrenada |
| Pérdida de rendimiento por inspección manual | Identificación temprana para tratamiento oportuno |
| Dependencia de expertos | Herramienta accesible para cualquier agricultor |
| Evaluaciones inconsistentes | Estandarización mediante modelo validado |

---

## 🧠 Descripción del Proyecto

Sistema de clasificación de enfermedades en hojas de papa basado en **Redes Neuronales Convolucionales (CNN)** implementadas con PyTorch, capaz de analizar imágenes y determinar el estado fitosanitario del cultivo.

### Clases Detectadas

- Papa Sana  
- Tizón Tardío  
- Tizón Temprano  


---

## 🔬 Pipeline de Desarrollo

1. Organización del dataset en carpetas por clase.
2. División en entrenamiento, validación y prueba.
3. Transformaciones de imagen:
   - Resize
   - Normalización
   - Conversión a tensor
4. Entrenamiento del modelo CNN.
5. Evaluación mediante métricas y matriz de confusión.
6. Exportación del modelo entrenado (`.pth`).
7. Despliegue en aplicación web con Streamlit.

---

## 📊 Evaluación del Modelo

Se utilizaron las siguientes métricas:

- **Accuracy** → rendimiento general del modelo  
- **Precision** → confiabilidad de las predicciones positivas  
- **Recall** → capacidad de detectar correctamente cada enfermedad  
- **F1-score** → equilibrio entre precisión y recall  
- **Matriz de Confusión** → análisis detallado de errores por clase  



---

## 🖥️ Aplicación Web

La aplicación fue desarrollada con [Streamlit](https://potato-disease-classifierapp-kvehrcjnnt5f2orrmuokld.streamlit.app/) y permite:

- 📤 Subir una imagen (`.jpg` / `.png`)
- 🖼 Visualizar la imagen cargada
- 🤖 Obtener predicción automática
- 📊 Ver probabilidad por clase
- ⚡ Inferencia rápida en CPU
- 🧠 Carga optimizada del modelo con `st.cache_resource`

---

