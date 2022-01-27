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
## Flex Box

````
.container {
    border: 0.3rem solid black;
    display: flex;
    align-items: flex-start;
    height: 50vh;
       
}
````
align-items: flex-start;
align-items: flex-end;
align-items: stretch;
align-items: baseline;

Se le puede dar orden a los contenedores, con la propierad: order

````
.box1 {
    background-color: aquamarine;
    order: 1;
}
```

*disclaimer*: Los contenedores que se les easigne un roden con la propiedad order, se ordenaran pegados a la izquierda. Los contenedores que no se les aplique la propiedad order, se pasaran todos a la izquierda.

### flex-grow

permite al contener crecer las posiciones indicadas

````
.box1 {
    background-color: aquamarine;
    flex-grow: 1;    
}
````
flex-grow: 1; 

