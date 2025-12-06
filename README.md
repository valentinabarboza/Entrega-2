# Determinantes socioeconómicos e institucionales del nivel de incautaciones de drogas (2023)

Repositorio del trabajo final del curso **Estadística para el Análisis Político 2 (POL 304 - 0689)**.

El proyecto analiza cómo factores **institucionales** (democracia, corrupción) y **estructurales** (población, nivel de ingresos económicos) se relacionan con el **nivel de incautaciones de drogas** (kilos incautados) a nivel global en el año 2023, utilizando modelos de regresión y análisis de clúster en R.

---

## 1. Estructura del repositorio

- `data_final.xls`  
  Base de datos integrada con:
  - `kilos_totales` (incautaciones de drogas en kilos).  
  - `democracia` (Electoral Democracy Index – V-Dem).  
  - `corrupcion` (CPI SCORE – Transparency International; valores altos = menor corrupción).  
  - `poblacion` (World Population – Banco Mundial).  
  - `Ningresos` (Income group – clasificación de ingreso del Banco Mundial).

- `DASHBOARD.Rmd` *(si lo tienes con otro nombre, cámbialo aquí)*  
  Script en R Markdown que genera el dashboard interactivo con el análisis descriptivo y los modelos.

- `DASHBOARD.html`  
  Versión compilada del dashboard. Puede abrirse en cualquier navegador.

- `TRABAJO-FINAL.html`  
  Informe final en formato HTML, generado desde R Markdown, con:
  - Introducción y justificación.  
  - Descripción de datos y variables.  
  - Metodología.  
  - Resultados de regresión lineal, regresión logística y clúster.  
  - Conclusiones.

- `README.md`  
  Este documento.

---

