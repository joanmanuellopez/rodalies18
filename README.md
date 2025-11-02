# Evolución diaria de pasajeros en la red de Rodalies de Barcelona el año 2018

## Contexto del proyecto
Proyecto en lenguaje R, se trata de un análisis exploratorio para estudiar los flujos de viajeros en la red de Rodalies de Barcelona en el año 2018 a partir de los datos abiertos publicados en la web de Renfe. A partir de los resultados obtenidos me surgió la idea de desarrollar un método para detectar las estaciones de la red que presentan tendencias claras de flujos de commuting, tanto residencial como laboral.

### Retos

El mayor reto que plantea este dataset es la falta de granularidad, ya que solo se facilitan las medias anuales de pasajeros por tramos de 30 minutos. Esta limitación en los datos impide analizar con más detalle ciertos aspectos: 

* *Días de la semana*. Diferencias en los flujos entre laborables vs festivos.
* *Meses del año*. Diferencias en los flujos en los meses de verano respecto el resto del año.
* Al ofrecer las entradas y salidas de viajeros por separado, no se permite establecer una matriz origen-destino de manera directa.

### Fuentes de datos
El conjunto de datos utilizado es el **Volumen de Viajeros por Franja Horaria (Barcelona)** disponible en el portal [Renfe Data](https://data.renfe.com/dataset/volumen-de-viajeros-por-franja-horaria-barcelona) con información del año 2018, la más actual de las publicadas (última revisión del portal, septiembre de 2025).

## Conclusiones principales

El análisis llevado a cabo en este proyecto ha permitido conocer:  

* Cuáles son las estaciones con mayor flujo de viajeros (subidos y bajados) en la red de Rodalies. Se observa que básicamente son las ubicadas en la ciudad de Barcelona.
* Cómo es la evolución de los accesos a la red durante la jornada. Se observa el pico de la hora punta de la mañana entre las 7h y las 8h, y el de la tarde entre las 17h y las 19h.
* Algunos ejemplos de estaciones con flujos de commuting residencial o laboral. El hecho de que los datos solo proporcionen las medias anuales, distorsionan las observaciones, que hubieran sido más precisas de haber podido coger tan solo los datos correspondientes a los días laborables.

## Descripción de los ficheros

Se incluye el fichero RMD que se usa para generar el informe en HTML, así como los conjuntos de datos originales en formato CSV publicados en el portal de datos abiertos de renfe operadora.

**rodalies18_pf.Rmd**  
Análisis exploratorio de los datos, en el que se comprueba la distribución de viajeros subidos y bajados en la red, así como cuáles son las estaciones con mayor flujo de viajeros (subidos y bajados). A continuación se explora la evolución horaria del número de pasajeros que acceden a la red en el conjunto global de las estaciones, estableciéndose las horas punta de la mañana y de la tarde. Finalmente, a partir de la obtención de las horas punta, se propone un método para la detección de flujos típicos de commuting laboral o residencial en las estaciones de la red.
