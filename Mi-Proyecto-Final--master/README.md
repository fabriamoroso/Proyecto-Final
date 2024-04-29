# Data-Science Project -  Rendimiento de los Cultivos
==============================

## Resumen
En este proyecto se trabajará con dos Dataset.  El primero provisto por el Servicio Meteorologíco de la Republica Argentina y el segundo dataset proviene de la Subsecretaria de Agricultura, Dirección Nacional de Agricultura, Dirección de Estimaciones Agrícolas. En el siguiente link puede encontrarse el dataset https://datosestimaciones.magyp.gob.ar/reportes.php?reporte=Estimaciones y https://www.argentina.gob.ar/smn/institucional/contacto.

El dataset provisto por la Subsecretaria de Agricultura contiene una serie de estadística agrícola por cultivo, campaña, provincia y departamento de la República Argentina con los siguientes datos: superficie sembrada, superficie cosechada, producción y rendimiento. Las superficies se muestran en hectáreas, la producción en toneladas y el rendimiento en kg/ha.
El segundo dataset provisto por el Servicio Meteorologíco contiene la temperatura diaria desde 1988 al 2022 de Junin y Tres Arroyos tanto en tanto las precipitaciones  y temperatura máxima, media, mínima.  

## Objetivo de la Investigación
El objetivo de este trabajo es poder implementar un algoritmo predictivo de machine learning que permita conocer los valores futuros de los cultivos en estudio en determinados departamentos, así como también responder a una serie de preguntas: ¿El rendimiento de los cultivos tiene un comportamiento predecible con respecto a otras variables? ¿Cúal será el rendimiento en un determinado periodo de tiempo? ¿Existe estacionalidad en los rendimientos? ¿Cómo son esos ciclos, si es que hay? ¿Es posible predecir el valor de una variable mediante el uso de otra?. Por supuesto que en la medida que se avance en el trabajo podrán surgir nuevas interrogantes.



## Criterio de selección
Se definio para abordar la problematica en dividir la provincia de Bs As en dos grandes sectores (Norte - Sur), debido a la gran extensión de territorio y diferencia de suelo.  Se tomo las precipitaciones de dos departamentos (Junin - Tres Arroyos), y se considero las zonas con cercania de 60km.  Ademas, se consideraron los cultivos más significantes en Provincia tales como Avena, Cebada cervecera, Girasol, Maiz, Soja 1ra, Soja 2da, Soja total, Sorgo y Trigo.


## Diccionario de Variables
A continuación se brinda el listado de variables utilizadas en el proyecto:
-Estimaciones (Provincia de BsAs 1987-2022.csv)
°Cultivo: Tipos de cultivos
°Campaña: Periodo de tiempo de duración del rendimiento
°Provincia: División administrativa en que se organiza el Estado
°Departamento: Los Departamentos y partidos son las subdivisiones de segundo orden de una provincia
°idprovincia: número asignado a cada Provincia
°iddepartamento: número asignado a cada Departamento
°Sup.Sembrada: Superficie en héctarea sembrada
°Sup.Cosechada: Superficie en héctarea cosechada
°Producción: Toneladas de producción
°Rendimiento: El rendimiento se expresa kg/héctarea

-192602 TRES ARROYOS 1988-2022.xlsx / 192602 JUNIN AERO 1988-2022.xlsx
°Fecha: dd/mm/aaaa
°Temperatura máxima: mediciones en centrigrados
°Temperatura media:  mediciones en centrigrados
°Temperatura minima: mediciones en centrigrados
°Precipitación: mediciones en milimetros 

------------

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc. -https://prezi.com/view/SYtG8Y0j2evRCRi3FCsG/
    │   
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── utils.py           <- makes pip installed
  
    │   │
  

--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
