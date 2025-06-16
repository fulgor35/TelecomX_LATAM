 📊 Telecom X - Análisis de Evasión de Clientes
 🎯 Objetivo

El objetivo de este proyecto es analizar los datos históricos de clientes de **Telecom X** para comprender los factores que influyen en la evasión (churn) de clientes. A través de técnicas de limpieza, transformación y análisis exploratorio de datos, se busca extraer insights útiles que permitan crear futuras estrategias de retención, así como alimentar modelos predictivos que anticipen el abandono de clientes.


 🧠 Lo que se practicó

Durante este proyecto se practicaron y aplicaron habilidades esenciales de Ciencia de Datos, tales como:

- Importación y manipulación de datos estructurados en formato JSON.
- Aplicación del proceso **ETL** (Extracción, Transformación y Carga).
- Análisis exploratorio de datos (EDA) con visualizaciones significativas.
- Tratamiento de datos faltantes y detección de incoherencias.
- Conversión y normalización de variables categóricas y numéricas.
- Evaluación de correlaciones entre variables.
- Generación de un informe final estructurado y redactado en entorno colaborativo.


 📂 Estructura del análisis
 🔹 Extracción de datos

- Los datos fueron cargados a partir de archivos en formato JSON, representando información de clientes, servicios contratados y facturación mensual.

 🔹 Transformación
 ✅ Conocer el conjunto de datos

- Se exploraron las columnas del dataset, su estructura y tipo de datos.
- Se utilizó un diccionario de datos para comprender el significado de cada variable.

 ✅ Comprobación de incoherencias

- Se identificaron valores nulos en columnas clave como `cargo_total`.
- Se eliminaron o transformaron registros con datos incompletos.

 ✅ Creación de la columna de cuentas diarias

- Se creó la variable `cargo_diario`, obtenida al dividir `cargo_mensual` por 30 para estimar el valor diario facturado.
 ✅ Estandarización y transformación de datos

- Se renombraron todas las columnas a español, en formato snake_case.
- Se transformaron variables categóricas binarias (`Yes/No`) a numéricas (`1/0`).
- Se creó una nueva variable `cantidad_servicios` que suma todos los servicios contratados por cliente.

 🔹 Carga y Análisis (L – Load & Analysis)

 📈 Análisis descriptivo

- Se usó `.describe()` para obtener estadísticas clave de variables numéricas.

 📉 Distribución de evasión

- Se generó un gráfico de barras para visualizar la proporción de clientes que abandonan versus los que permanecen.

 🧩 Recuento de evasión por variables categóricas

- Se agruparon los datos por columnas categóricas como `tipo_contrato`, `metodo_pago`, `pareja`, etc., visualizando la proporción de abandono por categoría.

 📊 Conteo de evasión por variables numéricas

- Se utilizaron boxplots para explorar cómo variables como `meses_contrato`, `cargo_total` y `cargo_diario` se distribuyen entre quienes abandonan y quienes permanecen.

 🔹 Tarea Extra

 🔍 Análisis de correlación entre variables

- Se utilizó la función `.corr()` y un mapa de calor para visualizar la fuerza de la relación entre `churn` y otras variables numéricas.
- Se concluyó que `meses_contrato` y `cantidad_servicios` tienen fuerte relación negativa con la evasión.

 🔹 Informe Final

- El informe fue redactado directamente en el archivo `.ipynb`, incluyendo secciones de introducción, tratamiento de datos, análisis y conclusiones.
- Cada sección está acompañada de texto en formato Markdown y referencias a visualizaciones relevantes.

---

 📊 Visualizaciones

El análisis incluye múltiples visualizaciones como:

- Gráficos de barras para evasión.
- Gráficos apilados por variables categóricas.
- Boxplots para variables numéricas vs. churn.
- Heatmap de correlaciones entre variables.

Todas las visualizaciones están incluidas directamente en el notebook y referenciadas en las secciones correspondientes.

---

 ✅ Recomendaciones finales

- Incentivar contratos a largo plazo, dado que la duración es la variable más inversamente correlacionada con el churn.
- Promover paquetes con múltiples servicios, ya que se observó menor abandono entre clientes con mayor cantidad de servicios contratados.
- Revisar estrategias de precios, especialmente para quienes enfrentan altos cargos mensuales.
- Priorizar acciones sobre clientes sin pareja o dependientes, quienes muestran mayor tendencia a abandonar.

---

 🛠️ Herramientas utilizadas

- **Lenguaje de programación:** Python
- **Entorno:** Google Colab
- **Bibliotecas:**  
  - `pandas` para manipulación de datos  
  - `matplotlib` y `seaborn` para visualizaciones  
  - `numpy` para operaciones numéricas
- **Formato de datos:** JSON
- **Asistencia y mentoría:** ChatGPT (OpenAI)

---

 🚀 Cómo ejecutar el proyecto

1. Clona este repositorio en tu equipo local o en Google Colab:

2. Abre el archivo TelecomX_Churn_Analisis.ipynb en Google Colab o Jupyter Notebook.

3. Ejecuta las celdas paso a paso para revisar el análisis completo y sus resultados.

Gracias por visitar este repositorio.
¡Transformar datos en decisiones nunca fue tan poderoso! 🚀
