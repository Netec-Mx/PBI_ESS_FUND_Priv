# Práctica 1. Importar el archivo de AdventureWorks Sales 

## Planteamiento del ejercicio

En este primer ejercicio se le presenta el conjunto de datos que será utilizado a lo largo del curso, con base en estos datos se planea elaborar un reporte que represente el estatus de las ventas dentro de la empresa ficticia *AdvertureWorks*.

## Objetivo
Al finalizar la práctica, serás capaz de:
- Importar el archivo y hacer un análisis preliminar de cómo se conforman los datos y la calidad de los mismos.

## Tiempo estimado

Dependiendo la experiencia previa que tenga Power BI, puede que algunas de estas actividades las pueda realizar en más o menos tiempo, pero el tiempo aproximado para analizar y realizar el laboratorio es de 20 minutos.

## Objetivo visual

![Actividades a realizar.](./imgs/Diagrama%20Ejercicio%201.png)

## Obtener los datos

Antes de crear el reporte, es necesario tener acceso a los datos y, por lo tanto, poder manipularlos para crear nuestro reporte.

Para ello, recordemos que la información puede venir de distintos lugares: archivos locales, archivos remotos (en ubicaciones de la empresa o bien en internet), servicios especializados (Servicios de Microsoft, AWS, Google, entre un largo etcétera).

En ese sentido para este primer laboratorio, usaremos un archivo de Excel para obtener la información, el archivo se encuentra en la carpeta documentos de la maquina virtual. Lo identificaras como _**AdventureWorks Sales.xlsx**_.

Una vez corroborada la presencia del archivo que trabajaremos, es momento de abrir la aplicación de Power BI Desktop.

Una vez dentro de Power BI comenzaremos con una serie de tareas para poder obtener y analizar la información. 

Por lo que tendremos que hacer las siguientes tareas:

1. Obtener la información.

> Recuerda como obtener la información dentro de Power BI y cual es tipo de dato que estamos usando en este ejemplo.

![Referencia del menu de inicio.](./imgs/Lab-11.png)

>Al momento de obtener la información ¿Que notas de raro con el conjunto de datos?  
Power BI analiza la información e identifica el contenido que podría ser necesario exportar, en este caso por ejemplo hojas de calculo, tablas, etcetera.

![Referencia del menu para insertar los datos.](./imgs/Lab-12.png)


> Si bien tanto las tablas y las hojas tendrán básicamente el mismo contenido, existirán diferencias entre una opción y otra, inspecciona las diferencias entre una y otra. En este ejercicio solamente seleccionaremos las hojas de calculo pues serán usados mas adelante para modificar la información, en ese sentido agrega las siguientes tablas:

- ColorFormats
- DimEmployee
- DimEmployeeSalesTerritory
- DimProduct
- DimReseller
- DimSalesTerritory
- FactResellerSales
- ResellerSalesTargets

# Examinar los datos

2. Examinar los datos de cada consulta usando Power Query Editor.

> Al obtener este conjunto de datos es necesario determinar la calidad de los mismos, poder determinar que elementos faltan, cuales sobran, o aquellos que necesitan ser modificados. Toma en consideración que estas actividades se harán en el siguiente laboratorio.

> Dando una pequeña explicación de que hace cada tabla y su contenido podemos resumir lo siguiente:  
La consulta **ColorFormats** tiene información que se utilizará para aplicar formato condicional.  
La tabla **DimEmployee** contiene los datos de todos los empleados de AdventureWorks, para nuestro análisis no necesitamos la información de personas ajenas al proceso de ventas.  
El conjunto **DimEmployeeSalesTerritory** es el puente que permite correlacionar los datos del vendedor y de los territorios.  
El contenido de la tabla **DimProduct** como su nombre indica, describe las características del producto en distintos idiomas.  
La consulta  **DimReseller** contiene la información de los distintos negocios que revenden nuestros productos.  
La tabla **DimSalesTerritory** define en que territorios tiene presencia nuestro negocio.  
El conjunto **FactResellerSales** contiene la información de la ventas que deseamos analizar.  
El catalogo **ResellerSalesTargets** define los objetivos que cada vendedor debe lograr por mes.    


3. Examina los datos mediante las opciones de vista de Power Query para ver los datos estadísticos.

![Referencia del menu vista.](./imgs/Lab-13.png)

> Si bien esto lo cubriremos mas adelante, puedes usar las opciones de la pestaña **Vista**, en la sección **Vista previa de datos** puedes usar por ejemplo las opciones; _Distribución de columnas_, _Perfil de columna_, _Calidad de columnas_. ¿Que notas de los valores?, ¿Que valores notas atípicos?, ¿Que modificaciones harías?, ¿Las columnas tienen el tipo de dato correcto?

De estas observaciones que has detectado, en el siguiente ejercicio haremos algunas transformaciones en el conjunto de datos para dejar la información lista para ser utilizada.

# Resultados

Hasta este punto deberás contar con 8 consultas cargadas en Power Query dichas consultas y contenido que deben contener lo puedes corroborar con las siguientes imágenes de referencia.

### Resultado ColorFormats
![Resultado ColorFormats.](./imgs/Lab-14.png)
### Resultado DimEmployee
![Resultado DimEmployee.](./imgs/Lab-15.png)
### Resultado DimEmployeeSalesTerritory
![Resultado DimEmployeeSalesTerritory.](./imgs/Lab-16.png)
### Resultado DimProduct
![Resultado DimProduct.](./imgs/Lab-17.png)
### Resultado DimReseller
![Resultado DimReseller.](./imgs/Lab-18.png)
### Resultado DimSalesTerritory
![Resultado DimSalesTerritory.](./imgs/Lab-19.png)
### Resultado FactResellerTargets
![Resultado FactResellerTargets.](./imgs/Lab-110.png)
### Resultado ResellerSalesTargets
![Resultado ResellerSalesTargets.](./imgs/Lab-111.png)
