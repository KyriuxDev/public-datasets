# Incidencia Delictiva Estatal (México, 2015 – Diciembre 2025)

---

## Descripción

Este conjunto de datos contiene el registro histórico de los **presuntos delitos denunciados en México a nivel estatal**, organizados por tipo, subtipo y modalidad de delito. Los datos fueron publicados por el **Secretariado Ejecutivo del Sistema Nacional de Seguridad Pública (SESNSP)** y cubren desde enero de 2015 hasta diciembre de 2025.

---

## Diccionario de Datos

Cada registro de esta base de datos incluye las siguientes columnas:

| Columna | Tipo de Dato | Descripción |
| :--- | :--- | :--- |
| **`Año`** | `Integer` | Año en que se registraron las carpetas de investigación. |
| **`Clave_Ent`** | `Integer` | Clave numérica oficial (INEGI) de la entidad federativa. |
| **`Entidad`** | `String` | Nombre del estado o entidad federativa donde ocurrió el delito. |
| **`Bien jurídico afectado`** | `String` | Categoría legal más amplia del delito (ej. *La vida y la integridad corporal*, *El patrimonio*, *La libertad personal*). |
| **`Tipo de delito`** | `String` | Clasificación general del delito dentro del bien jurídico afectado (ej. *Homicidio*, *Robo*, *Secuestro*). |
| **`Subtipo de delito`** | `String` | Especificación del tipo de delito (ej. *Homicidio doloso*, *Robo a casa habitación*). |
| **`Modalidad`** | `String` | Detalle adicional sobre cómo se cometió el delito (ej. *Con violencia*, *Sin violencia*, *Con arma de fuego*). |
| **`Mes`** | `String` | Mes de la incidencia |
| **`Fecha`** | `Date` | Fecha en la que ocurrió el delito ordenado en DD/MM/YYYY|
| **`Incidencia`** | `Integer` | Número de carpetas de investigación iniciadas en cada mes del año correspondiente. Hay una columna por cada mes. |
| **`Entidad federativa`** | `String` | Nombre del estado o entidad federativa donde ocurrió el delito. |
---

## Fuente de los Datos

* **Institución:** Secretariado Ejecutivo del Sistema Nacional de Seguridad Pública (SESNSP)

* **Enlace Oficial:** [datos.gob.mx – Incidencia Delictiva](https://www.datos.gob.mx/dataset/incidencia_delictiva)
