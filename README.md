# 🚦 Siniestros Viales en Bogotá D.C. (2015–2021)

Análisis exploratorio e interactivo de los siniestros viales georreferenciados ocurridos en Bogotá, con datos abiertos de la **Secretaría Distrital de Movilidad**.

---

## 📊 Visualizaciones incluidas

| # | Gráfico | Tipo |
|---|---------|------|
| 1 | Siniestros por localidad | Bar Chart horizontal |
| 2 | Distribución por gravedad | Pie Chart |
| 3 | Tendencia histórica anual | Line Chart |
| 4 | Calor por hora y día de semana | Heatmap |
| 5 | Clase de accidente por localidad | Stacked Bar |
| 6 | Mapa de puntos críticos | Scatter Mapbox |

---

## 🗂️ Fuente de datos

**Datos Abiertos Bogotá — Secretaría Distrital de Movilidad**  
Licencia: Creative Commons Attribution 4.0  
🔗 https://datosabiertos.bogota.gov.co/dataset/historico-siniestros-bogota-d-c

---

## ⚙️ Requisitos

- Python 3.8 o superior
- pandas
- plotly

Instalar dependencias:

```bash
pip install pandas plotly
```

---

## 🚀 Cómo ejecutar el proyecto

### 1. Descargar el dataset

El dataset **no está incluido** en este repositorio por su tamaño. Debes descargarlo manualmente:

1. Ingresa a: https://datosabiertos.bogota.gov.co/dataset/historico-siniestros-bogota-d-c
2. Haz clic en **Descargar** → selecciona el formato **CSV**
3. Guarda el archivo en la **misma carpeta** donde está el notebook con el nombre original:
   ```
   historico_siniestros_bogota_d.c_-.csv
   ```

### 2. Ejecutar el notebook

Abre `Siniestros_Bogota.ipynb` en Jupyter y ejecuta todas las celdas en orden. El notebook ejecutará el archivo **historico_siniestros_bogota_d.c_-.csv** local que descargaste en la misma carpeta del notebook.

### 3. Gráficos exportados

Al finalizar la ejecución, se genera la carpeta `graficos_interactivos/` con los 6 gráficos en formato `.html` para visualización interactiva en el navegador.

---

## 📁 Estructura del proyecto

```
📦 siniestros-bogota/
├── 📓 Siniestros_Bogota.ipynb         # Notebook principal
├── 📄 README.md                        # Este archivo
└── 📂 graficos_interactivos/           # Generada al ejecutar el notebook
    ├── 01_siniestros_por_localidad.html
    ├── 02_distribucion_gravedad.html
    ├── 03_tendencia_historica.html
    ├── 04_heatmap_hora_dia.html
    ├── 05_clase_por_localidad.html
    └── 06_mapa_siniestros.html
```

---

## 🔍 Principales hallazgos

- **Kennedy y Engativá** lideran en número de siniestros, seguidas de Suba y Usaquén.
- El **choque** representa la gran mayoría de los accidentes en todas las localidades.
- La accidentalidad se mantiene alta de **6:00 a.m. a 9:00 p.m.**, con pico entre las 12:00 y las 15:00 horas.
- En **2020** hubo una caída drástica de siniestros, directamente relacionada con las restricciones de movilidad por la pandemia de COVID-19.
- Los siniestros más graves (heridos y muertos) se concentran sobre los corredores viales principales de la ciudad.

---

*Análisis realizado con Python, Plotly Express y pandas.*  
*Datos: Secretaría Distrital de Movilidad — Licencia Creative Commons Attribution 4.0*
