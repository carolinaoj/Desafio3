# Desafio3
Telecom X: Análisis de Evasión de Clientes (Churn)
Este proyecto forma parte de una iniciativa estratégica de Telecom X para reducir la pérdida de clientes mediante el análisis de datos y la preparación de un dataset óptimo para modelos de Machine Learning.

# Propósito del Análisis
La empresa enfrenta un alto índice de evasión de clientes. El objetivo de este análisis es:
- Extraer y normalizar datos complejos provenientes de una API en formato JSON.
- Limpiar y transformar variables críticas (cargos mensuales, totales y tipos de contrato).
- Identificar patrones de abandono mediante un Análisis Exploratorio de Datos (EDA).
- Entregar un dataset procesado que permita al equipo de Ciencia de Datos realizar predicciones precisas sobre qué clientes tienen mayor riesgo de irse.

# Estructura del Proyecto
Plaintext
TelecomX-Churn-Analysis/
├── 📄 TelecomX_Churn_Analysis.ipynb   # Notebook con el proceso ETL y EDA

├── 📊 TelecomX_Data_Final.csv         # Dataset procesado y listo para ML

├── 📝 README.md                       # Documentación del proyecto

└── ⚙️ .gitignore                     # Archivos excluidos del repositorio

# Análisis y Conclusiones
Durante el EDA, se identificaron factores clave que correlacionan con la evasión:
- Visualizaciones Destacadas
- Churn por Tipo de Contrato: Los clientes con contratos "Mes a Mes" representan el mayor volumen de evasión en comparación con contratos de 1 o 2 años.
- Distribución de Cargos: Se observó que los clientes con cargos mensuales superiores a $70 USD tienen una tendencia de abandono significativamente más alta.
- Antigüedad (Tenure): Existe un "periodo crítico" en los primeros 6 meses de servicio donde ocurre el 40% de la fuga total.

# Conclusiones Principales
La falta de compromiso a largo plazo es el predictor número uno de Churn.
Los usuarios de Fibra Óptica con facturación alta son los más propensos a cancelar el servicio.
Se eliminaron registros nulos en la variable objetivo para asegurar que el modelo predictivo no sea sesgado.

# Instrucciones para Ejecutar
Para replicar este análisis en tu entorno local o en la nube:

# Clonar el repositorio:
Bash:

git clone https://github.com/tu-usuario/TelecomX-Churn-Analysis.git
Abrir en Google Colab:
Subir el archivo .ipynb a tu Google Drive.
Ábrir con la extensión de Google Colaboratory.

# Ejecutar las celdas:

- Asegúrarse de ejecutar la sección de Extracción primero para obtener los datos actualizados de la API.
- No se necesita descargar archivos externos; el notebook consume los datos directamente desde la fuente raw de GitHub.

# Requisitos:

- Python 3.x
- Librerías: pandas, numpy, requests, seaborn, matplotlib.
