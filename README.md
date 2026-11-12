# Proyecto 7: Análisis del comportamiento de clientes de NovaRetail+

## Objetivo del proyecto

Analizar el comportamiento de 15,000 clientes de NovaRetail+ durante 2024, utilizando información demográfica, hábitos de navegación, frecuencia de compra, publicidad dirigida y características de los clientes.

El propósito es identificar las variables que presentan una mayor asociación con los ingresos anuales generados, evaluar la intensidad de estas relaciones y detectar oportunidades que permitan optimizar las estrategias comerciales y apoyar la toma de decisiones del negocio.

## Datasets utilizados

El análisis utiliza un conjunto de datos en formato CSV:

- **`novaretail_comportamiento_clientes_2024.csv`**: contiene información de 15,000 clientes, incluyendo edad, nivel de ingreso, visitas mensuales, compras mensuales, gasto en publicidad dirigida, satisfacción, membresía premium, abandono, tipo de dispositivo, región e ingreso anual generado.

La variable principal de interés es **`ingreso_anual`**, que representa los ingresos generados por los clientes para NovaRetail+.

## Etapas del análisis

1. **Carga y exploración de datos:** lectura del archivo CSV, revisión de dimensiones, tipos de datos, estructura del dataset y valores faltantes.

2. **Validación y preparación de datos:** revisión de la integridad de la información, identificación de variables numéricas y categóricas y adecuación de tipos de datos para el análisis.

3. **Análisis estadístico descriptivo:** cálculo de medidas de tendencia central, dispersión y distribución de las principales variables, así como análisis de frecuencias de las variables categóricas.

4. **Análisis exploratorio y visualización:** elaboración de gráficos de dispersión, matrices de correlación y visualizaciones para identificar tendencias y posibles asociaciones entre las variables.

5. **Correlaciones de Pearson y Spearman:** evaluación de la dirección e intensidad de las asociaciones entre variables numéricas, especialmente respecto al ingreso anual generado.

6. **Correlación punto-biserial:** análisis de la relación entre variables binarias, como membresía premium y abandono, y el ingreso anual, incluyendo la evaluación de significancia estadística.

7. **V de Cramér:** evaluación de la intensidad de asociación entre variables categóricas, específicamente el tipo de dispositivo utilizado y la región geográfica de los clientes.

8. **Interpretación de resultados para el negocio:** elaboración de cinco hallazgos principales, integrando evidencia numérica, evidencia visual cuando corresponde, interpretación no causal, limitaciones y posibles implicaciones comerciales.

9. **Limitaciones y próximos pasos:** identificación de las restricciones del análisis y propuesta de futuras investigaciones relacionadas con segmentación, conversión, rentabilidad y validación de estrategias comerciales.

## Principales hallazgos

- **Frecuencia de compra:** presenta una asociación positiva muy fuerte con el ingreso anual (Pearson = 0.9671), siendo la variable con mayor correlación observada.

- **Visitas mensuales:** muestran una asociación positiva moderada con el ingreso anual (Pearson = 0.3371), lo que sugiere una relación entre la actividad de los clientes y los ingresos generados.

- **Publicidad dirigida:** presenta una asociación positiva débil con el ingreso anual (Pearson = 0.1975), por lo que una mayor inversión publicitaria no necesariamente se relaciona con incrementos proporcionales en los ingresos.

- **Membresía premium:** muestra una asociación positiva muy débil (r = 0.0931), aunque estadísticamente significativa (p < 0.05). Esto evidencia la importancia de distinguir entre significancia estadística y relevancia práctica.

- **Abandono de clientes:** presenta una asociación prácticamente nula con el ingreso anual (r = -0.0028), sin significancia estadística (p = 0.7295).

Adicionalmente, el análisis de V de Cramér identificó una asociación prácticamente nula entre el tipo de dispositivo y la región geográfica (V = 0.0124).

**Nota:** Los resultados representan asociaciones estadísticas y no permiten establecer relaciones de causa y efecto.

## Cómo abrir y ejecutar el notebook

1. Descarga o clona el repositorio que contiene este README, el notebook y, si está disponible para su distribución, el archivo CSV.

2. Para consultar el notebook sin ejecutarlo, abre el repositorio en GitHub y selecciona el archivo `.ipynb`. GitHub permite visualizar las celdas de código, resultados y gráficos guardados.

3. Para ejecutar las celdas, abre el notebook en un entorno compatible con Jupyter, como Jupyter Notebook, JupyterLab o Google Colab.

4. Asegúrate de que el archivo `novaretail_comportamiento_clientes_2024.csv` esté disponible en la ruta utilizada por el notebook. Si es necesario, modifica la ruta de lectura.

5. Ejecuta las celdas en orden, desde la importación de librerías y la carga del dataset hasta los análisis estadísticos, visualizaciones y conclusiones.

## Guía breve para reproducir el análisis

- Utiliza Python 3 y las librerías `pandas`, `numpy`, `matplotlib`, `seaborn` y `scipy`.

- Coloca el archivo `novaretail_comportamiento_clientes_2024.csv` en la ubicación esperada por el notebook o actualiza la ruta correspondiente.

- Ejecuta todas las celdas en orden para reproducir la exploración, preparación, análisis descriptivo, visualizaciones y cálculos de correlación.

- Utiliza Pearson y Spearman para analizar asociaciones entre variables numéricas.

- Aplica la correlación punto-biserial para estudiar la relación entre variables binarias y el ingreso anual.

- Utiliza V de Cramér para evaluar asociaciones entre variables categóricas.

- Revisa los coeficientes y valores p antes de interpretar los resultados, diferenciando la intensidad de una asociación de su significancia estadística.

- Considera que las correlaciones identificadas no demuestran causalidad y pueden estar influidas por otras variables no incluidas en el análisis.

## Resultado esperado

Al finalizar, se obtiene un análisis estadístico del comportamiento de los clientes de NovaRetail+, acompañado de visualizaciones, matrices de correlación y cinco hallazgos orientados al negocio.

Los resultados permiten identificar qué variables presentan mayores asociaciones con los ingresos anuales, reconocer las limitaciones de estas relaciones y proponer oportunidades de mejora en segmentación, conversión, publicidad dirigida y retención de clientes.

El proyecto demuestra la aplicación de técnicas de análisis exploratorio de datos, estadística y comunicación de resultados para apoyar la toma de decisiones comerciales basadas en evidencia.

