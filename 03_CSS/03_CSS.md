#
## Medidas en CSS

### Medidas Relativas

- Porcentajes % y se refieren al porcentaje con respecto a la pantalla del dispositivo

### Medidas Absolutas

- Se usan los pixeles. Medida que no cambia sin importar el tamaño de la pantalla


![medidas](/Doc/images/medidas.png)

## Medidas EM

EM es una acrónico de "element".
- Lo que hace es toma el tamañó de fuente que tenga el papa directo.

En el ejemplo, la etiqueta main, está tomando como base el tamaño de la etiqueta html

1.5 em, se mutiplica por los 16 px

16 * 1.5 = 24px. Esa es la propocion 

No es muy recomdable usarlo.

## Medidas REM

El valor inicial de REM siempre será 16px

Este codigo siempre debe venir en cualquier archivo CSS:

`````
* {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
}

html {
    font-size: 62.5%;
}
`````
## Medidas Min-Max

## Posicionamiento de Elementos

![Posicion](/Doc/images/posicion.png)

## Display

### Display block
¿Qué es un elemento block?
Va a utilizar el 100% del espacio que tiene disponible adelante (width) sin importar si el contenido tiene o no espacio.

- Se le puede agregar margin y el padding en las 4 posiciones.
- Como ocupa todo el espacio, cuando venga otra etiqueta, la colocara en el siguiente renglon.



### Display Inline

Etiqueta <span>: es una etiqueta como el div, pero para texto. 😫

- No tiene caja, solo contenido

- El display inline solo ocupa el espacio que ocupa el texto. Model box -> solo tiene contenido. Esto permite que si viene otra etiqueta span, la pondra en el mismo renglon de la anterior, si hay espacio.
- No se puede usar width y hieght
- Solo se puede usar el margin en las posiciones de arriba y abajo. En las posiciones derecha e izquierda no.

### Display Inline block

Permite usar funciones de inline y block.
- Inline: tomara espacio de su contenido
- Block: se podra usar padding arriba y abajo y se puede usar el widht y el height
Etiqueta <ul>
