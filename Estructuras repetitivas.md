# ⭐ Estructuras Repetitivas en C

Las estructuras repetitivas permiten **ejecutar un bloque de instrucciones varias veces**, hasta que se cumpla una condición o se alcance un límite. Son esenciales para ciclos, automatización y cálculos repetidos. [13]

---

## 🔹 1. Bucle While

El bucle `while` ejecuta un bloque **mientras la condición sea verdadera**.  
Se usa cuando **no sabemos cuántas veces** se repetirá el ciclo, pero sí conocemos la condición de parada. [13]

## 📌 Ejemplo

Mostrar los números del **1 al 5** usando un `while`.

---

### 📝 Análisis del problema

## 📥 Datos de entrada
- No hay entrada del usuario.  
- Se usa una variable interna: `contador`.

## ⚙️ Proceso
1. Inicializar `contador = 1`.  
2. Mientras `contador <= 5`, mostrar su valor.  
3. Incrementar `contador` en cada repetición.

## 📤 Salida
- Se muestran los valores:
  - Contador: 1  
  - Contador: 2  
  - Contador: 3  
  - Contador: 4  
  - Contador: 5  

---

## 🧪 Pruebas de escritorio

| contador inicial | condición `contador <= 5` | salida        | contador nuevo |
|-----------------|---------------------------|---------------|----------------|
| 1               | Verdadero ✔️              | Contador: 1   | 2              |
| 2               | Verdadero ✔️              | Contador: 2   | 3              |
| 3               | Verdadero ✔️              | Contador: 3   | 4              |
| 4               | Verdadero ✔️              | Contador: 4   | 5              |
| 5               | Verdadero ✔️              | Contador: 5   | 6              |
| 6               | Falso ❌                  | —             | — (fin)        |

## 🧩 Diagrama de flujo
<img width="728" height="881" alt="image" src="https://github.com/user-attachments/assets/e7eec8d7-0348-470c-bba6-f6ab2cfa8654" />

## 💻 Ejercicio en C

```c
#include <stdio.h>

int main() {
    int contador = 1;

    while (contador <= 5) {
        printf("Contador: %d\n", contador);
        contador++;
    }

    return 0;
}
```
## Evidencia

<img width="141" height="109" alt="image" src="https://github.com/user-attachments/assets/5fabbc2a-f521-4b52-94af-4ce2a889cc3c" />


---

## 🔹 2. Bucle Do…While

A diferencia del `while`, este **siempre ejecuta el bloque al menos una vez**, porque la condición se evalúa **al final** del ciclo.  
Es útil cuando necesitamos **una ejecución mínima garantizada**. [14]

## 📌 Ejemplo

Solicitar al usuario que ingrese un **número positivo**.  
Si el número ingresado es negativo o cero, se vuelve a pedir.  

---

### 📝 Análisis del problema

## 📥 Datos de entrada
- Número ingresado por el usuario (entero).

## ⚙️ Proceso
1. Ejecutar al menos una vez el pedido del número.  
2. Mientras el número sea ≤ 0, volver a pedirlo.  
3. Mostrar el número válido ingresado.

## 📤 Salida
- **Número ingresado:** ✅  
- Solo se muestra cuando es positivo.

---

## 🧪 Pruebas de escritorio

| Intento | Número ingresado | Condición `numero <= 0` | Salida               |
|---------|-----------------|------------------------|---------------------|
| 1       | -3              | Verdadero ✔️           | Se pide de nuevo    |
| 2       | 0               | Verdadero ✔️           | Se pide de nuevo    |
| 3       | 5               | Falso ❌               | Número ingresado: 5 |

## 🧩 Diagrama de flujo
<img width="680" height="492" alt="image" src="https://github.com/user-attachments/assets/37ce7192-7679-4fe7-bb05-cd2b073a076c" />

## 💻 Código en C
```c
#include <stdio.h>

int main() {
    int numero;

    do {
        printf("Ingrese un número positivo: ");
        scanf("%d", &numero);
    } while (numero <= 0);

    printf("Número ingresado: %d\n", numero);

    return 0;
}
```
## Evidencia
<img width="327" height="80" alt="image" src="https://github.com/user-attachments/assets/204e9fb7-55d0-4602-853e-1be92ce43b6c" />

Vuelve a pedir ingresar el numero cada que ingrese un numero menor a 0

---

## 🔹 3. Bucle For

El bucle `for` se utiliza cuando conocemos **exactamente cuántas veces** queremos iterar.  
Incluye inicialización, condición e incremento en una misma línea, haciéndolo más compacto. [15]

### ✔ Ejemplo

Imprimir los números del **1 al 10** usando un bucle `for`.

---

### 📝 Análisis del problema

#### 📥 Datos de entrada
- Ninguno (los números son generados automáticamente del 1 al 10).

#### ⚙️ Proceso
1. Inicializar un contador `i` en 1.  
2. Mientras `i <= 10`, ejecutar:  
   - Imprimir el valor de `i`.  
   - Incrementar `i` en 1.  

#### 📤 Salida
- Se muestran los números del 1 al 10, cada uno en una línea.

---

### 🧪 Pruebas de escritorio

| Iteración | Valor de `i` | Condición `i <= 10` | Salida |
|-----------|---------------|--------------------|--------|
| 1         | 1             | Verdadero ✔️       | 1      |
| 2         | 2             | Verdadero ✔️       | 2      |
| 3         | 3             | Verdadero ✔️       | 3      |
| ...       | ...           | ...                | ...    |
| 10        | 10            | Verdadero ✔️       | 10     |
| 11        | 11            | Falso ❌           | Fin del bucle |

---

### 🧩 Diagrama de flujo
<img width="68" height="213" alt="image" src="https://github.com/user-attachments/assets/5ee29d53-847c-45d7-a267-6ac7cd5345dc" />

### Ejercicio en C
```c
#include <stdio.h>

int main() {
    for (int i = 1; i <= 10; i++) {
        printf("%d\n", i);
    }

    return 0;
}
```
## Evidencia

<img width="107" height="222" alt="image" src="https://github.com/user-attachments/assets/c55a9eae-19cf-428f-93e5-b8b1a75511aa" />


---
[Volver a la unidad 2](Unidad2.md)

[Volver al inicio](Inicio.md)
