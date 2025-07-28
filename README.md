# Alura Store - Análisis de Datos

Este proyecto contiene un análisis exploratorio de las ventas de **Alura Store** para el *challenge* de Data Science de Alura Latam. El notebook `AluraStoreLatam.ipynb` descarga y procesa las bases de datos de las cuatro tiendas de la compañía.

## Propósito del análisis

El objetivo es comprender el comportamiento de las ventas y extraer insights relevantes, tales como:

- Ingresos totales por tienda.
- Ventas por categoría de producto.
- Calificación promedio obtenida por cada tienda.
- Productos más y menos vendidos.
- Promedio de costo de envío por tienda.

## Estructura del proyecto

```
Alura_Store/
├── AluraStoreLatam.ipynb  # Notebook con todo el análisis
└── README.md              # Este archivo
```

## Ejemplos de gráficos e insights

A lo largo del notebook se realizan distintos cálculos y visualizaciones. Algunos ejemplos son:

- **Ingresos por tienda**: se calcula la suma del precio de todos los productos para cada tienda y se muestra en un gráfico de barras horizontal.
- **Ventas por categoría**: mediante la función `ventas_categoria` se generan gráficos de barras que muestran cuántos productos de cada categoría se vendieron en cada tienda.
- **Calificación promedio**: se obtiene el promedio de la columna `Calificación` para cada tienda, resultando valores cercanos a 4 estrellas.
- **Producto más y menos vendido**: la función `producto_max_min` indica cuáles fueron los artículos con mayor y menor cantidad de ventas, por ejemplo en la tienda 4 el artículo más vendido fue `Cama box`.
- **Envío promedio**: se calcula el promedio del `Costo de envío` de cada tienda.

Estos cálculos pueden verse en el notebook en celdas como la que genera el diccionario de ingresos totales:

```
{'Tienda 1': 1150880400.0, 'Tienda 2': 1116343500.0, 'Tienda 3': 1098019600.0, 'Tienda 4': 1038375700.0}
```

Y también en la salida final del promedio de costo de envío:

```
{'Tienda 1': 23459.4572,
 'Tienda 2': 25216.2357,
 'Tienda 3': 24805.6804,
 'Tienda 4': 23459.4572}
```

## Cómo ejecutar el notebook

1. Asegúrate de tener instalado Python con Jupyter Notebook (o JupyterLab). También puedes abrirlo directamente en Google Colab.
2. Abre `AluraStoreLatam.ipynb` y ejecuta las celdas en orden. El notebook descargará automáticamente los archivos CSV desde GitHub y realizará todo el análisis.
3. Revisa cada sección para observar los gráficos generados y los insights obtenidos.

¡Listo! Con esto podrás replicar y modificar el análisis según tus necesidades.
