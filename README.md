# Proyecto de análisis de compras en Estambul

![Shopping Habits in Istanbul](./DATA/Imágenes%20Proyecto/shopping%20habits%20in%20Istanbul.png)

Este proyecto tiene como objetivo analizar las tendencias y patrones de compra en los centros comerciales de Estambul (Turquía).

## Descripción del proyecto
El análisis del presente proyecto busca encontrar patrones que permitan brindar una visión integral de los hábitos de compras en Estambul. 

El dataset contiene información de compras de 10 centros comerciales diferentes entre 2021 y 2023, y con esta información se ha generado un dashboard final a partir de un análisis descriptivo y gráfico que nos permite visualizar métricas clave en las tendencias de consumo.

## Directorio

    -Proyecto_Shopping/
        ├───Data/
            ├───Data Raw/
   	            - Customer_Shopping.xlsx
    	        - customer_shopping_data.csv
            ├───Data Modificaciones/
    	        - Customer_Shopping_cambios.xlsx
    	        - Customer_Shopping_descriptivo.xlsx
            ├───Data Analisis Final/
   	            - Customer_Shopping_dashboard.xlsx
            ├───Imágenes Proyecto/
                - Proyecto Dashboard.png
   	            - shopping habits in Istanbul.png	    
    -README.md

## Estructura de los datos
El dataset original consta de 99.457 filas y 10 columnas, cuya información reflejada es la siguiente:
- **invoice_no** : identificador único de factura.
- **customer_id** : identificador único de cada cliente.
- **gender** : género del cliente.
- **age** : edad del cliente.
- **category** : categoría de los productos comprados.
- **quantity** : cantidades de cada producto por transacción.
- **price** : precio del producto por el total de unidades en liras turcas (TRY).
- **payment_method**: método de pago utilizado en las transacciones.
- **invoice_date** : día en que se generó la transacción.
- **shopping mall** : nombre de los centros comerciales donde se realizó la transacción.

## Desarrollo del proyecto
- Se realiza un primer análisis de los datos para ver como está estructurado
el dataset.
- Empezamos con la transformación de los datos, eliminando duplicados, agregando
nuevas columnas y normalizando los datos.
- La columna "price" está referenciada a la moneda local, la lira turca (TRY).
A efectos prácticos, genero una columna nueva referenciando los precios en moneda EUR.  
El tipo de cambio utilizado (exchange rate TRY/ EUR) es de 0,0273709. 
- Se continúa con la limpieza de datos, generando nuevas columnas que permitan
un mejor análisis posterior de la información.
Para un mejor entendimiento del dataset, cambio el nombre de la columna "price"
a "ingreso total EUR".
- Se realiza el análisis descriptivo de las columnas numéricas.
- Se continúa con el análisis descriptivo de las columnas categóricas y temporales.
- Realizamos gráficos de las columnas relevantes.
- Recopilamos los insights que se han deducido del análisis.
- Finalmente se desarrolla el dashboard.


## Dashboard

![Dashboard](./DATA/Imágenes%20Proyecto/Proyecto%20Dashboard.png)

## Conclusiones
- Según los análisis realizados, se desprende que existe una estabilidad muy marcada en 
los hábitos de consumo.
- Si bien existe un mayor consumo por parte del género femenino (60%), sus patrones
de compra por categoría de producto, rango de edad, centro comercial y método de pago
son prácticamente similares a lo largo del tiempo que el género masculino.
- Tres centros comerciales (Mall of Istanbul, Kanyon y Metrocity) acaparan más
del 55% de las compras.
- Es un mercado en el que el método de pago más habitual es el efectivo (45% de las transacciones),
y no se aprecian cambios significativos ni por género ni por rango de edad.
- Hay que remarcar un dato importante con relación a la categoría, los 3 productos
más vendidos son clothing, cosmetics y food & beverage, sin embargo, solo clothing genera
más del 45% de los ingresos totales.

    Por otro lado, la categoría technology es el producto menos vendido en el período de análisis,
sin embargo, genera el 23% de los ingresos totales.

## Contribuciones
Las contribuciones a este proyecto son bienvenidas. Si tienes alguna sugerencia, mejora o
corrección, no dudes en ponerte en contacto o enviar tus ideas.

Cualquier tipo de contribución, ya sea código, documentación o feedback, será valorada.

¡Gracias por tu ayuda y colaboración!

## Autor
- Johnny [Github Profile](https://github.com/jbdatalytics)





