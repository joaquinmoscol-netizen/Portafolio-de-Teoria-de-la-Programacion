# 🔹 Explicación de Ejemplos de Algoritmos Secuenciales  

## ¿Qué es una Estructura Secuencial?

Una **Estructura Secuencial** (o Lineal) es la forma más básica de un algoritmo. En ella, las instrucciones se ejecutan en perfecto orden, una después de la otra, desde el "Inicio" hasta el "Fin". No hay saltos, ni decisiones (condicionales), ni repeticiones (ciclos).

<img width="406" height="680" alt="image" src="https://github.com/user-attachments/assets/3758ad00-7c75-40a3-a14c-9a8c4e811897" />


**Explicación de la imagen:** Este es un concepto visual de una secuencia. Imagina una receta:
1.  Leer ingredientes (Entrada).
2.  Mezclar ingredientes (Proceso).
3.  Servir (Salida).

No puedes hacer el paso 2 sin el 1. Ese orden estricto es una estructura secuencial.

---

## Pasos para Escribir un Algoritmo

Tu presentación indica que siempre seguimos tres pasos fundamentales:

<img width="396" height="700" alt="image" src="https://github.com/user-attachments/assets/3ac0cecd-a788-4754-a9d2-53253e89ee11" />

**Explicación de la imagen:** Esta diapositiva resume el método de trabajo:
1.  **Análisis del problema:** Es el "¿Qué necesito?". Aquí identificamos las **Entradas**, **Procesos** (fórmulas) y **Salidas** (resultados).
2.  **Desarrollo del algoritmo:** Es el "¿Cómo lo hago?". Aquí escribimos las instrucciones (el pseudocódigo o el diagrama de flujo).
3.  **Validación o prueba de escritorio:** Es el "¿Funciona?". Hacemos un seguimiento manual para ver si el resultado es correcto.

---

## Ejemplo 1: Suma de dos números

* **Objetivo:** Determinar la suma de dos números.

### 1. Análisis del Problema
* **Entrada:** `num1`, `num2` (Los dos números a sumar).
* **Proceso:** `suma = num1 + num2` (La operación aritmética).
* **Salida:** `suma` (El resultado del cálculo).

### 2. Desarrollo (Imagen)
<img width="200" height="235" alt="image" src="https://github.com/user-attachments/assets/11f0d33e-57e6-45e4-9d9a-b657d865c844" />

#### Diagrama de Flujo
<img width="215" height="288" alt="image" src="https://github.com/user-attachments/assets/7a2cb8cd-a69a-4860-84fe-9f5cf645dc54" />


**Explicación de la imagen (Diagrama):**
* `Inicio`: Marca el comienzo.
* `Leer num1` / `Leer num2`: (Paralelogramo) Símbolos de **Entrada**. Le pedimos al usuario los dos valores.
* `suma <- num1 + num2`: (Rectángulo) Símbolo de **Proceso**. Aquí es donde la computadora realiza el cálculo.
* `Mostrar suma`: (Paralelogramo) Símbolo de **Salida**. Le mostramos al usuario el resultado guardado en `suma`.
* `Fin`: Marca el final.

#### Pseudocódigo (PSeint)
<img width="202" height="223" alt="image" src="https://github.com/user-attachments/assets/965056ed-28ef-4c7c-a011-8fc16a052e8a" />

**Explicación de la imagen (Pseudocódigo):**
Esto es lo mismo que el diagrama, pero escrito en palabras:
* `// Variables`: Un comentario para explicar que definimos las variables `num1` y `num2` como `Real`.
* `// Entrada`: Comentario que indica que `Leer num1` y `Leer num2` son las instrucciones de entrada.
* `// Proceso`: Comentario que indica que `sumar = num1 + num2` es la instrucción de asignación y cálculo.
* `//Salida`: Comentario que indica que `Escribir sumar` es la instrucción de salida.

**Pruebas de Escritorio}:**
Simular datos de entrada, para comprobar que los resultados sean correctos.
De no ser ası́, será necesario revisar el análisis del problema y el código del algoritmo para aplicar las respectivas correcciones y repetir la prueba de escritorio hasta obtener los datos de salida esperados o correctos.

<img width="440" height="170" alt="image" src="https://github.com/user-attachments/assets/a111be24-613c-450d-ae6a-f181dd366d81" />

---

## Ejemplo 2: Superficie (Área) de un Triángulo

* **Objetivo:** Conocer la superficie de un triángulo usando su base y altura.

### 1. Análisis del Problema
* **Entrada:** `base`, `altura`.
* **Proceso:** `area = (base * altura) / 2` (La fórmula matemática del área).
* **Salida:** `area`.

### 2. Desarrollo (Imagen de la Presentación)

#### Diagrama de Flujo
<img width="242" height="289" alt="image" src="https://github.com/user-attachments/assets/d279c71e-80b6-4635-8042-84861f353924" />

**Explicación de la imagen:**
Es otra estructura secuencial:
1.  `Inicio`.
2.  `Pedir base` (Entrada).
3.  `Pedir altura` (Entrada).
4.  `area <- (base * altura) / 2` (Proceso). Se usan los operadores `*` (multiplicación) y `/` (división).
5.  `Presentar area` (Salida).
6.  `Fin`.

---

## Ejemplo 3: Longitud y Área de un Círculo

* **Objetivo:** Calcular la longitud de la circunferencia Y el área de un círculo, pidiendo solo el radio.

### 1. Análisis del Problema
* **Entrada:** `radio`.
* **Constante:** `PI` (Un valor fijo, como 3.14159).
* **Proceso:** Se necesitan dos cálculos:
    1.  `longitud = 2 * PI * radio`
    2.  `area = PI * radio ^ 2` (El `^` es el operador de potencia).
* **Salida:** `longitud` y `area` (dos resultados).

### 2. Desarrollo (Imagen de la Presentación)

#### Diagrama de Flujo
<img width="206" height="304" alt="image" src="https://github.com/user-attachments/assets/caf816d3-ee1d-4799-916d-5a4791f3f185" />


**Explicación de la imagen:**
Este ejemplo muestra múltiples procesos y múltiples salidas, pero sigue siendo secuencial (uno después del otro).
1.  `Inicio`.
2.  `Leer radio` (Entrada).
3.  `longitud <- 2 * PI * radio` (Proceso 1).
4.  `area <- PI * radio ^ 2` (Proceso 2).
5.  `Mostrar longitud` (Salida 1).
6.  `Mostrar area` (Salida 2).
7.  `Fin`.


[⬅️ Volver a Unidad 1](Unidad%201.md)
