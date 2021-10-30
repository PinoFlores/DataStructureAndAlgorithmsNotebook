# Estructuras De Datos Lineales

## Datos Estaticos

Este tipo de datos se caracterizan por:

- No se puede variar su ubicacion a lo largo de la ejecucion de programa.
- Se reserva su espacio en tiempo de compilacion. _Cuando el programa empieza su ejecucion es necesario saber de antemano su tamano y ubicacion en memoria._
- Se almacena en una zona estatica de la memoria: pila.
- El dato se identifica por una variable que no es mas que una direccion de memoria donde esta almacenada la informacion.
- Cuando se asigna un valor a ese dato, se almacena directamente en esa direccion de memoria.
- Cuando se accede a ese dato, se accede de forma directa al contenido de esa direccion de memoria.

## Punteros

Es un objeto cuyo valor se refiere o "apunta" a otro valor almacenado en otra parte de la memoria mediante una direccion. Por lo tanto un puntero referencia a una ubicacion en memoria.

# 1. Arrays / Matriz, Vector o Arreglos

Los Vectores son un tipo de estructura de datos estaticas, o sea, de tamano fijo. Pertenecen al tipo de estructuras de datos lineales. Un vector es almacenado en memoria de forma secuencia.

- Topics
  - Static
  - Dynamic
  - String
  - Searching
  - Sorting
    - Radix Sort
    - Quick Sort
    - Heap Sort
    - Bubble Sort
    - Selection Sort
    - Insertion Sort
    - Merge Sort
    - Counting Sort

| Algorithm  | Time   |
| ---------- | ------ |
| **Access** | O(1)   |
| **Push**   | O(1)   |
| **Search** | O(_n_) |
| **Insert** | O(_n_) |
| **Delete** | O(_n_) |

| Space |
| ----- |
| O(n)  |

**Example** A list of shopping cart

| Index | Value  |
| ----- | ------ |
| 0     | Apple  |
| 1     | Orange |
| 2     | Mango  |
| 3     | Grape  |
| 4     | Cheese |

| 0     | 1      | 2     | n-1 |
| ----- | ------ | ----- | --- |
| Apple | Orange | Mango | ... |

### Indices

`0, 1 , 2 , ... , n-1`

El primer elemento tiene como indice el **0**

```
vector[0] = Apple
```

El ultimo elemento tiene como indice el **n - 1**

```
n = 5
vector[n-1] = Cheese
```

### Longitud / Length

La longitud de un vector sera el total de elementos que en el se encuentran.

```
vector.length = 5
```

**Javascript Demo**

```
const fruits = ['Apple', 'Orange', 'Mango', 'Grape', 'Melon']; // <= Space O(n)

const primeraFruta = fruits[0]; // Applet <= Time O(1) : Acceso

const longitud = fruits.length; // 5

const ultimaFruta = fruits[longitud - 1]; // Melon  <= Time O(1) : Acceso
```

#### Metodos Predefinidos en Js

push
pop
