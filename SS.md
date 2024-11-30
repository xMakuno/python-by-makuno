---
marp: true
title: Ordenamiento y Búsqueda
theme: default
header: FDTC 2024
---

# Futuros Dirigentes Técnicos Científicos
## Nivel 6 - Informática

---

<!-- _class: invert-->
# Introducción a Algoritmos

---

### ¿Qué es un Algoritmo?
Un algoritmo es un conjunto de pasos bien definidos que se siguen para resolver un problema o realizar una tarea.

```plaintext
Inicio
1. Leer dos números.
2. Sumar los números.
3. Imprimir el resultado.
Fin
```

---

### ¿Para qué sirven los algoritmos?
Los algoritmos son fundamentales porque:

- Proveen soluciones claras y estructuradas.
- Pueden ser traducidos a lenguajes de programación.
- Son esenciales en áreas como la inteligencia artificial, análisis de datos y sistemas operativos.

---

<!-- _class: invert-->
# Ordenamiento y Búsqueda

---

### ¿Qué es Ordenar?
El ordenamiento es el proceso de organizar elementos de una colección en un orden específico, como:

- Orden ascendente (menor a mayor).
- Orden descendente (mayor a menor).

```plaintext
Entrada: [3, 1, 4, 1, 5]
Salida (ascendente): [1, 1, 3, 4, 5]
```

---

### ¿Qué es Buscar?
La búsqueda implica encontrar un elemento específico dentro de una colección. Puede ser:

- Exacta: Buscar un valor específico.
- Por rango: Buscar valores que cumplan ciertos criterios.

```plaintext
Arreglo: [10, 20, 30, 40, 50]
Buscar: 30
Resultado: Índice 2
```

---

<!-- _class: invert-->
# Algoritmos de Ordenamiento

---

### Burbuja (Bubble Sort)
Es un algoritmo simple que compara pares de elementos adyacentes y los intercambia si están en el orden incorrecto.

```python
def bubble_sort(arr):
    n = len(arr)
    for i in range(n):
        for j in range(0, n-i-1):
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]

```

---

### Rápido (Quick Sort)
Divide y conquista: selecciona un pivote y organiza elementos menores a la izquierda y mayores a la derecha.

```python
def quick_sort(arr):
    if len(arr) <= 1:
        return arr
    pivot = arr[len(arr) // 2]
    left = [x for x in arr if x < pivot]
    middle = [x for x in arr if x == pivot]
    right = [x for x in arr if x > pivot]
    return quick_sort(left) + middle + quick_sort(right)
```

---

<!-- _class: invert-->
# Algoritmos de Búsqueda

---

### Búsqueda Lineal
Busca un elemento revisando uno por uno desde el inicio hasta el final.

```python
def linear_search(arr, x):
    for i in range(len(arr)):
        if arr[i] == x:
            return i
    return -1

```


---

### Búsqueda Binaria
Funciona en arreglos ordenados, dividiendo el rango de búsqueda a la mitad en cada paso.

```python
def binary_search(arr, x):
    low, high = 0, len(arr) - 1
    while low <= high:
        mid = (low + high) // 2
        if arr[mid] == x:
            return mid
        elif arr[mid] < x:
            low = mid + 1
        else:
            high = mid - 1
    return -1
```

---

<!-- _class: invert-->
# Aplicación de Algoritmos

---

### Importancia de Algoritmos de Ordenamiento y Búsqueda

- Ordenar facilita análisis, búsqueda y clasificación de datos.
- Son la base de sistemas más complejos como bases de datos y motores de búsqueda.

Ejemplo práctico: Buscadores como Google ordenan páginas por relevancia y las encuentran rápidamente.

