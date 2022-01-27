# Variables

Custom properties = variables

elemento para crear variables :root

````
:root {
    --primary-color: #003473;
    --secondary-color: #b4d2f7;
    --header-size: 4rem;
    --font:1.8rem;
}
````
para llamar a la variable, usar var( )

````
header {
    width: 100vw;
    height: 15vh;
    background-color: var(--primary-color);
}
````

son utilis de usar en proyectos grandes donde se tiene mucho código.

# Web fonts

### ¿Qué tipo de familias hay?

![familias](/Doc/images/familias.png)

La tabla anterior muestra las fuentas más usadas.

## ¿Cómo están seteadas en la compu?

### navegador
1. ir a Settings del navegador
2. Ir a diseño o appearance
3. Ir a fonts o customize fonts
4. Se pueden modificar y cambiar por las opciones listadas
5. 

### ¿Cómo obtener fuentes nuevas?

Se pueden cambiar por otras en [Google Fonts](https://fonts.google.com/)

No es bueno importar las fuentes en el archivo .css porque afecta el desempeño de la página, es mejor desde el archivo html usando la etiqueta *head*

### Prácticas recomendads

* Cargar 1 sola fuente por proyecto
* Importar la fuente usando la etiqueta *head*

