## ¿Qué es un algoritmo?

Un algoritmo es un procedimiento computacional bien definido, finito y paso a paso que toma una entrada (o conjunto de entradas) —conocido como **input**— y produce una salida (o conjunto de salidas) —conocido como **output**—. Esencialmente, es una secuencia de instrucciones diseñadas para resolver un problema específico o realizar una tarea concreta.

Los algoritmos constituyen la columna vertebral de la informática: permiten procesar datos, realizar cálculos y automatizar la toma de decisiones. Desde operaciones simples hasta sistemas complejos como motores de búsqueda o modelos de inteligencia artificial, todos dependen de algoritmos.

Desde una perspectiva más formal, un algoritmo es una herramienta para resolver un **problema computacional bien especificado**. Dicho problema define la relación deseada entre la entrada y la salida, y el algoritmo proporciona un procedimiento preciso para lograr esa transformación.

Además, un algoritmo debe cumplir dos propiedades fundamentales:

- **Correctitud:** Para cada instancia de entrada, produce la salida correcta.
- **Terminación:** El algoritmo debe finalizar en un número finito de pasos.

---

### Ejemplo: Problema de Ordenación

Uno de los problemas más comunes en informática es el **problema de ordenación**, cuyo objetivo es reorganizar una secuencia de elementos en un orden específico, generalmente no decreciente.

- **Entrada (input):** Una secuencia de números
- **Salida (output):** Una permutación (reordenación) `(a1, a2, ..., an)` tal que  
  `a1 ≤ a2 ≤ ... ≤ an`

Cada conjunto de datos de entrada se denomina una **instancia del problema**. En general, una instancia consiste en los datos específicos necesarios para resolver un caso particular del problema.

Este problema es fundamental porque aparece como subrutina en múltiples aplicaciones: bases de datos, sistemas de búsqueda, análisis de datos, etc.

---

### ¿Por qué es valioso estudiar algoritmos?

1. **Eficiencia:**  
   Los algoritmos permiten resolver problemas de manera eficiente en términos de tiempo y recursos.  
   Por ejemplo, ordenar una lista utilizando **Quicksort** es considerablemente más rápido que usar **Bubble Sort** en conjuntos de datos grandes.

2. **Optimización:**  
   Permiten mejorar procesos reales.  
   Ejemplo: en logística, se utilizan algoritmos para encontrar rutas óptimas, reduciendo costos de transporte y tiempos de entrega.

3. **Escalabilidad:**  
   Un algoritmo eficiente puede manejar grandes volúmenes de datos, algo crucial en sistemas modernos como Big Data o machine learning.

4. **Innovación tecnológica:**  
   Tecnologías como motores de búsqueda, sistemas de recomendación y modelos de aprendizaje automático dependen de algoritmos sofisticados.

---

## Rol de los Algoritmos

Los algoritmos representan la lógica central detrás de cualquier proceso computacional. Aunque otras tecnologías son importantes, todas dependen de algoritmos para funcionar correctamente:

- **Hardware:**  
  Proporciona la infraestructura física (CPU, memoria, etc.) para ejecutar algoritmos.

- **Software:**

  Implementa algoritmos de forma accesible.  
  Ejemplo: un navegador web utiliza algoritmos para renderizar páginas, gestionar pestañas y ejecutar código JavaScript.

- **Bases de datos:**  
  Utilizan algoritmos para almacenar, recuperar y manipular datos eficientemente (por ejemplo, mediante índices o árboles de búsqueda).

- **Redes:**  
  Los protocolos de red emplean algoritmos para enrutar paquetes de datos de forma eficiente a través de Internet.

---

## Correctitud de los Algoritmos

Se dice que un algoritmo es **correcto** si, para cada instancia de entrada:

- Produce la salida correcta.
- Termina en un número finito de pasos.

Interesantemente, existen algoritmos **incorrectos o probabilísticos** que pueden ser útiles si su tasa de error es controlada.

---

Los diferentes algoritmos diseñados para resolver un mismo problema a menudo difieren drásticamente en su eficiencia.

## Comparación de algoritmos de ordenación

1. **Ordenación por inserción (Insertion Sort)**
   - Tiempo: $c_1 n^2$
   - Crecimiento: proporcional a $n^2$

2. **Ordenación por mezcla (Merge Sort)**
   - Tiempo: $c_2 \, n \log(n)$
   - Crecimiento: proporcional a $n \log(n)$

Para valores grandes de $n$, se cumple que:

- $\log(n) \ll n$
- Por lo tanto, $n \log(n) \ll n^2$

Esto implica que **Merge Sort es mucho más eficiente que Insertion Sort para entradas grandes**.

---

## Comparación en computadoras

### Computadora A

- Velocidad: $10^{10}$ instrucciones por segundo (10 billones)
- Algoritmo: **Insertion Sort**
- Número de elementos: $n = 10^7$

Tiempo de ejecución:

$$
T_A = \frac{2n^2}{10^{10}} = \frac{2(10^7)^2}{10^{10}} = \frac{2 \cdot 10^{14}}{10^{10}} = 2 \cdot 10^4 = 20000 \text{ segundos}
$$

- Resultado:  
  $20000$ segundos ≈ **5.5 horas**

---

### Computadora B

- Velocidad: $10^7$ instrucciones por segundo (10 millones)
- Algoritmo: **Merge Sort**
- Número de elementos: $n = 10^7$

Sabemos que:

$$
\log_2(10^7) \approx 23
$$

Tiempo de ejecución:

$$
T_B = \frac{50 \, n \log(n)}{10^7} = \frac{50 \cdot 10^7 \cdot 23}{10^7} = 50 \cdot 23 = 1150 \text{ segundos}
$$

- Resultado:  
  $1150$ segundos ≈ **19 minutos**

---

## Conclusión

- Aunque la **Computadora A es 1000 veces más rápida**, tarda más tiempo debido a un algoritmo ineficiente.
- La **Computadora B**, usando un mejor algoritmo, es mucho más rápida en la práctica.

**La eficiencia del algoritmo es más importante que la potencia del hardware.**
