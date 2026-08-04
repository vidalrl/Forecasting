## Vision general del proyecto
- Se estima el numero de ventas de 20 productos de 8 dias futuros 
- informacion tomada de una cadena de supermercados, especificamente de dos locales

## ¿Que se puede lograr con estos datos?
- reduccion de costes de almacen
- reduccion de costes de capital
- reducir roturas de stock

## Limpieza de datos
La información venia en tres tablas diferentes, se transforman, se unen y limpian para poder trabajar en ellas

## EDA

Insights
- Estructura jerárquica
- Hay productos nuevos a nivel de tienda
- Aunque no a nivel general, por lo que podríamos pensar que no son realmente productos nuevos si no demanda intermitente
- Hay demanda intermitente
- No sabemos la causa: falta de demanda, retirada del mercado o rotura de stock

Acciones:
- Modelizar a nivel tienda producto
- Crear una variable que capture el efecto de la demanda intermitente
- Utilizar algoritmos basados en árboles y rápidos: XGBoost o lightGBM

![Tendencias de venta por producto](https://github.com/vidalrl/Forecasting/blob/main/images/descargar.png)


## Transformacion de datos

-Se crea la variable demanda intermitente con lag de un dia
no tenemos manera de saber si es 0 ventas o una rotura de stock 
-se crea la variable ventas con lag de 15 dias
-se crea la variable sell_price con lag de 7 dias
-Se aplica la transformacion correspondiente a las variables numericas y categoricas utilizando OHE y target enconding


