## Herencia

> La herencia es el código CSS que se va pasar de un padre a un hijo.


## Especificidad 

¿Cómo se controla el orden al declarar CSS?
1. Importancia
2. Epecificidad
3. Orden en las fuentes


En CSS usar las clases y evitar los id.
Para CSS es más importante dos clases que una clase y una etiqueta

### Prácticas no recomendadas
- Usar id para los estilos
- Usar el !important
- Usar los estilos embebidos


## Combinators

![combinators](/Doc/images/combinators.png "Combinators más comunes")

Los combinators ayudan a tener una *especificidad* mas certera. Además de evitar usar id's

```
h2 + p {
    color: red;
}
```
En este ejemplo, indica que se aplique el color rojo a todas las etiquetas *párrafo* (*p*) que estén cerca (por debajo) de una etiqueta *h2*

Esto es muy útil en proyectos donde se tengan grandes cantidades de cajas contenedoras con algunas etiquetas cercanas o hermanas. Ayuda a realizar cambios específicos sin usar tanta clase.

### General Sibling

````
h2 ~p {
    color: red;
}
````

### Hijo y Descendientes

#### Hijo

````
div > p {
    color: purple;
}
`````
todas las etiquetas p que esten directamente dentro de etiquetas div, se les aplica las propiedades y valores indicados.

#### Descendientes

`````
div  p {
    color: purple;
}
`````
Y dice que toas las etiquetas p que estén dentro de de las etiqueta div, se les cambia el color a purple

[Game](https://flukeout.github.io/)