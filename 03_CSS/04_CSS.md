#

## Display Flex

Es un valor dentro de la propiedad *display*  que permite modificar a los contenedores de forma flexible. *flex*

`````
.container {
    border: 0.3rem solid black;
    display: flex;
}
`````
### flex-wrap: wrap;
Permite que los elementos se bajen a la siguiente linea cuando ya no tengan espacio en la pantalla.

![flex-wrap](/Doc/images/flex-wrap.png)

```
.container {
    border: 0.3rem solid black;
    display: flex;
    flex-wrap: wrap-reverse;
}
````

### wrap-reverse

realiza de forma inversa

### Propiedad: justify-content

Permite centrar los contenedores

````
.container {
    border: 0.3rem solid black;
    display: flex;
    flex-wrap: wrap-reverse;
    justify-content: center;
}
````
o tambien
````
.container {
    border: 0.3rem solid black;
    display: flex;
    flex-wrap: wrap-reverse;
    justify-content: space-around;
    
}
````

![space-around](/Doc/images/space-around.png)

space-evenly: deja los espacios iguales

````
.container {
    border: 0.3rem solid black;
    display: flex;
    flex-wrap: wrap-reverse;
    justify-content: space-evenly;
    
}
````
