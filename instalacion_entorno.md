## Construcción del entorno de conda

Crearemos el entorno a través del siguiente comando:

```
conda env create -f tdd_pra2.yml
```

Posteriormente activaremos el entorno para poder realizar el registro del nuevo entorno en jupyter y utilizarlo como un kernel más.

```
conda activate tdd_pra2
python -m ipykernel install --user --name=tdd_pra2
conda deactivate
```

Una vez instalado el kernel en jupyter podemos volver al entorno base de conda y ejecutar desde él `jupyter lab`, el nuevo kernel nos aparecerá entre las opciones

## Actualizar el entorno

Cuando se añade alguna dependencia en el fichero conda hay que ejecutar el siguiente comando para instalar esas actualizaciones:

```
conda env update -f tdd_pra2.yml
```

## Eliminación del entorno

Para eliminar completamente el entorno tendremos que eliminar el kernel de jupyter y posteriormente el entorno de conda:

```
jupyter kernelspec remove tdd_pra2
conda env remove -y --name tdd_pra2
```

