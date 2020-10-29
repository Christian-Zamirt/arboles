# Árbol 

Un árbol es una estructura de datos no lineal puesto que cada elemento apunta a uno o varios elementos del mismo tipo; esto es dado un elemento, no hay un único camino a seguir. El elemento que apunta a otro es llamado padre, mientras que el elemento apuntado se conoce como hijo. Todos los elementos tienen un padre a excepción de la raíz. Puede decirse que un árbol esta formado por subárboles resaltando así su naturaleza recursiva.

# ¿Qué es un árbol binario?

Un árbol binario es aquel es el que cada elemento apunta como máximo a otros 2 elementos, comúnmente llamados hijo izquierdo y hijo derecho.

![image](https://user-images.githubusercontent.com/72089660/97500667-993ffa00-1935-11eb-86e9-9af8dbfb6203.png)

# ¿Qué es un árbol binario de búsqueda?

Un árbol binario de buque da o ABB, es un árbol binario en el cual para todo elemento, los elementos mayores a él, se ubican en su rama derecha, mientras que los elementos menores van en su rama izquierda. Cada elemento se almacena una sola vez por lo que no existen elementos repetidos.


![image](https://user-images.githubusercontent.com/72089660/97501028-3a2eb500-1936-11eb-8dd5-f4d988aedbe0.png)

Cada elemento(nodo) de un árbol ABB cuenta con tres campos:

---Dato(numero, letra, palabra, etc), en este caso usaremos un numero(entero).

---Puntero al nodo derecho

---Puntero al nodo izquierdo

Los punteros tienen que ser del tipo árbol, ya que apuntaran a un nodo del mismo tipo, este seria un ejemplo de como se seria el tipo arbol ABB.

Primero creamos el nodo:

  struct nodo{
   int dato;
   struct nodo *der;
   struct nodo *izq;
  };

Los punteros son variables que guardaran en la memoria la dirección de otra variable en este caso la de una estructura llamado nodo.

# Recorridos de una árbol

Es la manera recursiva como pasaremos por cada nodo del árbol, existes tres formas:


---Enorden: Si visitamos primero hijo izquierdo, luego el padre y finalmente el hijo derecho

---Preorden: Primero el padre, luego el hijo izquierdo y finalmente el hijo derecho.

---Postorden: Primero hijo izquierdo, luego el hijo derecho y finalmente el padre

# implementación en lenguaje C++

Este programa se encargara de realizar los recorridos(amplitud) por Orden,pre-orden y post-orden, assi como tambien agregar 
nodos a el arbol y mostrarlo.

![image](https://user-images.githubusercontent.com/72089660/97506506-af9f8300-1940-11eb-8b3b-ffb87ed626f2.png)

Primero creamos el nodo:

  struct nodo{
   int dato;
   struct nodo *der;
   struct nodo *izq;
  }; como se a mostrado en la introduccion se sabe que un arbol consta de tres campos : dato, puntero derecho y puntero izquierdo.
en la funcion insertar es donde ocurre el proceso aqui por medio de la condicional if dice que el arbol no tiene ningun nodo, estos
los va a digitar el usuario y que si el nodo hijo exede  al nodo padre este se va a la derecha en cambio si es menor este va  la
izquierda.

![image](https://user-images.githubusercontent.com/72089660/97508651-c0062c80-1945-11eb-90c3-73339299e063.png)

En la funcion preOrden se hace el recorrido empezando en el nodo padre,luego al nodo hijo izquierdo y finalizando con el nodo hijo derecho.

En la siguiente funcion es donde hace el proceso de ordenar el recorrido(amplitud) En orden quiere decir que se va empezar   
el recorrido del nodo hijo izquierdo, luego el nodo padre y finalizando con el nodo hijo derecho.

En la funcion postOrden el recorrido empieza del nodo hijo dereho,luego el padre y finalizando con el nodo hijo izquierdo

![image](https://user-images.githubusercontent.com/72089660/97509758-c6e26e80-1948-11eb-9ed6-659954842b41.png)

En el main se encargara de llamar las funciones empleadas para realizar el proceso, asi como mostrar en pantalla el numero de nodos,
 los recorridos efectuados y mostrar el arbol 
 
 # Resultado
 
 
