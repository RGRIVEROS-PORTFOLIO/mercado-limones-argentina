# 🚗 Mercado de Limones Argentinos
## Selección adversa en transferencias automotrices argentinas 2023–2026

---

## Descripción

Análisis empírico de las transferencias automotrices registradas 
por la DNRPA entre 2023 y 2026, en el contexto de la crisis de 
sobrestock del mercado de 0km y la entrada de nuevas marcas al 
mercado argentino.

El proyecto aplica el marco teórico de **Akerlof (1970) — 
"The Market for Lemons"** y **Jensen & Meckling (1976)** para 
evaluar si los patrones observados en el mercado secundario son 
consistentes con mecanismos de selección adversa e incentivos 
desalineados.

---

## Pregunta de investigación

> ¿Existe evidencia en los registros DNRPA 2023–2026 de que el 
> shock de sobrestock en el mercado de 0km generó condiciones de 
> selección adversa en el mercado de usados, consistentes con el 
> mecanismo de Akerlof (1970)?

---

## Hipótesis de trabajo

1. En períodos de stress del mercado nuevo, la antigüedad promedio 
   de los vehículos transferidos aumenta.
2. El volumen de transferencias de marcas con menor historial local 
   cae proporcionalmente más que el mercado general.
3. Existe concentración de transferencias en el último trimestre 
   de cada año, consistente con el problema principal-agente 
   en concesionarias (Jensen & Meckling, 1976).

---

## Marco teórico

- **Akerlof, G. (1970).** The Market for Lemons: Quality 
  Uncertainty and the Market Mechanism. *The Quarterly Journal 
  of Economics*, 84(3), 488–500.
- **Jensen, M. & Meckling, W. (1976).** Theory of the Firm: 
  Managerial Behavior, Agency Costs and Ownership Structure. 
  *Journal of Financial Economics*, 3(4), 305–360.

---

## Fuente de datos

- **DNRPA** — Dirección Nacional de los Registros de la 
  Propiedad del Automotor
- Portal: datos.gob.ar
- Archivos utilizados: muestra de 7 meses seleccionados 
  por criterio teórico (ver nota metodológica en notebooks)

---

## Stack tecnológico

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)

- Python 3.11
- Pandas / NumPy / SciPy
- Matplotlib / Seaborn
- Jupyter Notebook
- VS Code + Miniconda

---

## Estructura del proyecto

├── data/

│   ├── raw/              # Datos originales (no versionados)

│   ├── raw_futuro/       # Archivos posteriores al cierre del análisis

│   └── processed/        # Datos procesados

├── notebooks/

│   ├── 01_exploracion.ipynb

│   ├── 02_pipeline_temporal.ipynb

│   ├── 03_Indice_Seleccion_Adversa.ipynb

│   └── 04_conclusiones.ipynb

├── reports/

│   └── figures/          # Visualizaciones exportadas

├── requirements.txt

├── INFORME_EJECUTIVO.md

└── README.md

---

## Nota metodológica

El análisis utiliza una muestra de 7 archivos mensuales 
seleccionados por criterio teórico, no una serie continua. 
Las conclusiones son exploratorias. Ver detalle en 
`notebooks/01_exploracion.ipynb`.

---

## Hallazgo central

> Cuando el mercado de autos nuevos baja de precio, el mercado 
> de usados no se beneficia. Se vacía de calidad.

El Índice de Selección Adversa (ISA) construido en este proyecto 
confirma que **Marzo 2026 registra el mayor nivel de stress del 
mercado en toda la serie analizada** — coincidiendo exactamente 
con la crisis actual de sobrestock en el segmento 0km.

---

## Estado del proyecto

✅ Completo — Ver `INFORME_EJECUTIVO.md` para resumen ejecutivo.

---

## Autor

**Rodolfo Gabriel Riveros Lobos**  
Data Analyst Junior | Calidad ISO · CX · Mejora Continua  
[LinkedIn](https://linkedin.com/in/rgriveros) · 
[Portfolio](https://github.com/RGRIVEROS-PORTFOLIO)