# Index y su estructura básica

Index, es el archivo principal de un proyecto web y siempre debe llamarse *index.html*

¿porqué index?
*Es la pagina inicial que el servidor busca para abrir un proyecto. index, es la página que el servidor buscará para abrirla.*

Si esta pagian no existe, tendriamos que indicarle.

## Primeras líneas

1. Empezar con !DOCTYPE html

````
<!DOCTYPE html>
````


< !DOCTYPE html > -> Esta linea le dice al servidor que todo lo que contiene es HTML 5. 

2. < html > Crear contenedor principal o contenedor padre *html*. Llevara todo el contenido de etiquetas

````
<html></html>
````


< html lang="es" > El atributo *lang* le dice al navegador que idioma tiene el proyecto y le permite hacer traducciones a herramientas que lo hagan

````
<html lang="es">
</html>
````


3. Crear contenedores dentro de < html >< /html >

* head
* body

````
<!DOCTYPE html>
<html lang="es">
    <head></head>
    <body>
        
    </body>
</html>
````


Dejar un espacio se le llama tabulador. Se hace así para que sea más fácil de leer.

Para el navegador le vale m como se tenga organizado, pero es buena practica, para que los demás programadores entiendan el código.

Apertura y cierre de las etiquetas

Hay etiquetas que se abren y se cierran.

````
<html>

</html>
````


Hay etiquetas que solo se abren y se cierran solas.
````
<!DOCTYPE html>

<meta/>
````


Las etiquetas *head* y *body* son contenedores hermanos.

### Head < head > < /head >

En *head* va contener todo lo importante para el navegador que usa para cargar el proyecto en la forma en que el programador los construyo.

No es visual para el usuario final. Hay dependencias, librerias externas , fuentes, css. Aqui se llama.
Todo lo que está en el *head* no es visible para el usuario. 

En el *head*, como el cuerpo humano, es el cerebro. Aquí están las conexiones.

En el body, está todo lo visual para el usuario como son los textos, fotos, videos , etc. Seria todo lo visible para el usuario como el cuerpo humano son las piernas, brazos, dorso, etc.

## Etiquetas *meta*
* Las etiquetas *meta* le dan info al navegador para que sepa como tratar el proyecto.

### meta charset="UTF-8"
meta lleva un atributo llamado *charset*, el cual sirve para utf-8 sirve para que el navegador pueda leer caracteres especiales. Van incluidos los emojis.

````
<meta charset="utf-8" >
````
````
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
    </head>
    <body>
        
    </body>
</html>
````



### meta name="description"
Se usa para agregar una breve descripción de la páginba web y es mostrada en las búsquedas de google.

````
<meta name="description" content="Esta es una página de gatitos y robots">
````
Ejemplo gráfico:

![meta_name_content](/Doc/images/meta_name_content.png)

La parte sombreada es el texto contenido en el atributo *content*

y el codigo va quedando:

````
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <meta name="description" content="Esta es una página de gatitos y robots">
    </head>
    <body>
        
    </body>
</html>
````

### meta name="robots"

Permite a los robots de los motores de busqueda posicionar a la pagina en busquedasr referentes  las busquedas.

Con esta linea -> *content="index-follow"*, autorizamos a los robots a posicionar la pagina web
. Si no se desea que los robots sigan a la pagina se usa la línea -> *content="index-unfollow"*.

````
<meta name="robots" content="index-follow"/>
````

````
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <meta name="description" content="Esta es una pagina de gatitos y robots">
        <meta name="robots" content="index-follow">
    </head>
    <body>
        
    </body>
</html>
````

### Etiqueta *title* ->  < title > < /title>

````
<title></title>
````
Esta etiqueta, es para ponerle el título que que sea visible en las pestañas.

Por ejemplo, puedo ponerle: *Mi página GUEB*

![gueb](/Doc/images/gueb.png)

````
<title>Mi página GUEB</title>
````
Título de la pestaña

````
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <meta name="description" content="Esta es una pagina de gatitos y robots">
        <meta name="robots" content="index-follow">
        <title>Mi página GUEB</title>
    </head>
    <body>
        
    </body>
</html>
````

### Meta para productos responsive -> meta name="viewport"

````
<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
````
Es la fabulosa línea de código que hace que la página web se vea en la escale de la pantalla de una compu o telefono.

### Etiqueta para referenciar los archivos css

````
<link rel="stylesheet" href="./css/style.css"/>
````
La etiqueta *link*, tiene dos atributos: rel y href

* *rel*: Sirve para indicar que el documento que se va a referenciar es una hoja de estilos 
* *href*: indica la ruta del archivo del .css
Sirve  referenciar la hoja de estilos *.css*

El código:

````
<!DOCTYPE html>
<html lang="es">
    <head>
        <meta charset="UTF-8">
        <meta name="description" content="Esta es una pagina de gatitos y robots">
        <meta name="robots" content="index-follow">
        <title>Mi página GUEB</title>
        <link rel="stylesheet" href="./style.css">
    </head>
    <body>
        
    </body>
</html>
````

### Resumen

1. Primera línea -! < !DOCTYPE html>
2. Contenedor principal -> html < html >< /html>
3. Head. Está dentro de html
4. Metas. Están dentro de *head*; meta charset="UTF-8",  meta name="description", meta name="robots", meta name="viewport"
5. title. titulo de la pestaña -> < title>Mi página GUEB</> 
6. link, referenciar los archivos .css -> link rel="stylesheet" href="./css/style.css"/


[tags](https://allthetags.com/)

[Tiny](https://tinypng.com/)
