# Examen3IoT
Juan Felipe Ramírez Castañeda (000166472)

La opción elejida en el examen fue la del SIATA, mas especificamente de la medición de la contaminación PM2.5 del SIATA.

El dataset que se utilizo fue el siguiente: (https://siata.gov.co/EntregaData1/Datos_SIATA_Aire_AQ_pm25_Last.json)

## **Funcionamiento**
El google colab esta dividio en tres etapas:

1. La limpieza de los datos del SIATA
2. Interpolación de los datos con diferentes algoritmos
3. Creación de la visualización del SIATA

Para el dashboard se utilizaron una serie de imagenes las cuales estan ubicadas en una carpeta llamada **assets** las cuales se subieron en el google colab, las imagenes usadas estan en este repositorio

En la visualización se tiene una medición general acompañada por un mapa de calor interpolado en el que se muestran las distintas mediciones del AQI, en la metrica general se utilizaron solo los valores reales (sin interpolación), ademas se decidio utilizar un umbral de peligro a partir de 80 de AQI (que esta en el rango moderado) pero que sigue siendo lo suficientemente alto para que sea conveniente tomar precauciones

La visualización se accede por un proxy (localtunnel) el cual crea un servidor en internet, se accede desde colab, con la contraseña siendo la propia IP publica de este.

## **Tecnologias utilizadas**

* **Google colab** como plataforma de desarrollo
* **Python** como lenguaje de programación
* **Pandas** como herramienta de manejo de los datos
* **Dash** como visualización
* **Localtunnel** como el entorno de ejecución
