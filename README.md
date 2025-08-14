## Phyton para finanzas

<img align="right" alt="Python" width="250" src="https://github.com/JessBasile/TuPrimeraPagina-Basile/raw/main/imagenes/python.gif">

El presente proyecto se basa en la creación de una notebook en Google Colab, con un análisis de datos relacionados a las acciones de diferentes compañias con gráficos históricos sobre las cotizaciones en la bolsa de valores durante el período 2016-2017. Se elegió ese período dado fué una etapa electoral en EEUU, un momento clave para la economí y los mercados financieros. 

Se icieron verificación de `splits` en los momentos de caídas abruptas para descartar una división de las acciones existentes, en varias nuevas para bajar el precio unitario sin cambiar el valor total que posee cada accionista. La consulta fué hecha en el sitio web `finance.yahoo`. Afortunadamnte, las empresas analizadas no tuvieron slipts dentro del lapso sometido análisis.

Se deja a disposición video explicativo ([Link AQUÍ](https://view.genially.com/67ca73e4481e4913c9a91756)).

1. **Instalación de Librería**
`alpha_vantage` = para acceder a datos financieros y económicos en tiempo real o históricos a través de la API de Alpha Vantage
   ```
   !pip install alpha_vantage
   print("importación exitosa")
   ```
Luego de cada instalación o importación se coloca un print para confirmar que corre exitosamente.
   
2.  **Instalación de Métodos**
Se procede a importar los métodos necesarios
   ```
  from alpha_vantage.timeseries import TimeSeries # Importación del método TimeSeries a través de la API alpha_vantage
  print("importación del método TimeSeries exitoso")
  import matplotlib.pyplot as plt # Importación libreria para visualización de datos en gráficos
  print("importación de matplotlib exitosa")
  import pandas as pd # Importación libreria para manipulación de dataframe
  print("importación de pandas exitosa")
  ```

4.  **Obtención de API_KEY**

Se realiza a través del sitio web: https://www.alphavantage.co/

6. **Se crea una lista de accciones**
  ```
  lista_acciones = ["MELI","TSLA", "AAPL","MSFT","AMZN","GOOGL"]
  # Nombre reales por orden de aparición: MercadoLibre, Tesla, Apple, Microsoft, Amazon y Google
  print("lista de acciones creada con éxito")
  ```


***Gif explicativo***

<p align="center">
  <img src="https://github.com/JessBasile/Python/blob/main/Imagenes/Python_github.gif?raw=true" width="700">
</p>

