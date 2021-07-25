# GRID CSS

Es un sistema de maquetación __bidemensional__ de filas y columnas en CSS.

Esta pensado para planificar las estructuras y secciones que definen las __Interfaces Principales__ de los sitios y las aplicaciones web, es decir, lo que normalmente se hace en un boceto de una propuesta visual como wireframes o zonas de contenido, esas estructuras se pueden definir con Grid CSS.

# ¿Grid remplaza a  Flexbox?

No es un remplazo de flexbox, por el contrario, es un complemento de este.

Mientras que flexbox es un sistema unidimencional, es decir, tiene filas y columnas pero no al mismo tiempo, es ideal para acomodar elementos en linea, Grid CSS permite trabajar al mismo tiempo con ambos elelmentos (filas y columnas), por lo que crear reticulas de maquetación es extremadamente sencillo y rapido.

Por eso __Flexbox__ es excelente para el acomodo interno de los elementos de un componente de interfaz como por ejemplo Cards, Modals, Buttons, Forms, Menus, etc. Mientras que __Grid CSS__ es excelente para maquetar las secciones de contenido donde van los componentes por ejemplo Headers, Footers, SideBars, Gallerias, etc.

Asi que __Grid CSS__ no remplaza a __Flexbox__, lo complementa y ambas herramientas nos convierten en una filosofia de navaja suiza a la hora de maquetar interfaces de sitios y aplicaciones web.

## CONCEPTOS BASICOS

-  Contenedor Padre (Grid Container)
-  Elementos Hijos (Grid Items)
-  Lineas de Cuadricula (Grid Lines)
-  Pista de Cuadricula (Grid Track)
-  Celda de Cuadricula (Grid Cell)
-  Área de Cuadricula (Grid Area)

### GRID EXPLICITA

Hay varias maneras de definir una grid y una de ellas es la grid explicita, donde definimos __explicitamente__ el numero filas y el numero de columnas que nuestra grid va a tener.

### NOMBRES DE LINEAS

Podemos darle nombre (Personalizar el nombre de las lineas) a cada una de las lineas que trae por defecto las lineas de marcado de la grid que hemos definido.

### GRID AREAS

Podemos asignar nombres a las areas y realizar regiones con areas.

### Grid IMPLICITAS

El navegador definira la grid si se desborda los elementos que no defino en mi grid explicira.