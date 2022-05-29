# Rent prices analysis

## Descripción 🚀

Repositorio realizado para la práctica 2 de web scraping de la asignatura _Tipología y ciclo de vida de los datos_ del Máster en Ciencia de Datos de la [Universitat Oberta de Catalunya](https://www.uoc.edu/portal/en/index.html).

## Objetivo 🚀

Este repositorio consiste en una segunda parte de proyecto ya iniciado en la práctica 1, en donde, si accedemos al [repositorio](https://github.com/jvruoc/rent_prices), se ve que el objetivo fue extraer las características de determinados pisos en alquiler en la web de Fotocasa.

Por lo tanto, los objetivos a aplicar en este proyecto es analizar dicha información obtenida previamente.

## Contenido 📦

Finalmente el proyecto generado se distribuye con el siguiente árbol de directorios:

```
rent_prices_analysis
├── pdf
│   ├── images
│   │   ├── seleccion_datos_regresión.png
│   │   └── seleccion_datos.png
│   ├── Memoria final - Limpieza y análisis de datos.pdf
│   ├── Memoria final - Limpieza y análisis de datos.ipynb
│   └── README.md
├── data
│   ├── madrid-rent-prices_4-8_cleaned.parquet
│   ├── madrid-rent-prices_4-abr_cleaned.parquet
│   ├── madrid-rent-prices_cleaned.csv
│   ├── madrid-rent-prices_cleaned.parquet
│   ├── madrid-rent-prices_raw.csv
│   ├── MADRID.geojson
│   └── README.md
├── src
│   ├── analysis.ipynb
│   ├── cleaning.ipynb
│   ├── model_regression.ipynb
│   ├── pruebas_model_classification.ipynb
│   └── pruebas_model_regression-perceptron.ipynb
├── tdd_pra2.yml
└── README.md
```

Dentro de estos se destacan las siguientes carpetas

* _**src**_ : Carpeta con todo el código realizado de las diferentes metodologías y pruebas aplicadas.

* _**data**_ : Carpeta los diferentes conjuntos de datos generados a lo largo de los procedimientos.

* _**pdf**_ : Carpeta donde se encuentra el documento final y todos los recursos necesarios para generarlo.

## Entorno de conda

Se ha construido un entorno de _conda_ a través del siguiente comando:

```
conda env create -f tdd_pra2.yml
```

Posteriormente activaremos el entorno para poder realizar el registro del nuevo entorno en jupyter y utilizarlo como un kernel más.

```
conda activate tdd_pra2
python -m ipykernel install --user --name=tdd_pra2
```

Una vez instalado el kernel en jupyter podemos volver al entorno base de conda y ejecutar desde el `jupyter lab`, el nuevo kernel nos aparecerá entre las opciones

### Desactivar el Entorno

Con el fin de desactivar el entorno se ejecuta el siguiente comando.

```
conda deactivate
```

### Actualizar el entorno

Cuando se añade alguna dependencia en el fichero conda hay que ejecutar el siguiente comando para instalar esas actualizaciones:

```
conda env update -f tdd_pra2.yml
```

### Eliminación del entorno

Para eliminar completamente el entorno tendremos que eliminar el kernel de jupyter y posteriormente el entorno de conda:

```
jupyter kernelspec remove tdd_pra2
conda env remove -y --name tdd_pra2
```

## Autores ✒️

* [Jose Ventura Roda](https://www.linkedin.com/in/joseventuraroda/)
* [Kevin Martín Chinea](https://www.linkedin.com/in/kevmch/)
