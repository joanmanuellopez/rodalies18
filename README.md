# Evolución diaria de pasajeros en la red de Rodalies de Barcelona el año 2018

## Contexto del proyecto
Proyecto en lenguaje R, se trata de un análisis exploratorio para estudiar los flujos de viajeros en la red de Rodalies de Barcelona en el año 2018 a partir de los datos abiertos publicados en la web de Renfe. A partir de los resultados obtenidos me surgió la idea de desarrollar un método para detectar las estaciones de la red que presentan tendencias claras de flujos de commuting, tanto residencial como laboral.

### Retos

El mayor reto que plantea este dataset es la falta de granularidad, ya que solo se facilitan las medias anuales de pasajeros por tramos de 30 minutos. 

* Días de la semana (laborables vs festivos)
* Meses del año (verano vs invierno)
* No se puede estableceer una matriz origen-destino

### Fuentes de datos
El conjunto de datos utilizado es el **Volumen de Viajeros por Franja Horaria (Barcelona)** disponible en el portal [Renfe Data](https://data.renfe.com/dataset/volumen-de-viajeros-por-franja-horaria-barcelona) con información del año 2018, la más actual de las publicadas (última revisión del portal, septiembre de 2025).

## Conclusiones principales

* Estaciones con mayor flujo de viajeros (subidos y bajados).
* Evolución de los accesos a la red durante la jornada.
* Estaciones de commuting.

## Descripción de los ficheros

Se incluye el fichero RMD que se usa para generar el informe en HTML, así como los conjuntos de datos originales en formato CSV publicados en el portal de datos abiertos de renfe operadora.

**file1.Rmd**
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

**data1.csv**
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
