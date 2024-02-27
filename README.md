# <p align="center"> Proyecto Individual No. 2
# <p align="center"> Data Analytics</p>
<p align="center"> Realizado por:</p>

**<p align="center"> Luis David Rojas Díaz</p>**
<p align="center"> Estudiante</p>
<p align="center">
  <img src="Imágenes\Imagen1.png">
</p>

## Descripción del Proyecto

El Proyecto Individual No. 2 está centrado en Data Analytics **(Análisis de Datos)**, el objetivo principal es realizar el análisis sobre los datos adquiridos desde la página de Buenos Aires Data sobre los Siniestros Viales (Homicidios y Lesiones), teniendo a disposición la información del Observatorio de Movilidad y Seguridad Vial (OMSV) que es una dependencia de la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires. El propósito es que en el rol de Data Analytics, se genere información relevante que le permita a las autoridades locales tomar medidas para disminuir la cantidad de víctimas fatales por siniestros viales.

Lo anterior se contextualiza en que en Argentina mueren cerca de 4.000 personas cada año en siniestros viales y que la probabilidad de que una persona muera en un siniestro vial es de 2 o 3 veces más que en un hecho de inseguridad delictiva.

Así que en este proyecto se caracterizan los hechos y las victimas para entender la naturaleza de las victimas y presuntos victimarios. También se analiza en qué lugares ocurren y cuando ocurren los hechos, entendiendo un poco más del contexto de los accidentes leves, graves y fatales.

<p align="center">
  <img src="Imágenes\Readme.jpg">
</p>


