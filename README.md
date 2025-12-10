# Análisis de Calidad del Aire y Salud Pública

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

## Descripción del Proyecto

Análisis exhaustivo de la correlación entre la contaminación del aire urbana y los indicadores de salud pública en 24 de las principales ciudades del mundo. Este proyecto examina las concentraciones de contaminantes atmosféricos (PM2.5, PM10, NO2) y su relación con las tasas de mortalidad y enfermedades respiratorias.

**Objetivo:** Demostrar mediante análisis de datos y técnicas de Machine Learning la fuerte correlación entre la calidad del aire y el impacto en la salud pública, proporcionando insights accionables para políticas ambientales.

## Impacto y Aplicabilidad

- **Impacto Social:** Aborda un problema crítico que afecta a millones de personas en áreas urbanas
- **Sectores Aplicables:** Consultorías ambientales, ONGs, gobiernos, organismos internacionales (OMS, ONU)
- **Habilidades Demostradas:** Python, análisis estadístico, visualización de datos, machine learning

## Resultados Clave

- **95.8%** de las ciudades analizadas exceden el límite de PM2.5 recomendado por la OMS (15 μg/m³)
- **Correlación 0.958** entre concentración de PM2.5 y mortalidad respiratoria (p-valor < 0.001)
- **Modelo predictivo** con R² = 0.883 y MAE = 6.9 muertes/100k habitantes
- Las ciudades grandes tienen contaminación significativamente mayor que las pequeñas (p < 0.05)

## Visualizaciones Principales

### Mapa Mundial de Contaminación
![Mapa Mundial](images/Mapa%20Mundial%20Contaminación%20del%20Aire%20por%20Ciudad.jpg)
*Distribución geográfica de la contaminación PM2.5 en ciudades principales del mundo*

### Top 10 Ciudades Más Contaminadas
![Top 10 Ciudades](images/Top%2010%20Ciudades%20con%20Mayor%20Contaminación%20PM2.5.jpg)
*Delhi (India) lidera con 115 μg/m³, seguida por Mumbai y Jakarta*

### Correlación Contaminación vs Mortalidad
![Correlación](images/Correlación%20Contaminación%20del%20Aire%20vs%20Mortalidad.jpg)
*Relación lineal fuerte entre PM2.5 y muertes respiratorias por 100k habitantes*

### Análisis Regional
![Distribución Regional](images/Distribución%20de%20Contaminación%20PM2.5%20por%20Región.jpg)
*Asia y África presentan los niveles más altos de contaminación atmosférica*

### Dashboard Integral
![Dashboard](images/Dashboard%20Integral%20Análisis%20de%20Calidad%20del%20Aire.jpg)
*Visualización integrada con múltiples métricas de calidad del aire*

### Matriz de Correlación
![Matriz Correlación](images/Matriz%20de%20Correlación%20Variables%20Ambientales%20y%20de%20salud.jpg)
*Análisis de correlaciones entre todas las variables ambientales y de salud*

## 🔬 Metodología

### 1. Recolección de Datos
- **Fuente:** Datos basados en World Air Quality Database (IQAir) y WHO Air Quality Database
- **Alcance:** 24 ciudades principales en 22 países
- **Variables:** PM2.5, PM10, NO2, AQI, población, mortalidad respiratoria

### 2. Análisis Exploratorio (EDA)
- Estadísticas descriptivas y distribuciones
- Identificación de outliers mediante método IQR
- Análisis por región geográfica y categoría de población
- Creación de variables derivadas (pollution_index, health_risk_score)

### 3. Análisis Estadístico
- **Correlaciones:** Matriz de Pearson entre variables ambientales y de salud
- **Pruebas de hipótesis:** Test t de Student para comparación entre grupos
- **Significancia:** Validación estadística con p-valores < 0.05

### 4. Visualización de Datos
- Gráficos estáticos con Matplotlib y Seaborn
- Visualizaciones interactivas con Plotly
- Mapas geográficos con coordenadas de ciudades
- Dashboard integral con múltiples métricas

