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


# Fuentes

Es posible añadir nuevas fuentes con la propiedad **@font-face**

# Unidades Relativas

toman su valor con base a otro elemento. 
Se adaptan mejor a diferentes resoluciones  y densidades
de pixeles(mejor opcion cunado el trabajo se verá en la 
mayor parte de dispositivos).
Algunos ejemplos:

- em
- rem: se aconseja utilizarlo junto con el hack 62.5%
- vh
- vw
- porcentajes

**Importante:** Si en el documento, en el estilo css de *html* no se pone fuente, por defecto esta queda de 16px 

# Estandares de Escritura CSS(Usar 1 máximo 2)

## BEM(Block element Modifier): 
* Se crea un bloque(contenedor principal)
* El bloque puede tener multiples elementos
* Cada elemento se identifica con el doble gion bajo
* El elemento puede tener varios estado o acciones(ej: boton hundido, click en un hipervinculo)
* Los estilos de estado , accion(modificador), se denotan con doble guion

```
/*Ejemplos */
.card{}
.card__titulo{}
.card__boton{}
.card__boton--activo{}
```

## Modulos CSS:

```
    .card{}
    .card h2{}
    .card img{}
```

# SMACSS(No muy usado)

Estilos para elementos que comparten propiedades en comun

```
    #header, #article, #footer{
        width: 960px;
        margin: auto;
    }
```



