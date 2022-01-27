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