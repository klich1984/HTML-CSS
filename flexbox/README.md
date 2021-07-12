# Aprendidndo FlexBox

Plugin para visual code [CSS Flexbox Cheatsheet](https://marketplace.visualstudio.com/items?itemName=dzhavat.css-flexbox-cheatsheet)

- Uso plugin presionar `f1` y escribir `open CSS flexbox Cheatsheet`

## Que es:

Flexbox CSS es un sistema de maquetación unidimensional (Solo odemos tener filas o columnas no los dos a la vez), pensado principalmente para el acomodo interno de los elementos, componentes y/o widgets de una interfaz de usuario.

Podemos cambiar los ejes x(main axis) y y(cross axis)

# Conceptos Basicos

Todas las cajas por defecto estan con un `display: block`

- Contenedor Padre ( Flex Container ).
- Elementos Hijos ( Flex Items ).
- Eje Principal ( Main Axis )
- Eje Transversal ( Cross Axis ).

![Texto alternativo](/ruta/a/la/imagen.jpg)

# Propiedades CSS

Flexbox tiene 14 propiedades CSS, 8 que aplican al contenedor padre y 6 a los elementos hijos.

El primer valor enlistado en cada propiedad es el que toman por defecto.

## Propiedades del contenedor padre

- __display:__ Definira que una caja sera flexbox de linea o flexbox de linea
  - `display: flex;` -> es una caja flexible que trabaja en bloque
  - `display: inline-flex;` -> Hace que los contenedores que son flexbox se comporten como en linea(solo ocupa el ancho que necesite)

- __flex-direction:__ y __flex-wrap:__ determinan el flujo de la caja, como se van a comportar los elementos hijos y su shorthand(atajo) es __flex-flow__

- __flex-direction:__ Definira el eje principal(main axis) row - X, column - Y

  - `flex-direction: row | row-reverse | column | column-reverse`

![Imagen](/ruta/a/la/imagen.jpg)

- __flex-wrap:__ Define si la caja flexbox envuelve o NO a sus hijos dependiendo de la direccion.

  - nowrap; -> todos sus hijos se afilan en una sola fila, si no caben generan un scroll para poder visualizarlo. Si nuestro hijo tne un alto y ancho
  - warp; Envuelve a los contenedores hijos y considera el tamaño que tenga cada uno de los elementos hijos y si no caben se generan nuevas filas

- __flex-flow:__ flex-direction flex-wrap;

- __justify-content:__ Define la alineación de los hijos en el eje principal (main axis).
  - __Nota:__ esto depende del flex direction (X o Y) y tambien si hay espacios que repartir.

- __align-items:__ Define la alineación de los hijos en el eje transversal (cross axis) dentro de cada línea, funciona por cada linea que tenga el contenedor
  - __strech:__ Se estira en el eje que no es el principal, se estira al tamaño del padre, si no tiene un alto y un ancho definido.
  - __Nota:__  esto depende del flex direction (X o Y)y tambien si hay espacios que repartir.

- __align-content:__ Define la alineación de los hijos en el eje transversal (cross axis), NO funciona cuando los hijos están en UNA sóla línea (es decir cuando `flex-wrap` tiene el valor de `nowrap`, __NO FUNCIONA__).
  - __Nota:__ La propiedad `warp` y `warp-reverse` activan la propiedad `align-content`.

## Propiedades de los elementos hijos

- __flex-grow:__ FACTOR DE CRECIMIENTO Cuando la caja flexbox tenga espacio __sobrante__, es la habilidad o el factor de crecer, valor por defecto es 0, NO se aceptan valores negativos
  - `flex-grow: 0;`

- __flex-shrink:__ FACTOR DE REDUCIMIENTO Cuando la caja flexbox NO tenga espacio sobrante, es la habilidad o el factor de encogerse, valor por defecto es 1, NO se aceptan valores negativos.
  - `flex-shrink: 1;`

- __flex-basis:__ Es el tamaño del elemento hijo dentro de la línea de la caja flexbox, si existe se ignora la propiedad width o height.

  - Si la caja flexbox tiene dirección de fila, flex-basis representa el width.
  - Si la caja flexbox tiene dirección de columna, flex-basis representa el height.
  - Valor por defecto auto.
  - `flex-basis: auto | 100px | 2rem | 50% | etc...;`

- __flex:__ Es un shorthand de las propiedades flex-grow, flex-shrink y flex-basis, en ese orden.
  - `flex: 0 1 auto;`

- __order:__ Representa el orden que tendrán los elementos hijos en la caja flexbox con respecto a como estan en el html (por ejemplo como el posicionamiento con z index).

  - Valor por defecto 0.
  - Se aceptan valores positivos y negativos.
  - Un valor menor siempre irá antes que un valor mayor.
  - `order: 0 | 1 | 2 | -3 | etc...;`

- __align-self:__ Sobreescribe el valor de la propiedad align-items sólo para el elemento hijo especificado.
  - `align-self: stretch | flex-start | flex-end | center | baseline;`

# EJERCICIO PRACTICO

## Maquetación y Responsive Design

Ejemplo de maquetación y responsive design artesanal con Flexbox y con el framework Bootstrap
