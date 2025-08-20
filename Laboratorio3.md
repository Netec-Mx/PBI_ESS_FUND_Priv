# Laboratorio #3: Elaborar el reporte y subir datos 

## Planteamiento del ejercicio.

> En este ultimo ejercicio se espera que se elabore un reporte de ventas y se suba al servicio de Power BI. Este laboratorio retoma el conjunto de datos utilizados en los laboratorios previos, pero utiliza un archivo de Power BI distinto, esto debido a las limitantes de tiempo, por lo que algunos pasos y transformaciones se han realizado al archivo que se ha manejado para dejarlo en un estado final que es desde donde retomaremos el desarrollo de este laboratorio usando el Archivo **Laboratorio final**. Para fines de facilitar algunas instrucciones dentro del laboratorio, se usará la sintaxis **Nombre_tabla** | **Nombre_columna** para definir algunos de los datos a utilizar.

## Objetivo

> Crear nuestro informe en Power BI Desktop y subirlo al servicio de Power BI.

## Tiempo estimado

> Dependiendo la experiencia previa que tenga Power BI, puede que algunas de estas actividades las pueda realizar en mas o menos tiempo, pero el tiempo aproximado para analizar y realizar el laboratorio es de aproximadamente 60 minutos.

## Actividades a realizar

![Actividades a realizar.](./imgs/Diagrama%20Ejercicio%203.png)


# Pagina Overview

Nos piden elaborar un informe de 3 paginas usando Power BI, primero elaboraremos la pagina overview cambiando el nombre predeterminado de la pagina 1 por Overview, el boceto de como estarán distribuidos los elementos lo podemos ver en la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-32.png)

Ahora que tenemos una idea de la distribución de los elementos comenzaremos a ir poblando dichos elementos. Para el primer elemento que debemos trabajar hablamos del logo de la empresa, el logo de esta empresa están dentro de la carpeta documentos y la encontraremos como **AdventureWorks Logo**, inserta esta imagen tomando de referencia la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-33.png)

El siguiente elemento a desarrollar es un segmentador usando los datos **Date** | **Year**, debe tener un estilo de menú desplegable para optimizar el espacio. Ubicalo en el espacio designado. Prueba a seleccionar un año para filtrar la información.

![Borrador de la pagina overview.](./imgs/Lab-34.png)

El siguiente elemento a desarrollar es otro segmentador usando los datos **Region** | **Region**, debe tener un estilo de lista. Ubicalo en el espacio designado.

![Borrador de la pagina overview.](./imgs/Lab-35.png)

Generaremos ahora un objeto visual **columnas apiladas y lineas** usando los datos **Date** | **Month**, **Sales** | **Sales** y **Sales** | **Profit margin**. Modifica el aspecto del objeto visual para que muestre información incluso para los meses que no tienen valores. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-36.png)

Generaremos ahora un objeto visual **columnas apiladas** usando los datos **Region** | **Group**, **Sales** | **Sales** y **Product** | **Category**. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-37.png)

Generaremos ahora un objeto visual **barras apiladas** usando los datos **Product** | **Category**, **Sales** | **Quantity**, modifica el aspecto para permitir las etiquetas de los datos y cambia el color de las barras a un tono parecido a la linea que se muestra en gráfico superior. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-32.png)


# Pagina Profit

Nos piden elaborar una segunda pagina para el reporte, por lo que debemos agregar una nueva pagina al reporte de Power BI y renombrala como Profit. El boceto de la pagina será a lo mostrado en la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-38.png)

Comenzando con la primer visualización agregaremos un segmentador usando los datos **Region** | **Region** considera que es posible querer ver los datos de mas de una región al mismo tiempo. Ubicalo en la posición marcada.

![Borrador de la pagina overview.](./imgs/Lab-39.png)

Para la segunda visualización mostraremos una matriz usando los datos **Date** | **Fiscal** en la sección de filas, los siguientes datos irán en la sección de columnas (Todos estos datos son de la tabla Sales): Orders, Sales, Cost, Profit, Profit Margin.

![Borrador de la pagina overview.](./imgs/Lab-38.png)

Nos piden por ultimo agregar a los filtros de Power BI los siguientes criterios aplicándolos a nivel de pagina.

* Product | Category
* Product | Subcategory
* Product | Product
* Product | Color


# Pagina My Profit

Nos piden elaborar la ultima pagina para el reporte, por lo que debemos agregar una nueva pagina al reporte de Power BI y renombrala como My Profit. El boceto de la pagina será a lo mostrado en la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-310.png)

Agrega un filtro dentro de Power BI a nivel de esta pagina para filtrar la información con base al criterio **Salesperson (Performance)** | **Salesperson** y selecciona a **Michael Blythe**.

Agrega un segmentador basándonos en los datos **Date** | **Year** ubicalo en la posición designada y prueba a filtrar los valores por un año en particular.

![Borrador de la pagina overview.](./imgs/Lab-311.png)

Añade un objeto visual del tipo **Tarjeta de varias filas** considerando los siguientes valores: **Sales** | **Sales**, **Targets** | **Target**, **Targets** | **Variance**, **Targets** | **Variance Margin**. Cambia el formato de este visual para que el color de fondo sea un tono gris claro y que el tamaño fuente de los valores sea de 28pt. Ubicalo en la posición marcada.

![Borrador de la pagina overview.](./imgs/Lab-312.png)

Agrega un objeto visual del tipo **barras apiladas** usando los datos **Date** | **Month**,
**Sales** | **Sales** y **Targets** | **Target**. Colocalo en la ubicación designada.

![Borrador de la pagina overview.](./imgs/Lab-313.png)

Copia y pega esta ultima visualización justamente al lado de la original, cambiando el tipo de objeto visual a **columnas apiladas** 

![Borrador de la pagina overview.](./imgs/Lab-310.png)

# Modificaciones y publicación.

Regresa a la pagina Overview y cambia el valor del segmentador de los años a otro valor, por ejemplo el año fiscal 2018. Posteriormente cambia a la pagina My performance, ¿Coinciden los valores?

Regresa a la pagina Overview y seleccionando el segmentador selecciona la opción de sincronización de segmentadores para sincronizar los datos entre estas dos paginas. Haz algo parecido pero con el otro segmentador para sincronizar los datos para la pagina Profit.


Abra el navegador dentro de la maquina virtual y vaya a https://app.powerbi.com. Inicie sesión con las credenciales del inquilino de Microsoft 365 proporcionadas para desarrollar el laboratorio.

Dentro de Power Bi desktop en la pestaña Inicio seleccione Publicar y guarde el reporte en "Mi espacio de trabajo"

Abra el navegador Microsoft Edge y vaya a https://app.powerbi.com.

En el servicio Power BI, ingrese a "Mi espacio de trabajo" para verificar que el contenido fue publicado.

Al publicar el informe, el modelo de datos y el informe fueron cargados al servicio de Power BI. Al abrir el informe verás practicamente lo mismo que desarrollamos en Power Bi Desktop ahora en el servicio de Power BI.