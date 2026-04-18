#  Aplicación de Biológicos 2023

##  Descripción
Este proyecto contiene un respaldo (dump) de una base de datos en PostgreSQL que almacena información sobre la aplicación de vacunas y biológicos en diferentes centros de salud en México durante el año 2023.

El archivo incluye la estructura de la base de datos, la configuración y los datos necesarios para su restauración.

---

##  Objetivo
El propósito de esta base de datos es:

- Registrar la cantidad de vacunas aplicadas  
- Llevar control por entidad y municipio  
- Identificar centros de salud (CLUES)  
- Analizar datos por mes y año  
- Facilitar estudios estadísticos en salud pública  

---

##  Estructura de la Base de Datos

###  Tabla principal
**Nombre:** `aplicacion_biologicos_2023`  

Contiene información detallada sobre la aplicación de vacunas.

---

##  Campos principales

###  Identificación
- `_pk`: Identificador único (clave primaria)

###  Ubicación geográfica
- `clave_entidad`: Código del estado  
- `entidad`: Nombre del estado  
- `clave_municipio`: Código del municipio  
- `municipio`: Nombre del municipio  

###  Centro de salud
- `clues`: Código del establecimiento de salud  
- `nombre_clues`: Nombre del hospital o clínica  

###  Tiempo
- `mes`: Mes de registro  
- `anio`: Año (2023)  
- `fecha`: Fecha completa  

###  Vacunas y biológicos
Ejemplos de columnas:
- `vac06`, `vac12`, `vac13`  
- `bio50`, `bio03`  
- `bie01`, `vbc01`  

Cada una representa la cantidad aplicada de un biológico específico.

### ⏱️ Control de carga
- `_cargado_en`: Fecha y hora de inserción del registro  

---

##  Secuencia

Se utiliza una secuencia para generar automáticamente el identificador `_pk`:

```sql
CREATE SEQUENCE aplicacion_biologicos_2023__pk_seq;
