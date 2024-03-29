# Proyecto de Ejemplo Data Science

## Estructura del Proyecto

```
├───data
│   ├───input
│   │   ├───datos_a_trabajar.csv
│   │   ├───datos_a_trabajar.gzip
│   │   └─── ...
│   └───output
│       ├───models_metrics.csv
│       └───uplift.csv
├───ds_project
│   ├───notebooks
│   │   ├───eda.ipynb
│   │   ├───metrics.ipynb
│   │   └───models.ipynb
│   ├───metrics.py
│   ├───models.py
│   └───utils.py
├───images
│   └───metrics
│       ├───curva_roc.png
│       ├───feature_importance.png
│       └───uplift.png
├───models
│   └───model.pkl
├───.gitignore
├───poetry.lock
├───poetry.toml
└────README.md
```

### Carpetas:

- **data**: Almacena datos utilizados en el proyecto. Suele estar dividido en subcarpetas:
  - **input**: Contiene datos de entrada, como archivos CSV, bases de datos o cualquier información relevante que se utilice para el análisis o modelado.
  - **output**: Contiene los resultados generados durante el análisis o modelado, como archivos de resultados, métricas, o cualquier otro tipo de salida.

- **ds_project**: Directorio principal del proyecto.
  - **notebooks**: Contiene notebooks de Jupyter, que pueden incluir análisis exploratorio de datos, pruebas de modelos, visualizaciones, entre otros.
  - **metrics.py**: Un archivo de Python que puede contener funciones o clases para calcular métricas específicas utilizadas en el proyecto.
  - **models.py**: Archivo que puede contener definiciones de modelos de Machine Learning o funciones relacionadas con el entrenamiento y evaluación de modelos.
  - **utils.py**: Archivo que alberga funciones o utilidades compartidas en todo el proyecto.

- **images**: Almacena imágenes o gráficos generados durante el análisis de datos, visualizaciones o resultados de modelos.
  - **metrics**: Carpeta específica para imágenes relacionadas con las métricas o evaluación de modelos.

- **models**: Contiene modelos entrenados guardados en archivos, como archivos de modelo serializados (por ejemplo, pickle, joblib) o archivos guardados en formatos específicos para modelos de Machine Learning.

### Archivos:

- **.gitignore**: Archivo que enumera los archivos y carpetas que se deben ignorar en el control de versiones mediante Git.
- **poetry.lock**: Archivo generado por la herramienta de manejo de dependencias Poetry, que detalla las versiones específicas de las dependencias del proyecto.
- **poetry.toml**: Archivo de configuración de Poetry que contiene información sobre el proyecto y sus dependencias.
- **README.md**: Archivo de documentación que proporciona información general sobre el proyecto, su estructura y cómo ejecutarlo.

## Nota

*  Los archivos utilizados en este ejemplo se encuentran disponibles en el siguiente [enlace de Sharepoint](https://gruposecurity.sharepoint.com/:f:/r/sites/GR/analitica_avanzada/Documentos%20compartidos/C%C3%A9lula%20Vida/input?csf=1&web=1&e=mPItpm).
* En la sección de `eda.ipynb`, se emplean los datos del archivo **master.gzip**, mientras que para la sección de `models.ipynb`, se utilizan los conjuntos de datos **train.gzip** y **test.gzip**. En consecuencia, es necesario crear tanto el archivo master como los conjuntos de datos de entrenamiento y prueba.

## TO-DO (Cosas por Hacer)

* Flujo de trabajo con azure devops
* Agregar Pre-commit, testing y documentación
* Automatizar flujo con Azureml
