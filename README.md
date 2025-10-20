# Entrega-2
# Entrega-2
# Narcotráfico en América (2021–2023): marihuana y cocaína

Este repositorio contiene la organización y limpieza de datos para el curso **Estadística para el análisis político 2**. 
El objetivo es construir un panel país–año para analizar la relación entre producción/oferta (proxys), incautaciones y factores socioeconómicos.

## Alcance
- **Región:** América
- **Sustancias:** Marihuana (cannabis) y cocaína
- **Años:** 2021–2023
- **Unidades geográficas:** País

- ## 🧩 Estructura del repositorio
.
├─ code/
│ └─ 01_limpieza_unificacion.Rmd # Script de limpieza y unificación de bases
├─ data/
│ └─ panel_americas_2021_2023.csv # Base final unificada (limpia)
├─ data_raw/
│ ├─ POBLACIÓN MUNDIAL.xlsx
│ ├─ PBI PER CÁPITA income group.xlsx
│ ├─ V-Dem-CY-Core-v15.csv
│ └─ Cannabis_cultivation_production_and_eradication.xlsx

---

## Reproducibilidad

### Requisitos
- **R (>= 4.2)** y **RStudio**
- Paquetes:  
  `rio`, `dplyr`, `tidyr`, `janitor`, `stringr`, `countrycode`, `readr`, `lubridate`, `purrr`, `ggplot2`

## 📊 Diccionario de datos

| Variable | Tipo | Descripción | Unidad / Escala | Fuente |
|-----------|------|--------------|-----------------|---------|
| `country` | Texto | Nombre del país | — | Derivado |
| `country_iso3` | Texto | Código ISO3 del país | — | Derivado |
| `year` | Numérico | Año de referencia (2021–2023) | Año | Derivado |
| `population` | Numérico | Población total | Personas | Banco Mundial (SP.POP.TOTL) |
| `gdp_pc_current_usd` | Numérico | PBI per cápita en dólares corrientes | USD | Banco Mundial (NY.GDP.PCAP.CD) |
| `gov_index` | Numérico | Índice de gobernanza democrática (V-Dem, v2x_polyarchy) | 0–1 | V-Dem v15 |
| `cultivation_ha` | Numérico | Área cultivada de marihuana | Hectáreas | UNODC – *Cannabis cultivation, production and eradication* |
| `eradication_ha` | Numérico | Área erradicada de cultivos de marihuana | Hectáreas | UNODC |
| `production_tons` | Numérico | Producción estimada de marihuana | Toneladas | UNODC |

---

## 📚 Fuentes de datos
- **UNODC (United Nations Office on Drugs and Crime)**  
- *World Drug Report* y dataset “Cannabis cultivation, production and eradication” (última versión disponible).  
- **Banco Mundial (World Bank Data):**  
- *Population, total (SP.POP.TOTL)*  
- *GDP per capita (current US$) (NY.GDP.PCAP.CD)*  
- **V-Dem Institute (Varieties of Democracy, v15):**  
- Variable `v2x_polyarchy` (democracia electoral).  

---

## 📉 Limitaciones
- La información sobre producción e incautaciones depende de las **capacidades de reporte nacionales**, por lo que puede haber **sesgos de subregistro**.  
- Algunos países carecen de datos completos para los tres años de estudio.  
- Las cifras de incautaciones y producción son aproximaciones indirectas al nivel de narcotráfico.  
- La homogeneización de unidades y conversiones puede afectar la comparabilidad exacta entre países.  

## 👤 Autoría
**Autor:** Luana Valentina Barboza Idrogo  
**Curso:** Estadística para el análisis político 2  





├─ README.md
└─ .gitignore
