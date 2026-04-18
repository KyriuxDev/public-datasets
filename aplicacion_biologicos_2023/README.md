# Aplicación de Biológicos 2023 

## Descripción
Este conjunto de datos contiene el registro detallado de la aplicación de vacunas y biológicos en centros de salud de México durante el año 2023. La información está organizada por entidad federativa, municipio, unidad médica (CLUES) y periodo mensual.

La base permite conocer cuántas dosis de diferentes vacunas y biológicos fueron aplicadas en cada unidad de salud, facilitando el análisis del comportamiento de la vacunación a lo largo del tiempo.

Este tipo de información es útil para evaluar la cobertura de vacunación, identificar tendencias, analizar la distribución de recursos en salud y apoyar la toma de decisiones en políticas públicas sanitarias.

---

## Diccionario de Datos

Cada registro de esta base de datos incluye las siguientes columnas:

| Columna | Tipo de Dato | Descripción |
|--------|-------------|------------|
| _pk | Bigint | Identificador único del registro (clave primaria). |
| clave_entidad | Integer | Clave numérica de la entidad federativa. |
| entidad | String | Nombre del estado. |
| clave_municipio | Integer | Clave numérica del municipio. |
| municipio | String | Nombre del municipio. |
| clues | String | Código CLUES del establecimiento de salud. |
| nombre_clues | String | Nombre del centro de salud o unidad médica. |
| mes | Numeric | Mes del registro (1 a 12). |
| anio | Numeric | Año del registro (2023). |
| fecha | Date | Fecha correspondiente al registro mensual. |
| bio50, bio03, bio88, bio96, bio97 | Numeric | Cantidad aplicada de biológicos específicos. |
| vac06, vac12, vac13, vac17, vac18, vac19, vac23, vac36, vac38, vac39, vac40, vac43, vac46, vac47, vac48, vac51, vac54, vac55, vac56, vac59, vac62, vac63, vac67, vac68, vac69, vac70, vac81, vac82, vac83, vac84, vac85, vac87, vac91, vac92, vac93, vac94 | Numeric | Cantidad aplicada de diferentes vacunas. |
| bie01 – bie61 | Numeric | Variables asociadas a biológicos o indicadores complementarios. |
| vbc01 – vbc03 | Numeric | Variables de control de biológicos. |
| vhb01 – vhb06 | Numeric | Variables relacionadas con biológicos específicos. |
| vhx01 – vhx04 | Numeric | Variables adicionales de control. |
| vrv01 – vrv04 | Numeric | Variables de registro de vacunas. |
| vnc01 – vnc03 | Numeric | Variables de control de aplicación. |
| vnp01 | Numeric | Variable de biológico específico. |
| vtv01 – vtv03 | Numeric | Variables de vacunación. |
| vph01 – vph04 | Numeric | Variables relacionadas con vacuna VPH. |
| var01 | Numeric | Variable adicional de biológico. |
| vtd01 – vtd36 | Numeric | Variables de seguimiento de dosis aplicadas. |
| _cargado_en | Timestamp | Fecha y hora en que el registro fue cargado al sistema. |

---

## Consideraciones

- Los valores `\N` representan datos nulos (sin información registrada).  
- No todas las columnas tienen datos en todos los registros.  
- Los valores numéricos representan cantidades de dosis aplicadas.  
- La información está organizada de forma mensual por unidad médica.  

---

## Uso de la Base de Datos

Esta base de datos puede utilizarse para:

- Análisis de cobertura de vacunación por región  
- Seguimiento mensual de aplicación de biológicos  
- Estudios epidemiológicos  
- Evaluación del desempeño de unidades de salud  
- Visualización de datos en salud pública  

---

## Fuente de los Datos

Institución: Secretaría de Salud (México)  
Sistema: Registros de aplicación de biológicos en unidades médicas (CLUES)  
Tipo de fuente: Datos administrativos del sector salud  

---

## Notas

Este dataset fue exportado desde PostgreSQL mediante un archivo dump, el cual incluye la estructura de la tabla, secuencias y datos.

Se recomienda su uso en herramientas de análisis de datos o sistemas gestores de bases de datos como PostgreSQL.
