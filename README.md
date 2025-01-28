# Comprehensive Technical Test for Data Senior (IA) at Samay  
## Lung Sound Analysis for Respiratory Health  

### Objetivo  
El objetivo principal de esta prueba técnica es diseñar, desarrollar y optimizar una solución de aprendizaje automático para detectar y clasificar enfermedades respiratorias. Esto se logrará utilizando un conjunto de datos de sonidos pulmonares grabados con un estetoscopio electrónico. El cuaderno de trabajo entregado debe demostrar la competencia del candidato en el análisis de datos de sensores para aplicaciones de salud, específicamente en enfermedades pulmonares.  

---

### Descripción del Conjunto de Datos  
La evolución de la tecnología de los estetoscopios ha permitido la grabación de sonidos pulmonares de alta calidad en individuos sanos y en pacientes con diversas afecciones pulmonares.  

El conjunto de datos incluye grabaciones de audio de pacientes con siete enfermedades diferentes:  
- Asma  
- Insuficiencia cardíaca  
- Neumonía  
- Bronquitis  
- Derrame pleural  
- Fibrosis pulmonar  
- EPOC  

Además, incluye sonidos respiratorios normales.  

#### Características del Conjunto de Datos  
1. **Grabaciones**: Realizadas desde varias posiciones del pecho (determinadas por un médico especialista).  
2. **Modos de grabación**: Bell, Diaphragm y Extended para resaltar diferentes frecuencias corporales.  
3. **Detalles Demográficos**: Edad, género y diagnóstico de los pacientes.  
4. **Cobertura**: 112 sujetos (35 sanos y 77 con enfermedades respiratorias).  

---

### Partes del Proyecto  

#### 1. Exploración de Datos  
- Descargar y extraer los datos del archivo ZIP proporcionado:  
  URL: `https://prod-dcd-datasets-cache-zipfiles.s3.eu-west-1.amazonaws.com/jwyy9np4gv-3.zip`  
- **Tareas:**  
  - Crear una función para extraer nombres de archivo, construir etiquetas y analizar distribuciones mediante histogramas u otras herramientas gráficas.  
  - Generar una tabla con anotaciones demográficas y clasificaciones (por ejemplo, tipo de sonido, ubicación de grabación).  
  - Crear tablas de frecuencia absolutas y relativas.  
  - Graficar boxplots de la edad según el diagnóstico.  

---

#### 2. Procesamiento de Señales y Extracción de Características  
- **Tareas Principales:**  
  - Procesar archivos WAV y crear un marco de datos con las características extraídas (como tasa de muestreo, duración, amplitud, etc.).  
  - Realizar análisis estadístico general para cada enfermedad.  
  - Implementar funciones para graficar espectrogramas y formas de onda.  
  - Extraer características relevantes de los datos de audio (e.g., MFCC, tasa de cruces por cero, energía).  
  - Normalizar los datos y preparar las características para futuros modelos de aprendizaje automático.  

---

#### 3. Modelos de Aprendizaje Automático  
- **KNN (k-Nearest Neighbors):**  
  - Configurar una cuadrícula de hiperparámetros para optimizar el modelo.  
  - Implementar GridSearch para encontrar la mejor combinación de parámetros.  
  - Evaluar el modelo con un conjunto de pruebas y generar una matriz de confusión.  

- **Redes Neuronales Artificiales:**  
  - Entrenar un modelo usando PyTorch o Keras.  
  - Implementar callbacks y guardar los mejores modelos.  
  - Visualizar el rendimiento mediante una matriz de confusión en forma de heatmap.  

- **Algoritmos Clásicos de Machine Learning:**  
  - Desarrollar un clasificador multicategoría con SVM, XGBoost o LGBM.  

---

### Consideraciones Generales  
1. **Entrega:**  
   - Un cuaderno de trabajo funcional y listo para ejecutar.  
2. **Buenas prácticas:**  
   - Código estructurado, comentado y eficiente.  
3. **Resultados:**  
   - Resumir hallazgos clave, el desempeño de los modelos y el impacto potencial en la salud respiratoria.  
4. **Bibliografía:**  
   - Incluir referencias completas de todas las fuentes utilizadas.  

---

### Referencias Bibliográficas  
1. Fraiwan, Mohammad; Fraiwan, Luay; Khassawneh, Basheer; Ibnian, Ali (2021), "A dataset of lung sounds recorded from the chest wall using an electronic stethoscope", Mendeley Data, V3, doi: [10.17632/jwyy9np4gv.3](https://doi.org/10.17632/jwyy9np4gv.3).  
2. Luay Fraiwan et al., "Automatic identification of respiratory diseases from stethoscopic lung sound signals using ensemble classifiers," *Biocybernetics and Biomedical Engineering*, 2021, doi: [10.1016/j.bbe.2020.11.003](https://doi.org/10.1016/j.bbe.2020.11.003).  
3. Kaggle Dataset: Lung Sound Dataset.  
4. Md. Afzal Hossan et al., “A Novel Approach for MFCC Feature Extraction”, [IEEE](https://ieeexplore.ieee.org/abstract/document/5709752).  
