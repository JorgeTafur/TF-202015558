Autor:

Jorge Arturo Tafur Pastor U202015558

### Introducción

El trabajo final es la continuación del trabajo parcial, consiste en construir nuestro propio “waze”,
es decir un sistema que nos permita encontrar la ruta más corta entre 2 puntos en una ciudad. La
ciudad está representada por un grafo que fue el resultado de su trabajo parcial.
El trabajo parcial consistió en elaborar un grafo para representar una ciudad o una porción o distritos
de una ciudad grande como Lima.


### Definición del mapa

Se escogió el distrito de San Borje en Lima, Perú debido a que es un sector relativamente cuadrado y con el área suficiente para el propósito del proyecto.

Se utilizó una herramienta de google maps para la notación del mapa, donde también especifica las coordenadas que colocaremos para la lista de adyacencia

Link de la herramienta: https://www.google.com/maps/d/u/0/edit?mid=10YmeKCoY1-kNc_U00xwcjFf8B6iAUyvG&ll=-12.09966890248742%2C-77.00309358033083&z=15


### Descripción de las calles

Las calles constan de dos valores, su id en la secuencia de información y su propio nombre, por lo que en ejemplo sería (0, Avenida Canadá) o (2, Avenida Luis Aldana).

### Descripción de las intersecciones

Las intersecciones constan de su identificador, el valor intersección que es la combinación de 2 id de calles, y luego una secuencia de id de calles que sería la unión
de estas intersecciones. Posteriormente se agrega a la información la latitud, longitud, peso y factor de tráfico a las filas de datos.

### Explicación del procedimiento para obtener el grafo

Se lee el archivo de texto donde se encuentra la lista de intersecciones, ésta esta en forma de lista de adyacencia por lo que se puede leer como grafo al procesar 
el algoritmo respectivo.