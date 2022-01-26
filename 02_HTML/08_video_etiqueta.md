Etiqueta de video para llamar videos localizados en directorios del servidor

<video src="./videos/merge-conflicto.mov" controls preload="auto"> </video>

preload, ayuda a que el video se empieza a renderizar cuando la pagina se empieza a cargar en el navegador. Esto es para que no exista mucho tiempo de espera

ojo: no se empieza a reproducir solo el video, solo se carga. Poner play es decision del usuario.

herramienta para indicar al video que se empiece a reproducir en un minuto específico: #t=60,80
<video src="./videos/merge-conflicto.mov#t=60,80" controls preload="auto"> </video>

Para el navegador pueda elegir el formato de un video, en caso de que no pueda leer todos los formatos de videos y solo uno o el más comun, se usa lo siguiente:

<video controls preload="auto">
    <source src="./videos/merge-conflicto.mov#t=60,80"/>    
</video>

En caso de que el navegador lea todos los formatos, usará el primero de la lista.