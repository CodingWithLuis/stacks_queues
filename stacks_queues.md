En ciencias de la computación, las estructuras de datos son conceptos fundamentales para organizar y organizar los datos de manera eficiente. Dentro de esas estructuras podemos observar las pilas y colas. A continuación, vamos a describir cada una.

## Pilas

Las pilas son estructuras de datos lineales que siguen el principio **LIFO (Last In, First Out)**, lo que significa que el último elemento agregado a la pila es el primero es ser removido. Para entenderlo de mejor manera podemos visualizarlo como una pila de platos donde el último plato que colocamos en la parte superior es el primer plato en salir (se remueve de la parte superior).

### Operaciones donde hacemos uso de **pilas**

- **push**: Agrega un elemento a la parte superior de la pila
- **pop**: Elimina un elemento de la parte superior de la pila  
- **peek**: Retorna un elemento de la parte superior de la pila sin eliminar dicho elemento

### Ejemplo gráfico

Vamos a empezar con una pila vacía

![Pila vacía](./images/empty_stack.png)

Vamos a agregar el primer elemento a la pila, en este el 10

![Se agrega 10 a la pila vacía](./images/added_10_to_stack.png)

Ahora vamos a agregar el 20, para agregar el 20 hay que tener en cuenta que el 10 cae al fondo de la pila, es decir, el 10 se convierte en el primer elemento de la pila, si agregamos el 20 quedaría de la siguiente manera:

![Se agrega 20 a la pila](./images/added_20_to_stack.png)

Siguiendo la misma lógica aplicada para el 20 ahora vamos a agregar el 30, quedando de la siguiente manera:

![Se agrega 30 a la pila](./images/added_20_to_stack.png)

La pila actual desde el fondo hasta la parte superior quedaría de la siguiente manera 10, 20 y 30. Si nosotros quisieramos eliminar el 10, en este caso no podríamos debido a que tenemos tanto el 30 como el 20 en medio, por lo tanto, es necesario eliminar primero desde la parte superior hasta llegar al fondo. Para este ejemplo en particular vamos a tener que eliminar el 30 luego el 20 y al final el 10 aplicando **LIFO (First In Last Out)**, es decir, 10 fue el primero en entrar a la pila pero el último en salir, veamos el ejemplo de manera gráfica con imágenes

![Eliminamos 30 de la pila](./images/removing_30_to_stack.png)

Ahora vamos a eliminar el 20 de la pila

![Eliminamos 20 de la pila](./images/removing_20_to_stack.png)

Ahora vamos a eliminar el último elemento de la pila en este caso el 10

![Eliminamos 10 de la pila](./images/removing_10_to_stack.png)

 De esta manera hemos agregado y eliminado elementos de la pila

## Colas

Las colas son estructuras de datos lineales que siguen el principio **FIFO (First In, First Out)**, lo que significa que el primer elemento que agregamos a la cola es el primer elemento en ser removido. Para visualizarlo de mejor manera, pensemos en una fila de banco, la primer persona que llegó es la primer persona en ser atendida

### Operaciones donde hacemos uso de **colas**

- **Enqueue**: Agrega un elemento al final (posterior) de la cola.
- **Dequeue**: Elimina y devuelve el elemento frontal de la cola.
- **Front (o Peek)**: Devuelve el elemento frontal de la cola sin eliminarlo.
