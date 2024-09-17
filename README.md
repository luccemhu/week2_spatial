# 2-TAREA-1INT46-PUCP

## Diccionario de Datos

Enlace a GitHub Pages: https://luccemhu.github.io/1-TAREA-1INT46-PUCP/

Este documento proporciona una descripción de las variables en el conjunto de datos utilizado para el análisis. Cada variable se detalla a continuación.

## Variables

### Localidad
- **Descripción**: Nombre del lugar o área geográfica.
- **Tipo de Datos**: Texto (String)
- **Ejemplo**: `ABANCAY`

### Año
- **Descripción**: Año en el que se recopilaron los datos.
- **Tipo de Datos**: Numérico (Integer)
- **Ejemplo**: `2018`

### Número de Delitos
- **Descripción**: Cantidad total de delitos registrados en el área durante el año especificado.
- **Tipo de Datos**: Numérico (Integer)
- **Ejemplo**: `848`

### Geometría
- **Descripción**: Representación geométrica del área geográfica en formato MULTIPOLYGON. Utilizado para la visualización espacial.
- **Tipo de Datos**: Texto (String) en formato WKT (Well-Known Text)
- **Ejemplo**: `MULTIPOLYGON (((-72.91562 -...`

### Categoría de Riesgo
- **Descripción**: Clasificación del riesgo basado en el análisis de los datos de delitos.
- **Tipo de Datos**: Texto (String)
- **Posibles Valores**: 
  - `1_LowRisk`
  - `2_ModerateRisk`
  - `3_HighRisk`
  - `4_VeryHighRisk`
  - `5_HighRisk`
- **Ejemplo**: `5_HighRisk`

### Categoría de Riesgo (Categoría)
- **Descripción**: Categoría de riesgo detallada asociada al área geográfica.
- **Tipo de Datos**: Texto (String)
- **Posibles Valores**: 
  - `1_LowRisk`
  - `2_ModerateRisk`
  - `3_HighRisk`
  - `4_VeryHighRisk`
  - `5_HighRisk`
- **Ejemplo**: `5_HighRisk`

## Ejemplo de Fila de Datos

| Localidad | Año  | Número de Delitos | Geometría       | Categoría de Riesgo | Categoría de Riesgo (Categoría) |
|-----------|------|-------------------|-----------------|---------------------|--------------------------------|
| ABANCAY   | 2018 | 848               | MULTIPOLYGON (((-72.91562 -... | 5_HighRisk          | 5_HighRisk                      |

## Descripción Adicional

- **Localidad**: Identifica el nombre del lugar o área.
- **Año**: Indica el año en que los datos fueron recopilados.
- **Número de Delitos**: Representa la cantidad total de delitos reportados.
- **Geometría**: Se utiliza para mapear el área geográfica en herramientas de visualización geoespacial.
- **Categoría de Riesgo**: Clasificación del riesgo basado en la intensidad de los delitos.
- **Categoría de Riesgo (Categoría)**: Repetición de la categoría de riesgo para validar consistencia.
