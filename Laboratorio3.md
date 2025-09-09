# Práctica 3. Elaborar el reporte y subir datos 


En este último ejercicio, elaborarás un reporte de ventas y lo subirás al servicio de Power BI. Esta práctica utiliza el mismo conjunto de datos que los ejercicios anteriores, pero trabaja con un archivo de Power BI diferente. Debido a las limitaciones de tiempo, se han aplicado previamente algunas transformaciones y pasos al archivo que ahora se presenta en su versión final. A partir de este punto, continuarás el desarrollo del laboratorio utilizando el archivo `Laboratorio final`. Con el fin de facilitar algunas instrucciones dentro del laboratorio, se usará la sintaxis `Nombre_tabla | Nombre_columna` para definir algunos de los datos a utilizar.

## Objetivo
Al finalizar la práctica, serás capaz de:
- Crear un informe en Power BI Desktop y subirlo al servicio de Power BI.

## Duración aproximada

- 60 minutos.

## Objetivo visual

![Actividades a realizar.](./imgs/Diagrama%20Ejercicio%203.png)


### Tarea 1. Página Overview

Se requiere elaborar un informe de tres páginas usando Power BI. 

**Paso 1.** Primero, realiza la página `Overview` cambiando el nombre predeterminado de la `Página 1` por `Overview`. El boceto de la distribución de los elementos lo puedes ver en la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-32.png)

**Paso 2.** Ahora que tienes una idea de la distribución de los elementos, comenzarás a poblar dichos elementos. El primer elemento que trabajarás es el logo de la empresa, el cual está dentro de la carpeta `Documentos` y lo encontrarás como `AdventureWorks Logo`. Inserta esta imagen tomando de referencia la siguiente.

![Borrador de la pagina overview.](./imgs/Lab-33.png)

**Paso 3.** El siguiente elemento a desarrollar es un segmentador usando los datos `Date | Year`, debe tener un estilo de menú desplegable para optimizar el espacio. Ubícalo en el espacio designado. Prueba a seleccionar un año para filtrar la información.

![Borrador de la pagina overview.](./imgs/Lab-34.png)

**Paso 4.** El siguiente elemento a desarrollar es otro segmentador usando los datos `Region | Region`, debe tener un estilo de lista. Ubícalo en el espacio designado.

![Borrador de la pagina overview.](./imgs/Lab-35.png)

**Paso 5.** Ahora, genera el objeto visual `Columnas apiladas y líneas` usando los datos `Date | Month`, `Sales | Sales` y `Sales | Profit margin`. Modifica el aspecto del objeto visual para que muestre información incluso para los meses que no tienen valores. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-36.png)

**Paso 6.** Desarrolla el objeto visual `Columnas apiladas` usando los datos `Region | Group`, `Sales | Sales` y `Product | Category`. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-37.png)

**Paso 7.** Elabora el objeto visual `Barras apiladas` usando los datos `Product | Category` y `Sales | Quantity`. Modifica el aspecto para permitir las etiquetas de los datos y cambia el color de las barras a un tono parecido a la línea que se muestra en gráfico superior. Colócalo en la ubicación marcada.

![Borrador de la pagina overview.](./imgs/Lab-32.png)


### Tarea 2. Página Profit

**Paso 1.** Para elaborar la segunda página del reporte, debes agregar una nueva página al reporte de Power BI y renombrarla como `Profit`. El boceto de la página será similar a la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-38.png)

**Paso 2.** Comenzando con la primer visualización, agregarás un segmentador usando los datos `Region | Region`. Considera que es posible ver los datos de más de una región al mismo tiempo. Ubícalo en la posición marcada.

![Borrador de la pagina overview.](./imgs/Lab-39.png)

**Paso 3.** Para la segunda visualización, mostrarás una matriz usando los datos `Date | Fiscal` en la sección de filas, los siguientes datos (provienen de la tabla `Sales`) irán en la sección de columnas: `Orders`, `Sales`, `Cost`, `Profit`, `Profit Margin`.

![Borrador de la pagina overview.](./imgs/Lab-38.png)

**Paso 4.** Se requiere, por último, agregar a los filtros de Power BI los siguientes criterios aplicándolos a nivel de página.

* `Product | Category`
* `Product | Subcategory`
* `Product | Product`
* `Product | Color`


### Tarea 3. Página My Profit

**Paso 1.** Para elaborar la última página del reporte, debes agregar una nueva página al reporte de Power BI y renombrarla como `My Profit`. El boceto de la página será similar a la siguiente imagen.

![Borrador de la pagina overview.](./imgs/Lab-310.png)

**Paso 2.** Agrega un filtro dentro de Power BI a nivel de esta página para filtrar la información con base en el criterio `Salesperson (Performance) | Salesperson` y selecciona a `Michael Blythe`.

Agrega un segmentador basándote en los datos `Date | Year`. Ubícalo en la posición designada y prueba a filtrar los valores por un año en particular.

![Borrador de la pagina overview.](./imgs/Lab-311.png)

**Paso 3.** Añade un objeto visual del tipo `Tarjeta de varias filas` considerando los siguientes valores: `Sales | Sales`, `Targets | Target`, `Targets | Variance`, `Targets | Variance Margin`. Cambia el formato de este visual para que el color de fondo sea un tono gris claro y que el tamaño de la fuente de los valores sea de 28 puntos. Ubícalo en la posición marcada.

![Borrador de la pagina overview.](./imgs/Lab-312.png)

**Paso 4.** Agrega un objeto visual del tipo `Barras apiladas` usando los datos `Date | Month`,
`Sales | Sales` y `Targets | Target`. Colócalo en la ubicación designada.

![Borrador de la pagina overview.](./imgs/Lab-313.png)

**Paso 5.** Copia y pega esta última visualización justo al lado de la original, cambiando el tipo de objeto visual a `Columnas apiladas` 

![Borrador de la pagina overview.](./imgs/Lab-310.png)

## Tarea 4. Modificaciones y publicación

**Paso 1.** Regresa a la página Overview y cambia el valor del segmentador de los años a otro valor, por ejemplo el año fiscal 2018. Posteriormente, cambia a la página `My performance`. ¿Coinciden los valores?

**Paso 2.** Regresa a la página `Overview`, selecciona el segmentador y la opción de sincronización de segmentadores para sincronizar los datos entre estas dos páginas. Haz algo parecido pero con el otro segmentador para sincronizar los datos para la página `Profit`.


**Paso 3.** Abre el navegador dentro de la Máquina virtual y dirígete a https://app.powerbi.com. Inicia sesión con las credenciales del inquilino de Microsoft 365 proporcionadas para desarrollar el laboratorio.

**Paso 4.** Dentro de Power Bi Desktop, en la pestaña `Inicio` selecciona `Publicar` y guarda el reporte en `Mi espacio de trabajo`

**Paso 5.**  Abre el navegador Microsoft Edge y dirígete a https://app.powerbi.com.

**Paso 6.**  En el servicio Power BI, ingresa a `Mi espacio de trabajo` para verificar que el contenido se haya publicado.

## Resultado esperado

Al publicar el informe, el modelo de datos y el informe fueron cargados al servicio de Power BI. Al abrir el informe verás practicamente lo mismo que desarrollaste en Power Bi Desktop, ahora en el servicio de Power BI.
