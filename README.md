## Análisis de Movilidad en El Salvador durante la Pandemia (Proyectos ETL y OLAP)

Este repositorio contiene dos proyectos complementarios centrados en el análisis de la movilidad en El Salvador durante la pandemia por COVID-19, utilizando datos extraídos de informes públicos de Google Mobility.

### Proyecto 1: ETL y Preparación de Datos

Este proyecto se enfoca en la construcción de un flujo ETL (Extracción, Transformación y Carga) para depurar y estructurar los datos originales en formato CSV. Los datos son limpiados, normalizados y adaptados para ser almacenados en una base de datos relacional, permitiendo una posterior explotación analítica.

Funcionalidades principales:
- Limpieza y transformación de datos de movilidad.
- Conversión de fechas y unificación de nombres de departamentos.
- Inserción en tablas SQL bien estructuradas para análisis posterior.

---

### Proyecto 2: Cubo OLAP y Consultas Analíticas

Este segundo proyecto modela los datos preparados en un **cubo OLAP**, permitiendo consultas multidimensionales sobre distintas dimensiones como departamento, mes y categoría de movilidad (supermercados, farmacias, parques, etc.). Se integran consultas SQL para explorar patrones de comportamiento durante el confinamiento.

Funcionalidades principales:
- Diseño de un esquema estrella para análisis multidimensional.
- Construcción del cubo OLAP con medidas e indicadores clave.
- Consultas SQL para extraer conclusiones sociales y territoriales.

---

### Consideraciones para ejecutar los proyectos

Antes de ejecutar los scripts de transformación o análisis, asegurarse de:

1. Contar con el archivo CSV global de movilidad (`Global_Mobility_Report.csv` o equivalente).
2. Tener una base de datos configurada con todas las **tablas necesarias** utilizadas en el proyecto (según el esquema proporcionado en los scripts SQL).
3. Tener acceso a un entorno con soporte para SQL (MySQL/PostgreSQL) y herramientas como Power BI o Excel para visualizar el cubo OLAP.

