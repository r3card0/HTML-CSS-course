
A que se le agrega estilos, una vez que ya se tiene la etiqueta.

Que son y como se pueden usar

¿Que es una clase y para que se usa?
* En html la clase *class* es un atributo de las etiquetas.
* Que se usa para especificar una clase para un elemento de HTML. Varios elementos de HTML puede compartir la misma clase.
* Un elemento en HTML está definido por una tag de inicio, algun contenido y termina con un tag de fin.

````
<tagname>Content goes here...</tagname>
````
Ejemplos de elementos de HTML:

````
<h1>My First Heading</h1>
<p>My first paragraph.</p>
````
![html-element-anatomy](/Doc/images/html-element-anatomy.png)

### ¡Hey! seguimos con las clases!

* El atributo clase, es usado para hacer referencia a un nombre de clase en un archivo de estilos. (The class attribute is often used to point to a class name in a style sheet.)

Entiendo que una clase es la forma de dar estilos a las tags

Las clases son templates para los objetos.

El nombre del archivo de .css, normalmente se llama main, style o estilos si estas en un proyecto en español. Cuando el proyecto vaya creciendo y haya mas páginas, hay un archivo .css por cada pantalla y se nombra como la pantalla 🤗

Antes de entrar a las Pseudo Clases

Como nombrar clases?

Si se requiere dar clases a todas las etiquetas de ancla < a >, solo creand la clase en la primera etiqueta < a >, las demás toman esa misma clase:

````
<ul class="main-nav"> 
                <li class="main-nav__item"><a href="">Home</a></li>
                <li class="main-nav__item"><a href="">Cursos</a></li>
                <li class="main-nav__item"><a href="">Instructores</a></li>
                <li class="main-nav__item"><a href="">Blog</a></li>
            </ul>

````
Esto puede ayudar en ocasiones, pero en ocasiones puede compllicar las cosas porque cuando la pagina tenga varias secciones y  a cada sección se requiera poner estilos diferentes, donde en la sección 1 se tenga tags < a > y en la sección 2 tambien se tenga tags < a >, al ponerle clases a la primera, las demás las tomarán. 

Para evitar ponerle estilos a una etiqueta y que se cambie los estilos de otra etiqueta que no se requiere hay técnicas de hacer clases.

En el curso el instructor aplicará la metodología BEM y se requiere consultar en el siguiente link:

[BEM](https://en.bem.info/methodology/faq/#why-bem)

Esta metodología ayuda a nombrar a a las clases para que los proyectos puedan escalar sin problemas.

# Pseudo Clases

Una pseudo-clase es usada para definir un *efecto* o estado especial de un elemento.

Por ejemplo, pueder ser usada en:

* Dar estilo a un elemento cuando el cursor este sobre el elemento
* Dar estilo a un enlace diferenciando cuando se ha visitado o cuando no.

Sintaxis:
1. selector
2. :
3. pseudo-clase
4. Abri {
5. propiedad : valor;
6. Cerrar }

````
selector:pseudo-clase {
    propiedad: valor;
}
````
Ejemplo real:

````
.main-nav__item a:hover {
    color: blue ;
}

````
La pseudo-clase *hover*, crea el efecto de sombreado del elemento cuando el cursor esta posicionado sobre él. No ejecuta nada, solo lo sombrea. Es un estado de sombra. *hover*.

![hover](/Doc/images/hover.png)

La pseudo-clase *active* crea el efecto de color rojo cuando el enlace está **activo*, es decir, cuando está siendo presionado desde el mouse, cuando hace click en el enlace por el usuario.

````
.main-nav__item a:active {
    color: red;
}
````
![active](/Doc/images/active.png)










Referencias:

[Pseudo-clases](https://www.w3schools.com/css/css_pseudo_classes.asp)

# Pseudo Elementos

En CSS un pseudo-elemento es usado para estilizar partes específicas de un elemento.

 Por ejemplo puede ser usado para:

* Estilizar la primera letra o línea de un elemento
* Insertar contenido después o antes de un elemento

Sintaxis:
1. Selector
2. ::
3. pseudo-elemento
4. Abrir {
5. propiedad: valor;
6. Cerrar }

````
selector::pseudo-elemento {
    propiedad: valor;
}
`````


El pseudo-elemento ::first-line, es usada para agregar un estilo especial en la primera línea de un texto 

Ejemplo de la clase:

````
.main-nav__item a::after {
    content: " | ";
}
````
El pseudo-elemento  es usado para agregar un elementos al elemento de navegación. En el ejemplo, se agrego el elemento "|" *after*, o después de la etiqueta:

![after](/Doc/images/after.png)

Entonces: La pseudo-clase y el pseudo elemento son:

![pseudos](/Doc/images/pseudos.png)

Link para saber que otras pseudo-clases hay y para que sirven:

[pseudo-clases](https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes)

Link para saber que otros pseudo-elementos hay y para que sirven:

[pseudo-elementos](https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-elements)


