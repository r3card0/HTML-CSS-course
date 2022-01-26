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
![BEM](https://en.bem.info/methodology/faq/#why-bem)


.main-nav {
    margin-top: 10px;
    list-style: none; -> le quita los bullets  a las listas desordenadas
    padding-left: 0px; -> 2mdo cuadro concénctrico: indica el marco izquierdo
}

### Pseudo clases

Define el estilo de un estado especial de un elemento
1. .main-nav__item a:hover {
2. .main-nav__item a:active {

### Pseudo elemento

Define el estilo de una parte específica de un elemento
1. .main-nav__item a::after {