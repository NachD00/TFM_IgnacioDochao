# Análisis de Sentencias Judiciales mediante PLN

Este repositorio contiene el código fuente y los recursos asociados al Trabajo de Fin de Máster titulado **"Análisis de sentencias judiciales mediante PLN: un enfoque descriptivo y predictivo sobre la jurisprudencia australiana"**, desarrollado en el marco del Máster en Business Analytics en la Universidad Pontificia Comillas.

## 📄 Resumen

El objetivo de este proyecto es aplicar técnicas de Procesamiento de Lenguaje Natural (PLN) y Machine Learning para analizar un corpus de 24.985 sentencias judiciales australianas. El análisis combina:

- Representación semántica (TF-IDF, Word2Vec, LDA)
- Visualización de temas y agrupamiento de documentos
- Predicción del tratamiento posterior de las sentencias (`case_outcome`) mediante clasificadores supervisados

## ⚙️ Tecnologías y librerías utilizadas

- **Lenguaje**: Python 3.12
- **Entorno**: JupyterLab 4.3.4
- **PLN y procesamiento**:
  - `nltk`, `spaCy`
- **Modelado y representación**:
  - `gensim`, `scikit-learn`, `pyLDAvis`
- **Visualización**:
  - `matplotlib`, `seaborn`, `wordcloud`
- **Otras herramientas**:
  - `joblib`, `networkx`, `pandas`, `numpy`

## 🧪 Pipeline Metodológico

1. **Análisis Exploratorio de Datos (EDA)**
2. **Preprocesamiento del texto legal**
3. **Representación semántica**: TF-IDF, Word2Vec, LDA
4. **Clustering temático** con KMeans
5. **Predicción del `case_outcome`** con:
   - Regresión Logística
   - Random Forest
   - Gradient Boosting

## 📊 Resultados clave

- **F1-macro** alcanzado por los modelos:
  - Logistic Regression: `0.33`
  - Gradient Boosting: `0.24`
  - Random Forest: `0.19`
- **Temas jurídicos detectados** (via LDA): inmigración, fiscalidad, propiedad intelectual, daño laboral, entre otros.
- **Limitaciones**: desbalance severo de clases, corpus sin metadatos, y exclusión deliberada de modelos transformers por razones computacionales y de interpretabilidad.

## 🧠 Requisitos

Instalar las dependencias (se recomienda crear un entorno virtual):

```bash
pip install -r requirements.txt
