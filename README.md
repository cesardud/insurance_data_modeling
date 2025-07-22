## ️‍🩹🏘️ Análisis y Modelado de Datos de Seguros — Sure Tomorrow

Este proyecto utiliza técnicas de *machine learning* para ayudar a la compañía ficticia **Sure Tomorrow** a tomar mejores decisiones relacionadas con clientes asegurados. Se implementan modelos para clasificación, regresión y ofuscación de datos, evaluando su eficacia y aplicabilidad en escenarios reales.

---

## 🎯 Objetivo

Desarrollar modelos de machine learning que permitan:

- Identificar clientes similares para campañas de marketing.
- Predecir si un cliente nuevo recibirá beneficios de seguro.
- Estimar la cantidad de beneficios que podría recibir.
- Ofuscar datos sensibles sin afectar el rendimiento predictivo.

---

## 🛠️ Herramientas y tecnologías

- Python 3.8+
- Bibliotecas:  
  - `pandas`, `numpy` (procesamiento de datos)  
  - `matplotlib`, `seaborn` (visualización)  
  - `scikit-learn` (modelado y métricas)
- Jupyter Notebooks en VS Code

---

## 📊 Dataset

El archivo `insurance_us.csv` contiene información de personas aseguradas. Las columnas disponibles son:

- `sexo` — Género del cliente  
- `edad` — Edad del cliente  
- `salario` — Ingreso anual  
- `familiares` — Número de familiares  
- `beneficios` — Cantidad de beneficios recibidos (objetivo)

---

### 1. 🔍 Encontrar clientes similares

- **Modelo utilizado:** K-Nearest Neighbors (KNN)
- **Propósito:** Buscar clientes con características similares a uno dado, para estrategias de marketing personalizadas.

---

### 2. ✅ Predecir si un cliente recibirá beneficios

- **Enfoque:** Clasificación binaria
- **Modelos:**  
  - K-Nearest Neighbors (KNN)  
  - DummyClassifier (modelo de referencia)
- **Métricas:** F1 Score, matriz de confusión
- **Resultado:** El modelo KNN superó significativamente al dummy.

---

### 3. 🔢 Predecir el número de beneficios

- **Enfoque:** Regresión lineal
- **Variables predictoras:** sexo, edad, salario, familiares
- **Métricas:** R², error cuadrático medio
- **Resultado:** Se logró una predicción razonable del número de beneficios.

---

### 4. 🔐 Proteger datos personales

- **Técnica aplicada:** Enmascaramiento de datos (ofuscación)
- **Objetivo:** Ocultar información sensible (como ingresos o edad) sin reducir significativamente el rendimiento del modelo.
- **Resultado:** El modelo sigue funcionando correctamente con los datos transformados.

---

## 🚀 Cómo ejecutarlo

1. **Clonar el repositorio**:
   ```bash
   git clone https://github.com/cesardud/insurance_data_modeling.git
   cd insurance_data_modeling
   
2. **Crear el entorno virtual**
  ```bash
  python3 -m venv venv
  source venv/bin/activate




  

