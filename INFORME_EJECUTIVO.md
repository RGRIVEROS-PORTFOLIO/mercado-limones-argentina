# 🚗 Mercado de Limones Argentinos
## Selección adversa en transferencias automotrices argentinas — 2023-2026

**Informe ejecutivo** · Junio 2026

---

## Resumen en 30 segundos

Se analizaron **1.025.853 transferencias automotrices** registradas 
por la DNRPA entre enero 2023 y marzo 2026 para evaluar si la crisis 
actual del mercado de 0km (sobrestock, descuentos de hasta 25%) está 
deteriorando la calidad disponible en el mercado de usados.

**Resultado:** sí. Marzo 2026 registra el punto de mayor selección 
adversa de toda la serie analizada, medido a través de un índice 
compuesto construido específicamente para este proyecto.

---

## El hallazgo central

> Cuando el mercado de autos nuevos baja de precio, el mercado de 
> usados no se beneficia. Se vacía de calidad.

Los compradores con capacidad crediticia migran hacia el 0km atraídos 
por los descuentos. En el mercado de usados queda una demanda con 
menor capacidad de verificación, que acepta mayor incertidumbre de 
calidad a cambio de menor precio. El resultado es medible: la 
antigüedad promedio de los vehículos transferidos sube, y la 
participación de vehículos importados bajo Protocolo 21 (Mercosur) 
alcanza su máximo histórico exactamente en este período.

---

## Metodología

| Aspecto | Detalle |
|---|---|
| Fuente | DNRPA — Dirección Nacional de los Registros de la Propiedad del Automotor |
| Volumen | 1.025.853 registros, 7 archivos mensuales |
| Período | Enero 2023 — Marzo 2026 |
| Criterio de muestreo | Selección teórica de meses con relevancia macroeconómica |
| Marco teórico | Akerlof (1970), Jensen & Meckling (1976) |
| Herramienta central | Índice de Selección Adversa (ISA) — z-score compuesto, validado con análisis de robustez |

**Nota de honestidad metodológica:** este es un análisis descriptivo, 
no predictivo. Con 7 puntos temporales no es posible inferencia 
estadística con significancia. El valor del proyecto está en 
identificar y cuantificar un mecanismo de mercado, no en predecirlo.

Detalle completo de limitaciones en `notebooks/04_conclusiones.ipynb`.

---

## Los tres hallazgos clave

**1. No todas las marcas envejecen igual en el mercado de usados.**
Se identificó una taxonomía de cuatro comportamientos: marcas 
"anti-limón" (Toyota, Nissan — venta rápida por reputación verificable), 
"limón clásico" (Ford, Fiat — alta antigüedad por modelos discontinuados 
de larga circulación), "limón premium" (Mercedes Benz — retención 
prolongada por precio de reserva elevado del propietario) y mercados 
heterogéneos (Jeep — dos poblaciones de antigüedad mezcladas).

**2. La crisis del 0km se propaga en cascada hacia el segmento más vulnerable.**
Sobrestock en 0km → migración de compradores solventes hacia el 0km → 
contracción de demanda de calidad en usados Nacional → concentración 
de compradores vulnerables en Protocolo 21, el segmento con menor 
verificabilidad de historial.

**3. El Índice de Selección Adversa confirma el momento crítico.**
Marzo 2026 es el punto de mayor stress de toda la serie. Diciembre 
2024 es el de menor stress, explicado por la presión de objetivos 
comerciales de fin de año que fuerza a liberar primero las mejores 
unidades.

---

## Recomendaciones por actor

**Agencieros (vendedores de usados):** no compitan en precio contra 
el 0km con descuento — esa pelea no se gana. Compitan en transparencia: 
informe de dominio, service documentado, inspección de tercero.

**Compradores de usados:** si pueden esperar la normalización del 0km, 
esperen. Si necesitan comprar un Protocolo 21 ahora, destinen 3-5% 
del valor del vehículo a verificación profesional antes de cerrar.

**Financieras de crédito automotor:** incorporar el origen del 
vehículo (Nacional / Importado / Protocolo 21) y un proxy del ISA 
mensual como variables de scoring de riesgo, no solo marca/modelo/año.

---

## Líneas de trabajo futuro

1. Incorporar archivos de Abril-Mayo 2026 (publicados durante el cierre de este análisis)
2. Cruzar con Infovalores DNRPA para cuantificar depreciación en pesos
3. Procesar serie mensual completa (28 archivos) para análisis de series de tiempo con n robusto
4. Validar con fuente externa la hipótesis sobre Protocolo 21 (canal de acceso vs. asimetría)
5. Modelo a nivel de transacción individual, aprovechando el volumen de 1M+ registros
6. Comparación interprovincial — con foco específico en San Juan

---

## Estructura del proyecto

notebooks/

├── 01_exploracion.ipynb              → Diagnóstico, limpieza, taxonomía de marcas

├── 02_pipeline_temporal.ipynb        → Pipeline 7 archivos, 3 visualizaciones temporales

├── 03_Indice_Seleccion_Adversa.ipynb → Construcción ISA, análisis de robustez

└── 04_conclusiones.ipynb             → Síntesis, recomendaciones, conclusión

---

## Stack técnico

![Python](https://img.shields.io/badge/Python-3.11-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange)

Python · Pandas · NumPy · Matplotlib · Seaborn · SciPy · Jupyter · VS Code

---

## Autor

**Rodolfo Gabriel Riveros Lobos**  
Data Analyst Junior | Calidad ISO 9001 · Customer Experience · Mejora Continua  
[LinkedIn](https://linkedin.com/in/rgriveros) · [Portfolio GitHub](https://github.com/RGRIVEROS-PORTFOLIO)