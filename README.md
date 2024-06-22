# Modelo de Caja & Display

- todos los elementos en un HTML ya tienen un tipo de display por default.
- Algunos elementos comparten un display, mientras que otros tienen uno diferente.

# Tipos de display

### Block

un elemento se pondrá por debajo de otro sin importar su tamaño o que tanto contenido tiene.

**por default aplica a:** div, p,  títulos(h) , ul, ol, li, table, form

### Inline

el elemento se posicionará a la derecha una vez que haya tomado el espacio que requiere.
**por default aplica a:** span, a

### Inline-block

permite darle:

* width
* height
* margin

a un elemento inline, lo cual no es posible para los elementos inline.

# FlexBox

## Concepto

Alinea en una sola dimension y direccion. **DEBE APLICARSE SOBRE EL ANCESTRO INMEDIATO
QUE CONTENGA LOS ELEMENTOS A ALINEAR**, porque aplica solo al primer nivel de hijos.

## Propiedades:

* display: **flex** (habilita el contenedor para flex)
* flex-direction: **row**(izquierda a derecha), **row-reverse**(derecha a izquierda), **column**(arriba a abajo), **column-reverse** (abajo hacia arriba)
* justify-content: si flex-direction es *row*, alinea contenido al centro, izquierda, derecha. Si flex-direction es *column*, alinea al inicio, centro, final

## Relacion justify-content y align-content

| flex-direction |          justify-content          |                     align-content |
|:---------------|:---------------------------------:|----------------------------------:|
| row            | alinear contenido horizontalmente |   alinear contenido verticalmente |
| column         |  alinear contenido verticalmente  | alinear contenido horizontalmente |

# Grid

## Concepto:

A diferencia de Flex, Grid permite trabajar en dos direcciones, creando filas o columnas.

## Propiedades:

* display: **grid**(habilita contenedor para grid);
* grid-template-columns: para agregar columnas
* grid-template-rows: para agregar filas

## Particularidades:

* medidas recomendadas: **fr(fraccion)**, que distribuye uniformemente las columns o rows
* 





