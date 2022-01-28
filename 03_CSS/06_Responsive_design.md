# Responsive Design

Como asegurarse de que los productos cuadren en varios dispositivos.

Como empezar a realizar responsive design?

Saber que son los Media queries y los break points
 - Los break points son las dimensiones en el width de la pantalla en el que se va a generar un cambio. Este cambio reposicionara los elementos en base al dispositivo usado por el usuario.

 - Los media queries son: mobile first / only

 ## Mobil first

 mobile first - se comienza a trabajr desde un dispositivo mobil y despues para una compu o laptop
 only - Solo para dispositivos mobiles

![mobile](/Doc/images/mobile.png)

 se inicia desde las pantallas mas chicas hasta la mas grandes.

 ## Mostly fluid

 ![Mostly fluid](/Doc/images/mostly_fluid.png)

 Para implementar un media query:

 ## Layout Shifter


 ## Column Drop

 ![column drop](/Doc/images/drop-column.png)

### Practicas Recomendadas

* Separar siempre archivos .css por break point: mobile.css / style.css; tablet.css; desktop.css

Beneficios:

Dará velocidad a la carga del proyecto en el navegador

Checar:
[My device](https://www.mydevice.io/)

## Image Responsive

Usar la etiqueta picture
Acomodar primero la de mayor peso, hasta llegar a la imagen por default
La etiqueta img -> renderiza la imagen
width: 100%; -> es el mejor amigo, ya que de adapta al tamaño del padre

¿Cómo puedo saber que se están aplicando mis media queries desde archivos externos?
verificando en Networking delinspector de elementos del navegador

¿Qué significa que un proyecto sea "mobile-first"?
que el diseño está enfcado en dispositivos moviles partiendo de este punto hacia dispositivos con pantallas mas grandes

¿Cuántos breakpoints debería haber en tu proyecto idealmente?
maximo 3

¿Cómo es mejor dividir nuestros media queries?
un archivo con los estyilos generales y otro archivo por cada media query que se requiera

Es la principal característica del patrón Layout Shifter:
Se inicia en un diseño vertical y al crecer la pantall se reposicionan los elementos para dar un layout diferente

¿Dónde se recomienda colocar los media queries en CSS en caso usar un solo archivo?
Al final del archivo despues de todos los estilos


Conclusion, se debe usar la medida rem para facilitar la lectura  a personas con problemas visuales