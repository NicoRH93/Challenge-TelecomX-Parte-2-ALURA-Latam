# 📊 Telecom X - Análisis de Evasión de Clientes (Churn)

Este proyecto analiza la evasión de clientes (*churn*) en Telecom X con el objetivo de identificar patrones y factores asociados a la pérdida de usuarios. El trabajo incluye limpieza de datos, análisis exploratorio (EDA), visualizaciones y recomendaciones estratégicas.

---

## 📌 Objetivo
Entender qué variables influyen en la cancelación de clientes y proporcionar insights para desarrollar estrategias de retención efectivas.

---

## 🛠️ Instalación y configuración

### 1. Clonar el repositorio

git clone https://https://github.com/Diana13Delgado/Challenge-Telecom-X

---

### 2. Crea un entorno virtual

- python -m venv venv
- source venv/bin/activate   # En macOS/Linux
- venv\Scripts\activate      # En Windows

---

### 3. Instalar dependencias

pip install -r requirements.txt

Ejemplo de requirements.txt:
pandas
numpy
matplotlib
plotly

___

### 4. Ejecucion

- Usando Jupyter Notebook
- Abrir el archivo notebook_analisis.ipynb en Jupyter Lab o Jupyter Notebook.
- Ejecutar las celdas secuencialmente para:
  - Cargar y limpiar los datos.
  - Realizar el análisis exploratorio (EDA).
  - Generar visualizaciones interactivas.
  - Obtener conclusiones y recomendaciones.

---

## 📂 Contenido del proyecto
- **`URL:'https://raw.githubusercontent.com/ingridcristh/challenge2-data-science-LATAM/refs/heads/main/TelecomX_Data.json`** → Con información de clientes.
- **`TelecomX_LATAM.ipynb`** → Proceso completo de ETL, EDA y generación de insights.
- **Visualizaciones** → Gráficos comparativos por:
  - Género
  - Tipo de contrato
  - Método de pago
  - Tipo de servicio de internet
  - Servicio telefónico
  - Variables numéricas (meses de contrato, cuentas totales, cuentas mensuales y diarias)

---
## 🛠️ Proceso de análisis
<img width="1024" height="1536" alt="image" src="https://github.com/user-attachments/assets/416863a0-9d84-445f-a322-b2ea4357a334" />

### 1. Limpieza y tratamiento de datos
- Importación de datos desde la API TelecomX
- Integración de estructuras anidadas del JSON en un único DataFrame.
- Comprobacion de inconsitencias en los datos.
- Conversión a tipos numéricos de variables clave.
- Creación de variables derivadas como `cuentas_diarias`.

---

### 2. Análisis exploratorio (EDA)
- **Distribución general del churn**: proporción de clientes que cancelaron vs los que permanecen.
- **Segmentación por variables categóricas**:
  **- Género**
<img width="1007" height="474" alt="image" src="https://github.com/user-attachments/assets/76f847ba-3075-4a25-b996-da9ed7d7ade3" />

  **- Tipo de contrato**
 <img width="1004" height="464" alt="image" src="https://github.com/user-attachments/assets/8fcf957b-97a6-4e76-81a5-86d1bb434cfe" />
 
  **- Método de pago**
  <img width="1003" height="465" alt="image" src="https://github.com/user-attachments/assets/dd5ff4e9-16d6-4190-839a-66dfe08af2d9" />

  **- Tipo de internet**
  <img width="1009" height="483" alt="image" src="https://github.com/user-attachments/assets/a6ea342c-19bf-42b9-9445-e639cca8e63c" />

  **- Servicio telefónico**
  <img width="1009" height="479" alt="image" src="https://github.com/user-attachments/assets/81b8665d-54aa-4c98-8b83-1a3c96d19705" />

- **Variables numéricas**:
  **- Meses de contrato (`meses_contrato`)**
  <img width="994" height="473" alt="image" src="https://github.com/user-attachments/assets/c026668e-3ec8-4054-876a-06617a71ad39" />

  **- Gasto total (`cuentas_totales`)**
  <img width="994" height="468" alt="image" src="https://github.com/user-attachments/assets/4b76ede3-873d-43c3-b041-e71d3c391a9e" />

  **- Gasto mensual (`cuentas_mensuales`)**
  <img width="983" height="458" alt="image" src="https://github.com/user-attachments/assets/a2eb5275-7700-44fe-b0fe-133b2ac187f1" />

  **- Gasto diario (`cuentas_diarias`)**
  <img width="984" height="469" alt="image" src="https://github.com/user-attachments/assets/639de454-1926-4d6d-aefc-45e92031feaa" />

- Uso de histogramas y boxplots plots para identificar patrones.

---

## 📈 Conclusiones
1. **Churn significativo**: existe un volumen importante de cancelaciones.
2. **Contratos mensuales**: concentran la mayor tasa de evasión.
3. **Método de pago**: *electronic check* se asocia con mayor churn que pagos automáticos.
4. **Tipo de internet**: la tecnología influye en la retención.
5. **Servicio telefónico**: posible relación con satisfacción y retención.
6. **Cancelación temprana**: clientes que se van suelen tener pocos meses de contrato.
7. **Relación con gasto**: cancelados tienen menor gasto total y en algunos casos gasto mensual/diario más alto.

---

## 💡 Recomendaciones
- **Onboarding y retención temprana**: programas de fidelización en los primeros 3–6 meses.
- **Incentivar contratos anuales**: descuentos o beneficios para migrar desde contratos mensuales.
- **Optimizar métodos de pago**: incentivar pagos automáticos.
- **Revisar calidad/precio del internet**: ajustar oferta en segmentos con alta cancelación.
- **Analizar el servicio telefónico**: mejorar valor percibido o precio.
- **Monitorear segmentos sensibles al precio**: ofrecer planes flexibles o descuentos preventivos.

---

## 🚀 Próximos pasos
- Implementar un modelo predictivo de churn para priorizar acciones de retención.
- Integrar variables externas como quejas y uso de servicio para mejorar la precisión del análisis.
- Automatizar reportes mensuales de métricas clave.

---

## 🖥️ Tecnologías utilizadas
- **Python** (pandas, numpy)
- **Visualización**: plotly, matplotlib
- **EDA**: análisis estadístico y segmentación
- **Jupyter Notebook** para documentación del proceso

---

## 📄 Licencia
Este proyecto se publica con fines educativos y de análisis interno para Telecom X.

---

## Contacto
Diana Delgado: github/Diana13Delgado
