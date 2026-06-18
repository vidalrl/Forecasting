## Vision general del proyecto
- Se estima el numero de ventas de 20 productos de 8 dias futuros 
- informacion tomada de una cadena de supermercados, especificamente de dos locales

## ¿Que se puede lograr con estos datos?
- reduccion de costes de almacen
- reduccion de costes de capital
- reducir roturas de stock

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
