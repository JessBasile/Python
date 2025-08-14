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

3.  **Obtención de API_KEY**

Se realiza a través del sitio web: https://www.alphavantage.co/

4. **Se crea una lista de accciones**

Inicialmente el listao se compone por 6 empresas, luego el análisis se enfoque en 3.
  ```
  lista_acciones = ["MELI","TSLA", "AAPL","MSFT","AMZN","GOOGL"]
  # Nombre reales por orden de aparición: MercadoLibre, Tesla, Apple, Microsoft, Amazon y Google
  print("lista de acciones creada con éxito")
  ```
5. **Creación de Dataframe con variable Stock**

Abarca el período de elecciones EEUU 2016. Primero se procede a la iniciación del dataframe vacío como buena práctica, en segundo lugar se definen las fechas que abarcan el período electoral en USA con el traspaso del poder Obama-->Trump.
```
fecha_inicio = "2016-01-01"
fecha_fin = "2017-12-31"
```
Luego se conecta con la key de alpha_vantage y posteriormente se realiza una conversión del indice del dataframe de formato data a datatime, se ordena el índice en orden cronológico, se aplica un filtro por fechas, se concatena los datos en df_stocks y se procede a la visualización de la tabla:

	| date       | open    | high     | low      | close   | volume     | Stock |
|------------|---------|----------|----------|---------|------------|-------|
| 2016-01-04 | 112.36  | 112.840  | 108.145  | 109.95  | 535284.0   | MELI  |
| 2016-01-05 | 110.51  | 112.355  | 108.600  | 109.68  | 432668.0   | MELI  |
| 2016-01-06 | 107.98  | 108.980  | 106.110  | 107.33  | 579179.0   | MELI  |
| 2016-01-07 | 104.97  | 106.200  | 101.630  | 102.93  | 475036.0   | MELI  |
| 2016-01-08 | 104.39  | 104.880  | 100.860  | 101.09  | 443968.0   | MELI  |
| ...        | ...     | ...      | ...      | ...     | ...        | ...   |
| 2017-12-22 | 1070.00 | 1071.720 | 1067.640 | 1068.86 | 860800.0   | GOOGL |
| 2017-12-26 | 1068.64 | 1068.860 | 1058.640 | 1065.85 | 914574.0   | GOOGL |
| 2017-12-27 | 1066.60 | 1068.270 | 1058.380 | 1060.20 | 1027634.0  | GOOGL |
| 2017-12-28 | 1062.25 | 1064.840 | 1053.380 | 1055.95 | 982285.0   | GOOGL |
| 2017-12-29 | 1055.49 | 1058.050 | 1052.700 | 1053.40 | 1156357.0  | GOOGL |

3018 rows × 6 columns

6. **

## Gif explicativo

<p align="center">
  <img src="https://github.com/JessBasile/Python/blob/main/Imagenes/Python_github.gif?raw=true" width="700">
</p>

