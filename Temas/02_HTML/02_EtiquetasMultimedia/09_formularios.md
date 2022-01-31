El mejor formulario es cuando no lo hay 😛

etiqueta <form></form> para comenzar un formulario

<body>
    <form>
        <label for="nombre">
            <span>¿Cuál es tu nombre?</span>
            <input type="text" id="nombre" />
        </label>
    </form>
</body>

label

span

input

<body>
    <form>
        <label for="nombre">
            <span>¿Cuál es tu nombre?</span>
            <input type="text" id="nombre" placeholder="Tu nombre"/>
        </label>        
        <label for="inicio-platzi">
            <span>¿Qué día comenzaste en Platzi?</span>
            <input type="date" id="inicio-platzi" />
        </label>
        <label for="horaio">
            <span>¿En qué horario estudias?</span>
            <input type="time" id="horaio" />
        </label>
          
    </form>
</body>