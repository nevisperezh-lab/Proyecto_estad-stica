# Proyecto de Estadística (2024-2)

**Autor:** Nevis Saray Perez Herrera  
**Entorno:** Google Colab / Python 3  

---

## Descripción del Proyecto

Este repositorio contiene un Jupyter Notebook desarrollado para la materia de **Estadística**, en el cual se aplican conceptos de estadística descriptiva, regresión lineal simple, intervalos de confianza y pruebas de hipótesis utilizando Python y sus librerías de análisis de datos.

El documento está dividido en dos secciones principales:

1. **Ejercicio Práctico de Regresión Lineal (Pérdida de Hidrógeno en Acero):** Análisis de la relación entre el tiempo de almacenamiento y la pérdida de hidrógeno a 20°C.
2. **Proyecto de Predicción de Precios Inmobiliarios (Real Estate Price Prediction):** Análisis descriptivo y modelado estadístico para evaluar la relación entre el precio de viviendas y su ubicación geográfica (latitud y longitud).

---

## Tecnologías y Librerías Utilizadas

* **Lenguaje:** Python 3
* **Librerías principales:**
  * `numpy`: Operaciones numéricas y cálculo de vectores.
  * `pandas`: Manipulación y estructuración de datos.
  * `scipy.stats`: Cálculo de regresión lineal (`linregress`) y distribuciones estadísticas.
  * `matplotlib.pyplot`: Visualización y generación de gráficos (diagramas de dispersión e histogramas).
  * `google.colab`: Montaje y lectura de archivos en Google Drive.

---

##  Estructura del Documento

### 1. Ejercicio 12.5: Pérdida de Hidrógeno en Muestras de Acero

Se evalúa la pérdida de hidrógeno en ppm a diferentes tiempos $t$ (horas) para muestras almacenadas a 20°C.

* **Diagrama de dispersión:** Visualización del comportamiento lineal negativo entre el tiempo y el contenido de hidrógeno.
* **Ecuación de Regresión Lineal:**
  $$\text{Hidrógeno perdido (ppm)} = -0.1220 \cdot t + 7.8267$$
  * *Interpretación:* Por cada hora transcurrida, la cantidad de hidrógeno disminuye en promedio 0.1220 ppm.
* **Intervalo de Confianza (95%):** 
  * Para $t = 20\text{ h}$, el intervalo de confianza predicho es **$(3.646\text{ ppm}, 7.126\text{ ppm})$**.
* **Coeficiente de Correlación y Prueba de Hipótesis:**
  * Coeficiente de correlación ($r$): **$-0.964$** (fuerte correlación negativa).
  * Prueba de hipótesis ($\rho = 0$, $\alpha = 0.10$):
    * $t_{\text{estadístico}} = -6.314$
    * $t_{\text{crítico}} = 2.353$
    * **Conclusión:** Se rechaza $H_0$, lo que confirma una relación lineal estadísticamente significativa entre el tiempo y la pérdida de hidrógeno.

---

### 2. Proyecto: Análisis de Precios Inmobiliarios (Real Estate Price Prediction)

Análisis exploratorio de datos utilizando el dataset [Real Estate Price Prediction](https://www.kaggle.com/datasets/quantbruce/real-estate-price-prediction/data).

* **Variables analizadas:**
  * `Y house price of unit area` (Precio por unidad de área)
  * `X5 latitude` (Latitud)
  * `X6 longitude` (Longitud)

* **Estadística Descriptiva:**
  * **Precio por unidad de área:** Media = $37.98$, Mediana = $38.45$, Desviación Estándar = $13.606$, Varianza = $185.137$.
  * **Latitud:** Media = $24.969$, Mediana = $24.971$, Desviación Estándar = $0.0124$, Varianza = $0.0002$.
  * **Longitud:** Media = $121.533$, Mediana = $121.539$, Desviación Estándar = $0.0150$, Varianza = $0.0002$.

* **Visualización:**
  * Generación de histogramas comparativos con la curva de distribución normal ajustada para cada variable aleatoria continua.

---

##  Cómo Ejecutar el Notebook

1. **Clonar o descargar el repositorio:**
   ```bash
   git clone [https://github.com/TU_USUARIO/TU_REPOSITORIO.git](https://github.com/TU_USUARIO/TU_REPOSITORIO.git)
