# Resumen:
■■■■■■■


## Requisitos Mínimos:

- Elementos léxicos de python o [Keywords](https://realpython.com/python-keywords/)
- Convenciones de estilo [PEP8](https://www.python.org/dev/peps/pep-0008/)
- Operadores, Manejo de Strings y Literals.
- Entender sobre Listas, Tuplas, Conjuntos, Diccionarios.

## Tener claro:

- Declaración de funciones
- Recursividad
- Funciones anidades
- High Order Functions
- Funciones lambda.
- Programación Orientada a Objetos

## Nice to Have:

- Manejo de excepciones
- Manipulación de archivos.

---

# Tipos de colecciones
Nos referimos a las estructuras de datos. Una colección es un grupo de cero o más elementos que pueden tratarse como una unidad conceptual.

## Tipos de datos.

- Non-zeo Value
- Cero
- null
- undefined
Estos tipos de dato también pueden formar parte de una colección. Existen colecciones de tipo Dinámicas que son aquelas que pueden variar su tamaño y las Inmutables que no cambian su tamaño.

## Estructuras Lineales

De forma general encontramos estructuras de datos lineales que están definidas por sus índices. Es decir puedo encotnrarme estrcuturas de datos lineales que sean dinámicas o inmutables, de ello variarán sus propiedades, como poner un elemento al final, (sucesor) o no.

* Te encontrarás con Listas, Listas Ordenadas, Cola, Cola de prioridad y más.

Es decir está ordenadas por posición.
Solo el primer elemento no tiene predecesor

Ej:

- Una fila para un concierto
- Una pila de platos por lavar, o una pila de libros por leer.
-Checklist, una lista de mercado, la lista de Schindler

* Estructuras Jerárquicas

- Estructuras basadas en una jerarquia definida.
- Los árboles pueden tener n números de nieleves hacia abajo o adyacentes. Te encotnrarás con árboles Binarios, Montículos.

- Ordendas como árbol invertido (raices)
- Solo el primer nodo no tiene predecesores, pero si sucesores.
Es un sistema de padres e Hijos.
Ej:

- Libros, Capítulos, Temas.
- Abuelos, Madres, Hijos.
- Estructuras Grafos:

Cada dato puede tener varios predecesores y sucesores, se les llama vecinos
Los elementos se relecionan entre si con n relaciones.
Ej:

- Vuelos aéreos, sistemas de recomendación
- La mismísima interntet es un grafo

* Estructuras Desordenadas:
- Estructuras como Bolsa, Bolsa ordenada, Conjuntos, DIccionarios, Diccionario ordenados.

No tienen orden en particular
No hay predecesores o sucesores.
Ej:

- Una bolsa de gomitas, no sabe de qué color te va a tocar.

* Estructuras Ordenadas:
Son estructuras que imponen un orden con una regla. Generalmente una regla de orden.
item <= item(i+1) Es decir que el item que sigue es el primer elemento +1.

Ej:

- Los directorios telefónicos, los catálogos,

---

Conclusión:

Suponga que tiene un dataset con muchos datos, una colección de libros, música, fotos, y desea ordenar esta colección, ante esta situación siempre existe el Trade Off entre rapidez/costo/memoria El conocimeinto de las propiedades de las colecciones te facilitará la selección de estructura de datos según sea el caso y velar por un software eficiente.

## Taxonomía:

- Colección:
  - Grafos
  - Jerárquicas
    - Árbol binario
    - Montículo
  - Lineales:
    - Lista
      - Lista Ordenada
    - Cola
      - Cola de prioridad
    - Pila
    - String
  - Desordenadas:
    - Bolsa
      - Bolsa Ordenada
    - Diccionario
      - Diccionario ordenado
    - Conjunto
      - Conjunto ordenado
---

# Operaciones Esenciales en Colecciones:
Algunas operaciones básicas responden necesidades puntuales como saber:

- Tamaño: Las dimensiones
- Pertenencia: Si un elemento pertenece o no.
- Recorrido: Pasar por los elementos
- String: Converir la colección a un string.
- Igualdad: Comparar colecciones
- Concatenación: Unir o sumar listas
- Conversión de tipo: Convertir tipos de datos entre si
- Insertar, Remover, Reemplazar, Acceder a n elementos en n posición.

Aquí se hace referencia a los métodos nativos de python para hacer ordenamientos, insertar, acceder y remover elementos. sort(), remove(), pop() Estos métodos son útiles para determinadas tareas.

---

# Colecciones Incorporadas en Python

- Listas: Propósito general, de índices con tamaños dinámicos. Ordenables lista =[].
Usaria las listas para almacenar una serie de números, una lista de palabras,y básicamente cualquier cosa.
- Tuplas: Inmutables, no se pueden añadir más elementos. Utiles para constantes por ejemplo coordenadas, direcciones. Es de tipo secuencial. tupla =()

Las usuaría cuando sé exactamente el tamaño que tendrán mis datos.

- Conjuntos: Almacenan objetos no duplicados.(Teoría de conjuntos), son de acceso rápido, aceptan operaciones lógicas, son desordenados.set() conjunto={1,2,3,4}

Usaría un casteo entre conjuntos y listas cuando quiero eliminar duplicados de una lista.

- Diccionarios: Pares de llaver valor, arrays asociativos (hash maps), son desordenados, y muy rápidos para hacer consultas. diccionario ={'Llave':"Valor"}

Los usaría para almacenar datos, listas, objetos que perfectamente pueden volverse un dataframe, o un defaultdict

---
