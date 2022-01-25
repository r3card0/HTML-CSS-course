¿porqué index?
Es la pagina inicial que el servidor busca para abrir una pagina web

1. Empezar con <!DOCTYPE html>

<!DOCTYPE html> Esta linea le dice al servidor que todo lo que contiene es HTML 5. 

2. Crear contenedor principal <html></html>
Llevara todo el contenido de etiquetas

<html lang="es"> atributo lang le dice al navegador que idioma tiene el proyecto y le permite hacer traducciones a herramientas que lo hagan

3. Contenedores dentro de <html></html>
  <head></head>
tabulador, dejar espacios para permitir leer elcdigo. Es una buena practica
head y body son contendores hermanos
En head va contener todo lo importante para el navegador que usa para cargar el proyecto. No es visual para el usuario final. Dependencias, librerias externas , fuentes, css. Aqui se llama.
En el head, como el cuerpo humano, es el cerebro, conexiones 

Etiquetas
meta: le dan info al navegador para que sepa como tratar el proyecto
meta lleva un atributo llamado charset, el cual sirve para utf-8 sirve para que el navegador pueda leer caracteres especiales. Van incluidos los emojis
<meta name="description" content="Es"
Se usa para agregar una breve descripción de la página web y la cual es mostrada en las busquedas de google.
![](images/)

<meta name="robots" content="index,follow"/>
Permite a los robots de los motores de busqueda posicionar a la pagina en busquedasr referentes  las busquedas
. Con esta linea autorizamos a los robots a posicionar la pagina web
<title></title>

<meta name="viewport" content="width=device-width, initial-scale=1.0"/>
es la fabulosa linea que hace que la pagina se vea en la escale de una compu o telefono

<link rel="stylesheet" href="./css/style.css"/> Sirve  refernciar a la hoja de .css, la hoja de estilos.
  <body></body>
  En body contiene todo lo visual para el usarios, textos, fotos, videos 
  Piernas, brazos, dorso

