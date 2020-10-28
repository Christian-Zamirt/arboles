# arboles

 Arbol

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

implementaciónen lenguaje C++


