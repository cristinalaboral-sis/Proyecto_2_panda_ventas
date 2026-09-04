# Consolidador y Limpiador de Datos de Ventas

Este proyecto realiza la extracción, consolidación, limpieza y exportación de datos de ventas a partir de fuentes heterogéneas (`ventas.csv` y `productos.xlsx`).

## 📌 Descripción del Proyecto
El flujo de trabajo automatiza las siguientes tareas:
- **Carga de datos:** Importación de fuentes en formato CSV y Excel.
- **Tratamiento de valores nulos:** Imputación/limpieza de datos faltantes en campos críticos.
- **Normalización:** Formateo de tipos de datos (conversión de fechas a `datetime`, eliminación de espacios en blanco en cadenas de texto).
- **Cálculos y Transformación:** Creación de columnas derivadas como `total_venta` (`cantidad` × `precio_unitario`).
- **Exportación:** Generación del dataset final consolidado en formato columnar eficiente `.parquet` (`ventas_consolidadas.parquet`).

## 🛠️ Tecnologías Utilizadas
- **Python 3.x**
- **Pandas** (para la manipulación y análisis de datos)
- **PyArrow / FastParquet** (para la lectura y escritura en formato Parquet)

## 📁 Estructura del Repositorio