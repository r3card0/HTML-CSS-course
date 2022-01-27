# CSS

## ¿Qué es CSS?

CSS significa -> Cascading Style Sheet

Aplica estilos en forma de cascada.

Cascading, es el nombre del algoritmo que usa el navegador al momento de implementar los estilos.

Es darle un estilo visual al html

## ¿Como iniciar CSS?

1. Tener creado un directorio del proyecto
2. Crear el archivo index.html
3. Crear directorio CSS
4. Crear archivo style.css
5. En en index.html agregar la línea de código: <link rel="stylesheet" href="./style.css">, en el <head></head> 

```
<link rel="stylesheet" href="./style.css">
```

### ¿Cuál es la sintaxis de CSS?
Un conjunto de reglas CSS consta de un selector y un bloque de declaración. Cada declaración incluye un nombre de propiedad CSS y un valor, separados por dos puntos. Una declaración CSS siempre termina con un punto y coma, y los bloques de declaración están rodeados por llaves.

> Sintaxis: Selector {propiedad: valor}



##  Practicas no recomendadas

Poner estilos en el archivo de html:
1. Usando la etiqueta <style></style>. Hace que tarde mucho en cargar cuando hay muchas líneas de estilos

2. Estilo embebido. Agregar estilos dentro de las etiquetas de html en forma de atributo.

## Práctica Recomendada

### Llamando a las etiquetas
Hay 3 formas de llamar o referenciar etiquetas para agregarles estilos

1. Por el elemento. Por la etiqueta 
2. Por clase.
3. Por ID.

## Pseudo clases y Pseudo elementos

¿qué son?
¿para qué son?
¿como se hacen, identifican, resuelven, etc. . . 

Como ponerle estilos a una etiqueta, sin que cambie las demas etiquetas del mismo tipo de etiqueta

BEM es un estandar para nombrar clases en css: 
[BEM](https://en.bem.info/methodology/faq/#why-bem)


.main-nav {
    margin-top: 10px;
    list-style: none; -> le quita los bullets  a las listas desordenadas
    padding-left: 0px; -> 2mdo cuadro concénctrico: indica el marco izquierdo
}

````
.main-nav {
    margin-top: 10px;
    list-style: none; 
    padding-left: 0px;
}
````


### Pseudo clases

Define el estilo de un estado especial de un elemento
1. .main-nav__item a:hover {
2. .main-nav__item a:active {



### Pseudo elemento

Define el estilo de una parte específica de un elemento
1. .main-nav__item a::after {

## Regla en CSS
![regla](/Doc/images/reglaencss.png "Regla de CSS")


- Selector: indica a CSS que elemento se quiere modificar
- Braket {}. Dentro de los brakets viene la declaración del estilo. 
- La declaración se compone de dos propiedades: el estilo que se va a implementar y el valor que tomará.
- property
- property value. Debe terminar con ";"

## Modelo de caja
![modelo de caja](/Doc/images/modelodecaja.png "Modelo de Caja")

![detalle](/Doc/images/detalle.png "Detalle de la caja")

Selector universal *

```
* {
    box-sizing: border-box;
    padding: 0;
    margin: 0;
}
````
- Sirve para quitar los espacios
- Le quita el scroll de la pantalla, calculando automáticamente el tamaño del elemento con el padding y el border para que la caja tome el tamaño de la pantalla y no genere barras de scroll 😌

Por lo tanto, siempre siempre siempre hay que agregar el selector universal a todas las hojas de stilo, para mantener esta buena práctica.

