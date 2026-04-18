# Transferencias Federales a Entidades Federativas (2011 – Actual)

---

## Descripción

Este conjunto de datos contiene el **historial mensual de los recursos que el Gobierno Federal de México transfiere a cada estado y municipio**, conocidos como *gasto federalizado*. Los datos fueron publicados por la **Secretaría de Hacienda y Crédito Público (SHCP)** y van desde enero de 2011 hasta los datos más recientes disponibles (enero 2026).

En México, los estados dependen en gran medida del presupuesto federal. Este gasto federalizado se distribuye principalmente a través de dos mecanismos: las **Participaciones Federales (Ramo 28)**, que son recursos sin destino etiquetado que cada estado puede gastar libremente, y las **Aportaciones Federales (Ramo 33)**, que son recursos con destino específico (educación, salud, infraestructura social, seguridad pública, etc.). También se incluyen recursos del **Ramo 23** (Provisiones Salariales y Económicas) y convenios de descentralización.

---

## Diccionario de Datos

Cada registro de esta base de datos incluye las siguientes columnas:

| Columna | Tipo de Dato | Descripción |
| :--- | :--- | :--- |
| **`CICLO`** | `Integer` | Año fiscal al que corresponde la transferencia. |
| **`MES`** | `String` | Mes en que se realizó la transferencia (ej. *Enero*, *Febrero*). |
| **`CLAVE_DE_CONCEPTO`** | `String` | Código alfanumérico único que identifica el concepto de transferencia para cada entidad (ej. `XAC2808`). |
| **`NOMBRE`** | `String` | Descripción completa del concepto, incluye el nombre del estado y el tipo de recurso (ej. *Chihuahua: Participaciones a Entidades Federativas y Municipios (R28)*). |
| **`TEMA`** | `String` | Agrupación temática del recurso (ej. *Transferencias del Gobierno Federal a Entidades Federativas y Municipios*). |
| **`SUBTEMA`** | `String` | Clasificación dentro del tema (ej. *Participaciones*, *Aportaciones*). |
| **`SECTOR`** | `String` | Sector del gobierno al que pertenece el recurso (ej. *Gobierno Federal Presupuestario*). |
| **`AMBITO`** | `String` | Nivel de gobierno de origen del recurso (ej. *Federal*). |
| **`TIPO_DE_INFORMACION`** | `String` | Indica si el dato es un *Flujo* (monto en el periodo) o un acumulado. |
| **`BASE_DE_REGISTRO`** | `String` | Momento contable en que se registra (ej. *Pagado*). |
| **`UNIDAD_DE_MEDIDA`** | `String` | Unidad en que se expresa el monto (siempre *Miles de Pesos*). |
| **`PERIODO_INICIO`** | `String` | Fecha de inicio de la serie histórica para ese concepto (formato `YYYY-MM`). |
| **`PERIODO_FINAL`** | `String` | Fecha de fin de la serie histórica disponible para ese concepto (formato `YYYY-MM`). |
| **`FRECUENCIA`** | `String` | Periodicidad de la publicación del dato (ej. *Mensual*). |
| **`DIFUSION`** | `String` | Plazo oficial de publicación del dato (ej. *30 días después del cierre del mes de referencia*). |
| **`MONTO`** | `Numeric` | Importe transferido en el periodo, expresado en miles de pesos corrientes. |

---

## Fuente de los Datos

* **Institución:** Secretaría de Hacienda y Crédito Público (SHCP)
* **Enlace Oficial:** [datos.gob.mx – Transferencias a Entidades Federativas](https://www.datos.gob.mx/dataset/transferencias_entidades_federativas_2011_actual)