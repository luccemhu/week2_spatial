# [2-TAREA-1INT46-PUCP](https://luccemhu.github.io/week2_spatial/)

## Diccionario de Datos

Enlace a GitHub Pages: https://luccemhu.github.io/week2_spatial/

Este documento proporciona una descripción de las variables en el conjunto de datos utilizado para el análisis.

| **Variable**              | **Descripción**                                                             | **Tipo de Datos**          | **Ejemplo**              | **Valores**                                                  |
|---------------------------|-----------------------------------------------------------------------------|----------------------------|--------------------------|--------------------------------------------------------------|
| `PROV_HECHO`               | Nombre del lugar o área geográfica.                                          | Texto (String)             | `ABANCAY`                | Nombres de localidades                                       |
| `ANIO`                     | Año en el que se recopilaron los datos.                                      | Numérico (Integer)         | `2018`                   | Años (por ejemplo, 2018, 2019)                               |
| `total_delitos`        | Cantidad total de delitos registrados en el área durante el año especificado.| Numérico (Integer)         | `848`                    | Valores numéricos                                             |
| `geometry`               | Representación geométrica del área geográfica en formato MULTIPOLYGON.       | Texto (String, WKT)        | `MULTIPOLYGON (((-72.91562 ...` | Formato WKT (Well-Known Text)                          |
| `total_q5`      | Clasificación del riesgo basado en el análisis de delitos.                   | Texto (String)             | `5_HighRisk`             | `1_LowRisk`, `2_ModerateRisk`, `3_HighRisk`, `4_VeryHighRisk`, `5_HighRisk` |
| `total_q5_cat`| Clasificación detallada del riesgo para validación.                          | Texto (String)             | `5_HighRisk`             | `1_LowRisk`, `2_ModerateRisk`, `3_HighRisk`, `4_VeryHighRisk`, `5_HighRisk` |

## Ejemplo de Fila de Datos

| PROV_HECHO | ANIO  | total_delitos | geometry       | total_q5 | total_q5_cat |
|-----------|------|-------------------|-----------------|---------------------|--------------------------|
| ABANCAY   | 2018 | 848               | MULTIPOLYGON (((-72.91562 -... | 5_HighRisk          | 5_HighRisk               |


## Descripción Adicional

- **Localidad**: Identifica el nombre del lugar o área.
- **Año**: Indica el año en que los datos fueron recopilados.
- **Número de Delitos**: Representa la cantidad total de delitos reportados.
- **Geometría**: Se utiliza para mapear el área geográfica en herramientas de visualización geoespacial.
- **Categoría de Riesgo**: Clasificación del riesgo basado en la intensidad de los delitos por el método cuantiles.
- **Categoría de Riesgo (Categoría)**: Repetición de la categoría de riesgo para validar consistencia.
