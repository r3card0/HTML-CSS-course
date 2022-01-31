# Calendar

¿cómo crear un formulario *form* donde se le de la opción al usuario de elegir su fecha de salida y de vuelta, ya sea que viaje en avión, ado o tren . .. .  ¿maya? 😂

Hay dos formas de crear un formulario tipo calendario, que tenga la hora, el día, la semana y el mes.

Opcion 1

1. Crear contenedor form
2. Crear label
3. Crear input
4. Crear span -> contiene la pregunta

Estructura base:
````
<form action="">
    <label for="">
        <span></span>
        <input type="text">
    </label>
</form>
````
Ejemplo real:
````
    <form>
        <label for="hora">
            <span>Hora</span>
            <input type="time" id="hora" name="hora" />
        </label>
        <label for="día">
            <span>Día</span>
            <input type="date" id="día" name="día" />
        </label>
        <label for="semana">
            <span>Semana</span>
            <input type="week" id="semana" name="semana" />
        </label>
        <label for="mes">
            <span>Mes</span>
            <input type="month" id="mes" name="mes" />
        </label>
        <input type="submit" />
    </form>
````

Como se ve
![calendar1](/Doc/images/calendar1.png)

Cuando se requiera capturar información que venga directamente del input, atributo *name* recopila la información y puede ser enviada a una base de datos. 

Opción 2

Seguir la misma estructura, pero en la etiqueta *input* se usaran atributos para crear al calendario.

````
 <form>
        <label for="calendario">
            <span>Calendario</span>
            <input type="datetime-local" id="calendario" name="calendario" />
        </label>
        <input type="submit"/>
    </form>
````

Con el atributo *type* se usa un valor "datetime-local", el cual le dice a la computadora que despliegue el dia y la hora local del computador. Y el resultado es:

![calendar2](/Doc/images/calendar2.png)

Al igual que el anterior, captura los datos para que con un poro de JavaScript, se pueda enviar a una base de datos.

La captura de la información, se crea con la etiqueta *input*, atributo *type* y valor *submit*:

````
<input type="submit"/>
````



[Tipos de input y sus usos](https://developer.mozilla.org/es/docs/Web/HTML/Element/input)
