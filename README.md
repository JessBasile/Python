## Phyton para finanzas

<img align="right" alt="Python" width="250" src="https://github.com/JessBasile/TuPrimeraPagina-Basile/raw/main/imagenes/python.gif">

El presente proyecto se basa en la creación de una notebook en Google Colab, con un análisis de datos relacionados a las acciones de diferentes compañias ([Link AQUÍ](https://view.genially.com/67ca73e4481e4913c9a91756)).

1. **Instalación de Librería**
   ´alpha_vantage´ = para acceder a datos financieros y económicos en tiempo real o históricos a través de la API de Alpha Vantage
   ´´´
   !pip install alpha_vantage
   print("importación exitosa")
   ´´´
   Luego de cada instalación o importación se coloca un print para confirmar que corre exitosamente.
   
2.  **Instalación de Métodos**
   Se procede a importar método TimeSeries a través de la API alpha_vantage
  ´´´
  from alpha_vantage.timeseries import TimeSeries # Importación del método TimeSeries a través de la API alpha_vantage
  print("importación del método TimeSeries exitoso")
  import matplotlib.pyplot as plt # Importación libreria para visualización de datos en gráficos
  print("importación de matplotlib exitosa")
  import pandas as pd # Importación libreria para manipulación de dataframe
  print("importación de pandas exitosa")
  ´´´

3.  **Obtención de API_KEY**
   Se realiza a través de: https://www.alphavantage.co/

4. **Se crea una lista de accciones**
  ´´´
  lista_acciones = ["MELI","TSLA", "AAPL","MSFT","AMZN","GOOGL"]
  # Nombre reales por orden de aparición: MercadoLibre, Tesla, Apple, Microsoft, Amazon y Google
  print("lista de acciones creada con éxito")
  ´´´

5. **
1. **Video explicativo:**

<p align="center">
  <img src="https://github.com/JessBasile/Python/blob/main/Imagenes/Python_github.gif?raw=true" width="700">
</p>

