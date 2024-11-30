---
marp: true
title: Introduccion a Python I
theme: default
header: FDTC 2024
---

# Futuros Dirigentes Técnicos Cientificos
## Nivel 6 - Informática

---

<!-- _class: invert-->
# ¿Qué es Informática?

---

### Informática
Es la disciplina que estudia el procesamiento, almacenamiento, transmisión y gestión de información mediante sistemas computacionales.

Combina principios teóricos, matemáticos y lógicos con herramientas tecnológicas para resolver problemas y automatizar tareas en diversos ámbitos, como ciencia, industria, educación y entretenimiento.

---

## Sobre este Curso
Durante el curso de FDTC, veremos las bases que necesitan para poder empezar nuestro camino en la informática y como esta nos puede ayudar a realizar proyectos que nos atraigan o ayuden en nuestra vida diaria.

---

<!-- _class: invert-->
# Introducción a Python

---

## Python

Es un lenguaje de programación multiparadigma que nos permite crear soluciones dentro de los campos de Aplicaciones Web, Proyectos IoT, Ciencia de Datos, Machine Learning e Inteligencia Artificial.

Aprenderemos sobre logica computacional, manipulacion de variables, estructura de datos, estructuras de flujo, uso de funciones y librerías.

![width:200px height:200px](python-logo.svg)

---

<!-- _class: invert-->
# Variables

---

### Declaración de Variables
Dentro de la programacion, lo que nos ayuda a guardar valores son las *variables*. Dichas variables guardan los valores para luego ser manipulados a nuestra necesidad. Usualmente al momento de programar, al nosotros declarar una variable podemos decir que le damos un **input** a dicha variable.

```python
# Primero le ponemos un nombre y luegole asignamos un valor a la variable
# nombre = valor
x = 10
```

---

### Impresión de Variables (OUTPUT)
La operación más básica dentro de la manipulación de variables es la **impresión**. Básicamente nos ayuda a desplegar información la cuál puede ser útil para un usuario.

```python
# Declaración
x = "Hola Mundo!"
# Imprimir en pantalla la variable x
print(x)
# es como decir print("Hola Mundo!")
```
---

### Asignacion de Variables (INPUT)
Dentro de la programacion, muchas veces se necesitan de variables con valores de acuerdo a las necesidades del usuario. Para ello, podemos utilizar la instruccion de *input()*, la cual permite solicitar un valor al usuario que este ejecutando el programa.

```python
# Programa que solicita el nombre al usuario
nombre = input("Ingrese su nombre") # nombre = Mario
print(nombre) # "Mario"
```

---

### Tipos de Datos
Una cualidad básica y fundamental de las variables son el *tipo*. Las variables tienen varios tipos datos que almacenana para tener un mejor entedimiento de como se pueden clasificar y manipular. Los tipos de datos se pueden desglosar en *primitivos* y *no-primitivos*. 

---

### Tipos de Datos: Primitivas
**Algunos** tipos de variables primitivas son:

- Integer (Número Entero)
- Float (Número Flotante; también llamado Decimal)
- String (Cadena de Carácteres; también llamado texto)

```python
# Variables Primitivas
x = 10               # Variable de Tipo entero
nombre = "Mario"     # Variable de Tipo Cadena de Caracteres
temperatura = 273.15 # Variable de Tipo Flotante
```

---

### Tipos de Variables: No Primitivas
**Algunos** tipos de variables no primitivas son:

- List (Lista)
- Set (Conjunto; listas con elementos unicos)
- Object (Objetos; tipos de datos especiales con)

```python
# Variables Primitivas
lista = [1,2,3,4]
conjunto = {1,2,3,4}
mi_objeto = Object()
```