### 5. Machine Learning
- **Modelo:** Regresión Lineal para predicción de mortalidad respiratoria
- **Features:** PM2.5, PM10, NO2, población urbana
- **Performance:** R² = 0.883, MAE = 6.9 muertes/100k

## Tecnologías Utilizadas

```python
- Python 3.8+
- Pandas & NumPy (manipulación de datos)
- Matplotlib & Seaborn (visualización estática)
- Plotly (visualizaciones interactivas)
- Scikit-learn (machine learning)
- SciPy (análisis estadístico)
- Folium (mapas interactivos)
```

## Estructura del Proyecto

```
air-quality-health-analysis/
│
├── notebooks/
│   └── analisis_calidad_aire.ipynb    # Análisis completo
│
├── images/                             # Visualizaciones principales
│   ├── Mapa Mundial Contaminación del Aire por Ciudad.jpg
│   ├── Top 10 Ciudades con Mayor Contaminación PM2.5.jpg
│   ├── Correlación Contaminación del Aire vs Mortalidad.jpg
│   ├── Distribución de Contaminación PM2.5 por Región.jpg
│   ├── Dashboard Integral Análisis de Calidad del Aire.jpg
│   └── Matriz de Correlación Variables Ambientales y de salud.jpg
│
├── requirements.txt                    # Dependencias del proyecto
└── README.md                          # Este archivo
```

## Cómo Ejecutar el Proyecto

### 1. Clonar el repositorio
```bash
git clone https://github.com/TU_USUARIO/air-quality-health-analysis.git
cd air-quality-health-analysis
```

### 2. Instalar dependencias
```bash
pip install -r requirements.txt
```

### 3. Abrir el notebook
```bash
jupyter notebook notebooks/analisis_calidad_aire.ipynb
```

O ejecutar directamente en Google Colab haciendo clic en el badge:
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/TU_USUARIO/air-quality-health-analysis/blob/main/notebooks/analisis_calidad_aire.ipynb)

## Principales Hallazgos

### 1. Crisis Global de Calidad del Aire
Solo 1 de cada 24 ciudades cumple con los estándares de la OMS para PM2.5, evidenciando una crisis de salud pública global.

### 2. Impacto Directo en Salud
Existe una correlación extremadamente fuerte (r=0.958) entre la contaminación del aire y las muertes respiratorias, con significancia estadística robusta.

### 3. Disparidad Regional
Asia y África enfrentan los niveles más críticos de contaminación, mientras que Oceanía y Europa mantienen índices relativamente bajos.

### 4. Tamaño de Ciudad como Factor
Las ciudades grandes (>15M habitantes) presentan niveles de contaminación significativamente mayores que las ciudades pequeñas (<5M), confirmado estadísticamente.

### 5. Capacidad Predictiva
El modelo de regresión lineal puede predecir con 88% de precisión la mortalidad respiratoria basándose únicamente en métricas de contaminación atmosférica.

## Conclusiones y Recomendaciones

**Conclusiones:**
- La contaminación del aire es un predictor confiable de mortalidad respiratoria
- El 95.8% de las ciudades analizadas requieren intervención urgente
- Existe una clara necesidad de políticas públicas basadas en evidencia científica

**Recomendaciones:**
1. Implementar sistemas de monitoreo continuo de calidad del aire
2. Establecer políticas de reducción de emisiones vehiculares e industriales
3. Desarrollar alertas tempranas para poblaciones vulnerables
4. Invertir en transporte público limpio y zonas de bajas emisiones

## Sobre el Autor

**Fabricio Bagatto**  
Ingeniero en Recursos Naturales | Data Analyst

Este proyecto forma parte de mi portfolio profesional, demostrando habilidades en:
- Análisis exploratorio de datos (EDA)
- Visualización de datos estática e interactiva
- Análisis estadístico y pruebas de hipótesis
- Machine Learning aplicado
- Comunicación de insights técnicos


## Agradecimientos

- Datos inspirados en **IQAir World Air Quality Database**
- Estándares de referencia de la **Organización Mundial de la Salud (OMS)**
- Comunidad de código abierto por las librerías utilizadas

---

**Nota:** Los datos utilizados son simulados pero realistas, basados en rangos y distribuciones de datasets públicos de calidad del aire.
