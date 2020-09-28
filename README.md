# notes-flexbox

## Intro a Flexbox

Es un módulo de CSS que nos permite, de forma más eficiente, armar diferentes layouts, alinear y distribuir el espacio entre los items de un container.

Hay un _cambio de perspectiva_ respecto de cómo manejamos el layout en comparación a usar Floats: pensamos en cómo se comportan los elementos dentro de un container en lugar de cómo lo hace c/u en particular. Además, tenemos mayor control sobre la alineación, dirección, orden y tamaño de los elementos, mientras que con Floats sólo podemos controlar cómo se comportan cada elemento en el eje horizontal.

- **axis**
  - main (default ➡️)
  - cross (default ⬇️)

- **container props**
  - `direction`: setear la dirección del eje principal (main axis)
    - `row`, `column`, `row-reverse`, `column-reverse`
  - `flex-wrap`: podemos forzar que los elementos ocupen 1 sola línea
    - `wrap-reverse`: cambia la dirección del _cross axis_
  - `justify-content`: define cómo se distribuye el espacio entre items a lo largo del _main axis_
  - `align-items`: define cómo se distribuye el espacio entre items a lo largo del _cross axis_


- **flex-items props**
  - `align-self`
  - `flex`
    - `flex-grow`
    - `flex-shrink`
    - `flex-basis`

## Flexbox Tips

- tener en cuenta que `justify-content` y `align-items` **siempre son relativas a la dirección de los ejes!** (ej: `flex-direction: row-reverse` & `justify-content: flex-end`)
- para centrar cosas (aplica para CSS en general), necesitamos definir _al menos_ **height** del contenedor de forma explícita. En el caso del ancho, por default va a tomar el ancho del contenedor.
