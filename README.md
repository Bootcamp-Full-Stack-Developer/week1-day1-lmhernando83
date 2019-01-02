# Revisión de los ejercicios del training

A continuación se hace una lista de observaciones que hacen referencia a errores detectados en los ejercicios del training. Aconsejamos que cada alumno revise su propio trabajo y aporte las correcciones que corresponden.

## HTML: Ejercicio 1

* Es buena practica escribir los tags y sus atributos en minúscula.
* `<title>`: No se admite ningún tag en su interior.
* Rutas: No usar una rutas absolutas para referenciar un recurso externo como una imagen o una hoja de estilo. De usarlas, se hará referencia a la raíz del sitio web y no al propio ordenador.
* No hacer uso del tag `<br>` para generar un margen entre dos elementos. Para efectos visuales aplicamos CSS.
* El tag `<br>` es un tag que no tiene cierre por lo tanto esto es incorrecto: `<br>Texto</br>`.
* No usar tags de presentación por cuestiones meramente estéticas: `<abbr><b>Texto</b></abbr>`. En su lugar usamos CSS de modo que solo escribiremos `<abbr>Texto</abbr>`.
* Existen tags en desuso como es el caso de `<s>` y `<u>`. En el ejercicio eran requeridos los tags `<del>` e `<ins>`.
* Para enfatizar un texto aplicamos el tag `<em>`, mientras que para resaltar su importancia aplicamos el tag `<strong>`. Los tags `<b>` e `<i>` se aplican como último recurso con el fin de resaltar el texto pero que no tiene alguna validez semántica.
* Es gramaticalmente incorrecto anidar una lista \(`<ul>`\) dentro un párrafo \(`<p>`\).
* La palabra DTD \(_Document Type Definition_\) es un acrónimo y por lo tanto ha de ser marcado como tal.
* Una citación ha de ser marcada con su tag correspondiente: `<blockquote>`.
* Es gramaticalmente incorrecto crear una lista \(`<ol>` o `<ul>`\) y a continuación anidar un párrafo \(`<p>`\) sin indicar un elemento `<li>`.

## CSS: Ejercicio 1

* Los acrónimos no tienen un aspecto correcto porque se ha definido un selector erróneo.

---

## HTML: Ejercicio 2

* En ocasiones re repiten errores del ejercicio 1.
* Es posible que algunos haya usado un editor visual?
* Existen atributos en desuso, como el caso de `border="1"`. Se recuerda que todo lo que es presentación ha de ser llevado a CSS.
* En algunas imágenes falta el atributo `alt` , mientras que en otras se ha aplicado un texto alternativo no acorde con la información que transmite la imagen.
* El elemento `<caption>` no se indica en la posición correcta.
* Una tabla está formada por filas \(`<tr>`\) y celdas \(`<th>` o `<td>`\). Cuando creamos una cabecera de tabla o un pie de tabla, hemos de crear al menos una fila.
* No se ha marcado con el tag correcto \(`<code>`\) los fragmentos de código.
* El elemento `<tbody>` es un elemento que ha de tener un cierre: `</tbody>`.
* No se posiciona correctamente el tag `<tfoot>` dentro de la estructura de tabla. Además de: no se ha declarado una fila en su interior, se ha definido una celda de encabezado en lugar de dato, `rowspan=“7”` es incorrecto en cuanto solo hay 4 columnas.

## CSS: Ejercicio 2

* El ejercicio requería utilizar el mismo fichero CSS del ejercicio 1 con el propósito de heredar los estilos anteriores.
* El encabezado no es de color azul, falta la almohadilla \(`#`\).
* Al elemento `<table>` se ha aplicado un `margin` de `32px` en los cuatro lados, sin embargo se requería solo en el lado superior.
* Al elemento `<caption>` se ha aplicado un `margin` de `32px` en los cuatro lados, sin embargo se requería solo en el lado inferior.
* No se ha aplicado el borde a las celdas como requerido. En su lugar se ha aplicado el atributo HTML `border="1"` previamente citado.
* No se ha aplicado un `padding` de `8px` a todas las celdas, sino solo a las celdas de datos \(`<td>`\).
* No se ha aplicado el selector descendente para cambiar el color de fondo a amarillo de la primera columna. En su lugar se ha utilizado un `ID`, desaconsejado por su alta especificidad.
* Las celdas encabezadas por HTML4 y HTML5 no deben estar con fondo rojo.
* Para conseguir un tamaño de fuente 30% más grande era suficiente con aplicar  `font-size: 130%`.
* No todos han hecho uso de los selectores adyacentes.
* Se ha creado una clase que apoya a la clase `.version` en lugar de aplicar el selector correcto.

---

## HTML: Ejercicio 3

### Index.html

* En ocasiones re repiten errores del ejercicio 1.
* El elemento `<b>` dentro un elemento de encabezado \(`<h1> ... <h6>`\) no tiene ningún valor semántico.

### productos.html

* No se ha marcado un encabezado de nivel 2 como tal.
* El elemento `<button>` tiene al menos un atributo obligatorio: `type`, que define el cometido del botón y cuyo valor puede ser `button`, `submit` o `reset`.
* Se ha hecho uso de los nuevos tags de HTML5: bien por la iniciativa pero hay que aplicarlos correctamente.
* Uso incorrecto de los niveles de encabezado: se pasa de `<h2>` a `<h4>`.

### contacto.html

* Es gramaticalmente incorrecto anidar un elemento `<address>` en un `<p>`.
* Un formulario siempre ha de iniciar con su etiqueta `<form>` .
* Los controles de formularios no llevan asociadas una etiqueta \(`<label>`\).
* Atributo `placeholder`: Se utiliza para aportar más información cuando la etiqueta no es lo suficientemente clara.
* En lugar de utilizar `<br>` para crear un salto de línea se aconseja `<p>` o `<div>`.
* No se marca correctamente la dirección con el tag `<address>`.
* Hemos aprendido que los estilos en línea no son un buen método para mantener CSS.
* El elemento `<button>` no tiene el atributo `value` en cuanto es entre el tag de apertura y tag de cierre donde se coloca el rotulo del elemento.

## CSS: Ejercicio 3

* En general, poca iniciativa en el uso de los selectores CSS presentados en el training.
* No es buena práctica el uso de selectores de ID por su alta especificidad.
* Poca coherencia en la estética y en la navegación.
* Se han creado tres ficheros CSS, uno por cada página. De esta manera no aprovechamos la herencia de estilos.
* Es preferible no usar palabras claves para los colores porque son limitadas a 140. En su lugar usamos valores hexadecimales, RGB o HSL.