<a href="https://www.python.org/">![Python](https://img.shields.io/badge/Python-3.10.11-3776AB?style=for-the-badge&logo=Python)</a>
<a href="https://numpy.org/">![NumPy](https://img.shields.io/badge/NumPy-1.23.5-013243?style=for-the-badge&logo=numpy)</a>
<a href="https://jupyter.org/">![Jupyter Notebook](https://img.shields.io/badge/Jupyter_Notebook-1.1.2-F37626?style=for-the-badge&logo=jupyter)</a>
<a href="https://pandas.pydata.org/">![Pandas](https://img.shields.io/badge/Pandas-2.1.4-150458?style=for-the-badge&logo=pandas)</a>
<a href="https://matplotlib.org">![matplotlib](https://img.shields.io/badge/matplotlib-3.7.2-4285F4?style=for-the-badge&logo=exordo)</a>
<a href="https://docs.python.org/3/library/urllib.html">![urllib](https://img.shields.io/badge/urllib-3.9.2-FFD43B?style=for-the-badge&logo=python)</a>
<a href="https://openpyxl.readthedocs.io/en/stable/">![openpyxl](https://img.shields.io/badge/openpyxl-3.1.10-009688?style=for-the-badge&logo=python)</a>
<a href="https://pyproj4.github.io/pyproj/stable/">![pyproj](https://img.shields.io/badge/pyproj-3.2.1-4E9A06?style=for-the-badge&logo=python)</a>
<a href="https://docs.python.org/3/library/warnings.html">![warnings](https://img.shields.io/badge/warnings-3.0.0-FF9800?style=for-the-badge&logo=python)</a>


### Datos del proyecto (originales y generados)

| Carpeta        | Tipo      | Nombre              | Formato | Descripción                                       |
|----------------|-----------|---------------------|---------|---------------------------------------------------|
| Datos_Originales  | Documento | [Homicidios_CABA](Datos_Originales/Homicidios_CABA.xlsx)  | xlsx   | Archivo Homicidios descargado de Buenos Aires Data |
| Datos_Originales  | Documento | [Lesiones_CABA](Datos_Originales/Lesiones_CABA.xlsx) | xlsx  | Archivo Lesiones descargado de Buenos Aires Data      |
| Datos_Originales  | Documento | [Población_CABA](Datos_Originales/Población_CABA.xlsx) | xlsx | Archivo de Población por comuna descargado de INDEC |
| Datos_limpios   | Documento | [Hechos_Homicidios](Datos_limpios/Hechos_Homicidios_CABA.csv) | csv     | Archivo revisado en el ETL_Siniestros_Viales.ipynb de Homicidios_CABA.csv |
| Datos_limpios   | Documento | [Hechos_Lesiones_CABA](Datos_limpios/Hechos_Lesiones_CABA.csv)| csv     | Archivo revisado en el ETL_Lesiones_No_Fatales.ipynb de Lesiones_CABA|
| Datos_limpios   | Documento | [Población_CABA](Datos_limpios/Población_CABA.csv) | csv     | Archivo revisado en el ETL_Población_CABA.ipynb de los datos originales de Población_CABA|
| Datos_limpios    | Documento | [Víctimas_Homicidios_CABA](Datos_limpios/Victimas_Homicidios_CABA.csv)       | csv     | Archivo revisado en el ETL_Siniestros_Viales.ipynb de Homicidios_CABA|
| Datos_limpios     | Documento | [Víctimas_LESIONES_CABA](Datos_limpios/Victimas_Lesiones_CABA.csv)| csv     | Archivo revisado en el ETL_Lesiones_No_Fatales.ipynb de Lesiones_CABA|
| Datos_Dashborad| Documento | [Siniestros_Viales](Datos_Dashboard/Siniestros_Viales.csv) | csv| Unión de los archivos de Hechos y Víctimas revisado en el ETL_General.ipynb |
| Datos_Dashborad| Documento | [Población](Datos_Dashboard/Poblacion.csv)| csv     | Originado del ETL de Población_CABA.csv.csv  revisado en el ETL_General.ipynb |
| --             | Notebook | [1. ETL_Siniestros_Viales](<1. ETL_Siniestros_Viales.ipynb>) | ipynb | Notebook del ETL de los datos originales de Homicidios (directo de la web) |
| --             | Notebook |[2. ETL_Lesiones_NO_Fatales](<2. ETL_Lesiones_No_Fatales.ipynb>)              | ipynb   | Notebook del ETL de los datos originales de Lesiones (directo de la web)   |
| --             | Notebook |[3. ETL_Población_CABA](<3. ETL_Población_CABA.ipynb>) | ipynb   | Notebook del ETL de los datos originales de Población (directo de la web) |
| --             | Notebook | [4. ETL_General](<4. ETL_General.ipynb>) | ipynb | Notebook sobre uniones de todos los archivos|
| --             | Notebook | [5. EDA_Siniestros_Viales](<5. EDA_Siniestros_Viales.ipynb>) | ipynb | Notebook para el análisis exploratorio de datos en general |
| --             | Dashboard | [Dashboard_PIDA_Siniestros_Viales](Dashboard_PIDA_Siniestros_Viales.pbix)   | pbix      | Dashboard donde se expone el análisis de los datos e información |


_Se asigna "--" a los archivos que no se encuentran dentro de ninguna carpeta del repositorio actual._

## Desarrollo del Proyecto

### 1. Extracción, Transformación y Limpieza de Datos

*"Es de aclarar que aunque se incia con los ETL, en estos documento inmersamente se debió realizar una exploración básica"*

inicialmente se descargan los datos directamente de la página de [CABA buenos aires](https://data.buenosaires.gob.ar/dataset/victimas-siniestros-viales), en donde se extraen los datos y se guardan como respaldo en la carpeta "Datos_Originales". Se descargaron dos archivos de excel, uno que contiene  los datos de siniestros viales que terminaron en fatalidad (Homicidio) y el otro archivo que contiene los datos de lesiones graves y leves en siniestros viales. A través de la página de [INDEC](https://censo.gob.ar/index.php/datos_definitivos_caba/) (Instituto Nacional de Estadística y Censo de la República de Argentina) se obtienen los datos de la población por comuna para poder crear y analizar los datos con respecto de la población.

En el [ETL_Siniestros_Viales.ipynb](<1. ETL_Siniestros_Viales.ipynb>) se revisó el archivo de excel de Homicidios de la página de Buenos Aires Data y se conformaron dos archivos, uno de hechos y otro de víctimas guardados en "Datos_Limpios".

En el [ETL_Lesiones_No_fatales.ipynb](<2. ETL_Lesiones_No_Fatales.ipynb>) se revisó el archivo de excel de Lesiones e igualmente que lo hecho con el archivo anterior se obtubvieron dos archivos, uno de hechos y otro de víctimas guardados en "Datos_Limpios".

En ambos casos solo re relizan transformaciones evidentes y mínimas sobre algunos registros en cero "0" y nulos. Se aprovecha para hacer una exploración rápida. En el caso del ETL_Lesiones_No_Fatales se requirió transformar coordenadas planas a coordenadas mundiales, para rescatar parte de la infromación.

En el [ETL_Población_CABA](<3. ETL_Población_CABA.ipynb>) se revisa el archivo de población por comuna; como el censo se realiza cada cada 12 años, se utiliza la variación por comuna considerandola lineal para crear una tabla con la información por comuna, año y población.

En el [ETL General](<4. ETL_General.ipynb>) se realizan las transformaciones necesarias para llevar los datos a una estructura más flexible en la herramienta de visualización, en este caso para Power Bi.

En este notebook se realizaron los siguientes pasos:
- Revisión de los periodos de fecha para los archivos de Homicidios y Lesiones (se encuetra que los homicidios cuentan con datos del 2016 hasta el 2021 y para el caso de Lesiones desde el año 2019 al 2021).
- Unión de los archivos Hechos Homicidios y Hechos Lesiones.
- Unión de los archivos Víctimas Homicidios y Víctimas lesiones.
- Corrección de formatos de número, fechas y coordenadas.
- Estandarización de valores para que coincidan entre los diferentes dataframe que fueron unidos.
- Imputación de datos nulos que tuvieran coincidencias en otras columnas (ej: comuna vs dirección)
- En el archivo de Población se discriminaron los datos por semestre para facilitar el calculo de indicadores.
- Se creó una columna que mide la tasa de homicidios en siniestros viales (THSV) por cada 100.000 habitantes
- Se crea también un índice que mide la variación de esta tasa por semestre.
- Se crea una columna que mide la variación del índice de siniestros mortales en moto semestral.
- Finalmente se obtinen dos archivos (Siniestros_Viales.csv y Poblacion.csv) que son usados en la herramienta de visualización (los datos se guarda en la carpeta "Datos_Dashboard").

### 2. EDA de los archivos para el Dashboard

*"Se debe tener en cuenta, que al realizar el EDA fué necesario realizar transformaciones incluso mayores en los archivos de ETL"*

En este [notebook](<5. EDA_Siniestros_Viales.ipynb>) se realizaron los siguientes pasos:

- Revisión e imputación de registros nulos o datos con "SD".
- Revisión de registros duplicados (solo se elimnaron registros donde en el mismo hecho ("ID") la víctima era moto, tenían más de 3 pasajeros (preuntamente) y en los datos de registros de víctimas habían coincidencias entre edad y sexo).
- Corrección del formato corresponidiente a los datos.
- Creación de columnas auxiliares de Fecha y hora (AA, MM, DD, HR), las había eliminado pero son necesarias para agrupar los datos en los gráficos.
- Análisis de Información:
    - Clasificación de Víctimas por el tipo de vehículo.
    - Clasificación de Víctimas por Sexo.
    - Clasificación de Víctimas por Tipo de Calle.
    - Clasificación de Víctimas por Comuna.
    - Clasificación de Víctimas por Rol de la Víctima.
    - Clasificación de Víctimas por Sexo y Rango Etario.
    - Clasificación de Víctimas por Vehículo presunto Acusado.
    - Mapa de Calor de los Sinestro Fatales y Lesiones.
    - Evolución del índice de muertes en siniestros viales en general y en moto.
    - Revisón de la correlación de los datos numéricos.

### 3. Dashborad Siniestros Viales

Con base ne los datos guardados en la carpeta "Datos_Dashboard" se creó un dashboard con las siguientes características:

- Portada que contextualiza la inforación de manera rápida y presenta la empresa (ficticia) que desarrola el proyecto.
- Dashborad con la información general de los siniestros viales que caracterizan los hechos según la gravedad, los vehículos implicados, el rol, sexo y edad de la víctima.
- Dashborad con la descripción del lugar de los hechos.
- Dashborad con la descripción del momento o línea temporal de los hechos (Año, Mes, Día y Horario)
- Indicador clave de desempeño (KPI-1) para la variación de la tas de siniestros viales con meta de disminución del 10% semestral.
- Indicador clave de desempeño (KPI-2) para la variación del índice del número de muertos por accidentes fatales en moto con meta de disminución del 7% anual.
- Indicador clave de desempeño (KPI-3) para la variación del índice del número de muertos por accidentes fatales en peatones con meta de disminución del 10% anual.

Vista general del [dasrborad](Dashboard_PIDA_Siniestros_Viales.pbix) a continuación:

<p align="center">
  <img src="Imágenes\Dashboard.gif">
</p>


## Observaciones encontradas en el Dashboard:

* Por cada 100 accidentes de tránsito 2 terminan en lesiones graves y 1 en muerte. Esto implica que la conversión de incidente grave a fatal es muy alta comparada en accidentes industriales; por ejemplo la teoría de la causalidad de Bird donde describe que 1 de cada 10 incidentes graves se convierten en fatal.


* Mueren más Hombres que Mujeres en accidentes de tránsito a nivel general, pero esto se debe también a que hay más hombres conductores que mujeres, en este informe no se respalda directamente esta afirmación pero infiere al observar la segunda conclusión o revisando la fuente externa de la UNDAV.


* Mueren más mujeres en transporte público que hombres (se transportan más mujeres en dicho transporte).


* Técnicamente muere 1 peatón mujer por cada peatón hombre. Pero mueren más mujeres adulta mayor, esto teniendo en cuenta también que hay más hombres adulto mayor que conducen.


* De las víctimas mortales, las que se transportan en moto representan ampliamente la mayoría de los casos (más del 40%).


* La conversión de incidentes leves a graves o muerte es más alta en las motos, pero es significativa en peatones, que desplazan a los autos al ser más probable que un accidente que involucra peatones termine en una lesión grave o muerte para el mismo.


* La principal víctima mortal de las motos son el peatón y de los autos son las motos, los autos representan el mayor número de casos como presunto acusado.


* Las comunas con más víctimas mortales son la 1, 4 y 9. Se puede inferir que la comuna 1 incide en las comunas aledañas al estar en este lugar el Puerto de la Ciudad Autónoma de Buenos Aires, donde la actividad portuaria y logística asociada influye en la circulación de tránsito de vehículos. las comunas 4 y 9 a parte de tener vías que conectan a la comuna 1, también lo hacen para salir de CABA hacia Avellaneda y Lanús (Zonas Industriales). Esto quiere decir que los incidentes fatales suceden camino al trabajo.


* En la hora de la mañana (4 a 9 a.m.) hay más víctimas mortales en las comunas 1,4 y 8 (saliendo al sur de CABA), lo mismo en el horario de 4 a 6 p.m.

* Aparentemente las víctimas fatales disminuyen desde el año 2016 hasta el año 2021 con un leve crecimiento en el año 2021. Pero aunque es cierto que disminuye, en el 2020 el acontecimiento global de la pandemia del Covid-19 alteró la tendencia real.


* Se aprecia estacionalidad en los meses de Agosto y en el rango de Enero a Diciembre; asociados a las vacaciones de Invierno y verano respectivamente.


* Se presentan más accidentes mortales los fines de semana en las horas de la mañana y se presentan entre semana los incidentes mortales en la tarde al finalizar la jornada laboral, en la mañana después de las 7:00 am (cuando las personas se dirigen a sus obligaciones) y después del medio día al rededor de las 2:00 p.m. cuando las personas regresan del almuerzo, algunos terminan sus jornadas (laborales o colegios). Esto se sustenta también de que los jóvenes mueren con mayor frecuencia en accidentes del medio día.


* En los eventos diarios, las lesiones leves se presentaron en un promedio de 24 víctimas día, con valores atípicos de más de 60 víctimas. En las lesiones graves el promedio diario es 1 víctima al día aproximadamente, con valores atípicos de más de 5 víctimas. Para el caso de los accidentes mortales, se presenta 1 cada 4 días aproximadamente, el máximo de víctimas en un día es 3.


* De acuerdo con el KPI 1. "Disminución de la Tasa de Homicidios por Siniestro Vial 10% cada semestre" (THSV), se deduce que se aparentemente se está cumpliendo con la reducción del 10% a nivel global y en el último semestre del año 2021; pero esto es debido a que en el 2020 el indicador fue afectado por las restricciones en pandemia (Covid 19).


* En el caso del KPI 2. "Disminución del número de muertes en un 7% cada año" el impacto de la pandemia al parecer tuvo un impacto negativo, dado que en el 2020 presentó un incremento en el número de víctimas. Esto puede ser a la reducción de vehículos en las calles que permitió un tránsito a mayor velocidad (se debe revisar que se haya permitido mayor circulación de motos).


* El KPI 3. "Disminución del número de muertes de peatones con respecto del año anterior en 10%" permite observar que esto no se ha logrado a nivel globa ni tampoco en el último año de análisis (2021). La tendencia indica que esto puede mejorar.

## Conclusiones y Recomendaciones:

* **Contextualización de los Hechos**: Este informe tuvo a disposición datos que dan respuesta a la clasificación de los incidentes, la ubicación y el momento; pero queda abierto a varias suposiciones por carecer del registro detallado que permita contextualizar los hechos; tales como el clima, si la víctima llevaba cinturón de seguridad, si el conductor de moto llevaba casco, si sobrepasaba los límites de velocidad, etc. Sin embargo, este estudio servirá para orientar los próximos análisis que permitan recolectar dichos datos en la población, lugar  y tiempos más relevantes.


* **Plan de acción Motos (Hombre)**: Se debe generar un plan específico para la disminución de accidentes para motos, ya que estos representan más del 40% de los hechos fatales. Podría ser especialmente conductores hombres, ya que en este tipo de víctima se aprecia una menor accidentalidad de las mujeres, más allá de saber que el 30% de las personas que conducen moto son mujeres.


* **Más Uso del transporte público**: Incentivar el uso de transporte público y disminuir el tráfico. (basado en que este medio de transporte es menos accidentado).


* **Colaboración con el sector productivo**: Incentivar a las empresas e instituciones el trabajo o estudio virtual disminuyendo la necesidad del desplazamiento. Lo anterior, porque se deduce de los datos que los hechos ocurren en la mañana cuando las personas se dirigen a sus que haceres diarios, al medio día cuando terminan algunos turnos o salen las personas a almorzar y en la tarde en el horario de regreso a sus hogares. Por ejemplo, los jóvenes mueren con mayor frecuencia en accidentes viales alrededor del medio día.


* **Plan Retorno (vacaciones)**: Realizar "plan retorno" en las temporadas de vacaciones, para disminuir el flujo vehicular y realizar acompañamiento a la entrada y salida de CABA.


* **Ingresos y salidas del sur de CABA**: Se deben tomar medidas en las horas de la mañana (4 a 9 a.m.) y en la tarde (4 a 6 p.m.) en las entrada y salida al sur de CABA dado que en estos horarios se generan más accidentes fatales. Esto es debido que CABA limita con Avellaneda y Lanús donde probablemente los habitantes de CABA van a trabajar en el día y regresan en la tarde y en la noche.


* **Mejorar registros de hechos leves**: Se debe estimar la tasa de conversión de accidentes leves a graves y fatales, mejorar el registro y análisis de estos hechos menores para generar alertas a tiempo de los sectores que deben abordarse antes de que sucedan los accidentes graves y mortales. la inteligencia artificial, jugará un rol especial en el futuro, cuando a través de video pueda clasificar los hechos menores, documentarlos y contarlos para este fin.

___________________________________________________________________________________________________
# Despedida

¡Gracias por su visita a este proyecto!</p>
Espero que haya sido de utilidad y que haya cumplido con sus expectativas.</p>
Cordial Saludo,

Luis David Rojas Díaz</p>
ldavidrd@gmail.com