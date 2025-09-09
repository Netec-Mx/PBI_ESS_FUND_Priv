# Práctica 3. Elaborar el reporte y subir datos 

## Planteamiento del ejercicio
En este último ejercicio, elaborarás un reporte de ventas y lo subirás al servicio de Power BI. Este laboratorio retoma el conjunto de datos empleados en los laboratorios previos, pero utiliza un archivo de Power BI distinto, esto debido a las limitantes de tiempo, por lo que algunos pasos y transformaciones se han realizado al archivo que se ha manejado para dejarlo en un estado final desde donde retomarás el desarrollo de este laboratorio usando el Archivo `Laboratorio final`. Con el fin de facilitar algunas instrucciones dentro del laboratorio, se usará la sintaxis `Nombre_tabla | Nombre_columna` para definir algunos de los datos a utilizar.

## Objetivo

Crear un informe en Power BI Desktop y subirlo al servicio de Power BI.

## Duración aproximada

Dependiendo la experiencia previa que tenga Power BI, puede que algunas de estas actividades las pueda realizar en mas o menos tiempo, pero el tiempo aproximado para analizar y realizar el laboratorio es de aproximadamente 60 minutos.

## Actividades a realizar

![Actividades a realizar.](./imgs/Diagrama%20Ejercicio%203.png)


# Página Overview

Nos piden elaborar un informe de 3 páginas usando Power BI, primero elaboraremos la página overview cambiando el nombre predeterminado de la página 1 por Overview, el boceto de cómo estarán distribuidos los elementos lo podemos ver en la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-32.png)

Ahora que tienes una idea de la distribución de los elementos, comenzarás a poblar dichos elementos. El primer elemento que trabajarás es el logo de la empresa, el cual está dentro de la carpeta `Documentos` y lo encontrarás como `AdventureWorks Logo`. Inserta esta imagen tomando de referencia la siguiente.

![Borrador de la pagina overview.](./imgs/Lab-33.png)

El siguiente elemento a desarrollar es un segmentador usando los datos `Date` | `Year`, debe tener un estilo de menú desplegable para optimizar el espacio. Ubícalo en el espacio designado. Prueba a seleccionar un año para filtrar la información.

![Borrador de la pagina overview.](./imgs/Lab-34.png)

El siguiente elemento a desarrollar es otro segmentador usando los datos `Region` | `Region`, debe tener un estilo de lista. Ubícalo en el espacio designado.

![Borrador de la pagina overview.](./imgs/Lab-35.png)

Generarás ahora el objeto visual `columnas apiladas y lineas` usando los datos `Date` | `Month`, `Sales` | `Sales` y `Sales` | `Profit margin`. Modifica el aspecto del objeto visual para que muestre información incluso para los meses que no tienen valores. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-36.png)

Generarás ahora el objeto visual `columnas apiladas` usando los datos `Region` | `Group`, `Sales` | `Sales` y `Product` | `Category`. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-37.png)

Generarás ahora el objeto visual `barras apiladas` usando los datos `Product` | `Category`, `Sales` | `Quantity`, modifica el aspecto para permitir las etiquetas de los datos y cambia el color de las barras a un tono parecido a la linea que se muestra en gráfico superior. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-32.png)


# Página Profit

Se pide elaborar una segunda página para el reporte, por lo que debes agregar una nueva página al reporte de Power BI y renombrala como Profit. El boceto de la página será similar a la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-38.png)

Comenzando con la primer visualización, agregarás un segmentador usando los datos `Region` | `Region`. Considera que es posible ver los datos de más de una región al mismo tiempo. Ubícalo en la posición marcada.

![Borrador de la pagina overview.](./imgs/Lab-39.png)

Para la segunda visualización mostraremos una matriz usando los datos `Date` | `Fiscal` en la sección de filas, los siguientes datos irán en la sección de columnas (Todos estos datos son de la tabla Sales): Orders, Sales, Cost, Profit, Profit Margin.

![Borrador de la pagina overview.](./imgs/Lab-38.png)

Nos piden por último agregar a los filtros de Power BI los siguientes criterios aplicándolos a nivel de página.

* Product | Category
* Product | Subcategory
* Product | Product
* Product | Color


# Página My Profit

Nos piden elaborar la última página para el reporte, por lo que debemos agregar una nueva página al reporte de Power BI y renómbrala como My Profit. El boceto de la página será a lo mostrado en la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-310.png)

Agrega un filtro dentro de Power BI a nivel de esta página para filtrar la información con base al criterio `Salesperson (Performance)` | `Salesperson` y selecciona a `Michael Blythe`.

Agrega un segmentador basándonos en los datos `Date` | `Year` ubícalo en la posición designada y prueba a filtrar los valores por un año en particular.

![Borrador de la pagina overview.](./imgs/Lab-311.png)

Añade un objeto visual del tipo `Tarjeta de varias filas` considerando los siguientes valores: `Sales` | `Sales`, `Targets` | `Target`, `Targets` | `Variance`, `Targets` | `Variance Margin`. Cambia el formato de este visual para que el color de fondo sea un tono gris claro y que el tamaño fuente de los valores sea de 28pt. Ubícalo en la posición marcada.

![Borrador de la pagina overview.](./imgs/Lab-312.png)

Agrega un objeto visual del tipo `barras apiladas` usando los datos `Date` | `Month`,
`Sales` | `Sales` y `Targets` | `Target`. Colócalo en la ubicación designada.

![Borrador de la pagina overview.](./imgs/Lab-313.png)

Copia y pega esta última visualización justo al lado de la original, cambiando el tipo de objeto visual a `columnas apiladas` 

![Borrador de la pagina overview.](./imgs/Lab-310.png)

# Modificaciones y publicación

Regresa a la página Overview y cambia el valor del segmentador de los años a otro valor, por ejemplo el año fiscal 2018. Posteriormente cambia a la página My performance, ¿Coinciden los valores?

Regresa a la página Overview y seleccionando el segmentador selecciona la opción de sincronización de segmentadores para sincronizar los datos entre estas dos páginas. Haz algo parecido pero con el otro segmentador para sincronizar los datos para la página Profit.


Abra el navegador dentro de la maquina virtual y vaya a https://app.powerbi.com. Inicie sesión con las credenciales del inquilino de Microsoft 365 proporcionadas para desarrollar el laboratorio.

Dentro de Power Bi desktop en la pestaña Inicio seleccione Publicar y guarde el reporte en `Mi espacio de trabajo`

Abra el navegador Microsoft Edge y vaya a https://app.powerbi.com.

En el servicio Power BI, ingrese a `Mi espacio de trabajo` para verificar que el contenido fue publicado.

Al publicar el informe, el modelo de datos y el informe fueron cargados al servicio de Power BI. Al abrir el informe verás practicamente lo mismo que desarrollaste en Power Bi Desktop, ahora en el servicio de Power BI.
