# ⭐ Estructuras Condicionales en C

Las estructuras condicionales permiten **tomar decisiones** dentro de un programa según el valor de una condición lógica. Son fundamentales para controlar el flujo del software y decidir qué bloque de código se ejecuta. [9]

---

## 🔹 1. If Simple

La estructura `if` simple evalúa una condición.  
Si es verdadera (**true**) se ejecuta el bloque; si es falsa (**false**) se ignora. Es útil cuando solo se debe comprobar una condición. [9]

# Ejemplo

Se necesita elaborar un procedimiento que permita ingresar un número y mostrar el mensaje "El número es positivo" únicamente cuando el valor ingresado sea mayor que cero.

## 📝 Analisis del problema

# Datos de entrada
- Un número entero ingresado por el usuario.

# Proceso
- Verificar si el número es mayor que cero.
# Salida
- Mensaje en pantalla (solo si la condición se cumple):
  - **El número es positivo**
- Si el número no es mayor que cero, no hay salida.

## Pruebas de escritorio

| Entrada (numero) | Condición (numero > 0) | Salida esperada                 |
|------------------|------------------------|---------------------------------|
| 10                | Verdadero              | "El número es positivo"         |
| 0                | Falso                  | *No muestra ningún mensaje*     |


## 🧩 Diagrama de flujo

<img width="300" height="1029" alt="image" src="https://github.com/user-attachments/assets/dcc03561-8534-4495-bd83-74667dc61851" />



## 💻 Ejercicio en C
```c
#include <stdio.h>

int main() {
    int numero;
    printf("Ingrese un número: ");
    scanf("%d", &numero);

    if (numero > 0) {
        printf("El número es positivo\n");
    }

    return 0;
}

```
## Evindencia

<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/dfa98ae2-e9aa-4722-aca3-ca4dfb11a83b" />


---


# 🔹 2. If – Else

Se utiliza cuando se requiere escoger entre **dos posibles resultados**.  
Si se cumple la condición se ejecuta el primer bloque; si no, el segundo. [10]

# ✔ Ejemplo 

## 📝 Analisis del problema

Se necesita elaborar un procedimiento que permita ingresar la edad de una persona y mostrar el mensaje "Eres mayor de edad" si tiene 18 años o más; caso contrario, mostrar "Eres menor de edad".


# Datos de entrada
- La edad de la persona (entero).

# Proceso
- Verificar si la edad es mayor o igual a 18.

## Salida
- **Eres mayor de edad** (cuando edad ≥ 18)
- **Eres menor de edad** (cuando edad < 18)

# Pruebas de escritorio

| Entrada (edad) | Condición (edad ≥ 18) | Salida esperada        |
|----------------|------------------------|-------------------------|
| 19             | Verdadero              | "Eres mayor de edad"    |
| 11             | Falso                  | "Eres menor de edad"    |

## 🧩 Diagrama de flujo
<img width="300" height="1029" alt="image" src="https://github.com/user-attachments/assets/681b010a-d2a5-4c18-9a83-b01962b53003" />

## 💻 Ejercicio en C

```c
#include <stdio.h>

int main() {
    int edad;
    printf("Ingrese su edad: ");
    scanf("%d", &edad);

    if (edad >= 18) {
        printf("Eres mayor de edad\n");
    } else {
        printf("Eres menor de edad\n");
    }

    return 0;
}
```
## Evidencia
### Verdadero
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/1699c4d5-318c-464e-ab51-f40cd5c96fc4" />

### Falso
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/68adf123-07ad-4754-a68d-66fe56752eea" />


---

## 🔹 3. If – Else If – Else

Se usa cuando existen **múltiples alternativas**.  
Las condiciones se evalúan en orden; la primera verdadera se ejecuta. [11]

# ✔ Ejemplo

## 📝 Analisis del problema

Se necesita elaborar un procedimiento que permita ingresar la nota de un estudiante y mostrar un mensaje según el rango obtenido:
- "Excelente" si la nota es mayor o igual a 90  
- "Aprobado" si la nota está entre 70 y 89  
- "Reprobado" si la nota es menor a 70


# Datos de entrada
- La nota del estudiante (entero).

# Proceso
- Verificar si la nota es mayor o igual a 90 → mostrar "Excelente".
- Si no, verificar si la nota es mayor o igual a 70 → mostrar "Aprobado".
- De lo contrario → mostrar "Reprobado".

# Salida
- **Excelente** (nota ≥ 90)  
- **Aprobado** (70 ≤ nota < 90)  
- **Reprobado** (nota < 70)

# Pruebas de escritorio

| Entrada (nota) | Condición evaluada                   | Resultado de la condición | Salida esperada |
|----------------|---------------------------------------|----------------------------|------------------|
| 95             | nota ≥ 90                             | Verdadero                  | "Excelente"      |
| 75             | nota ≥ 90 → Falso, nota ≥ 70 → Verdadero | Verdadero en el 2do caso  | "Aprobado"       |
| 60             | nota ≥ 90 → Falso, nota ≥ 70 → Falso  | Falso                      | "Reprobado"      |

## 🧩 Diagrama de flujo
<img width="300" height="1029" alt="image" src="https://github.com/user-attachments/assets/0fa6c221-27c0-40b0-9657-955898af0bc2" />

## 💻 Ejercicio en C
```c
#include <stdio.h>

int main() {
    int nota;
    printf("Ingrese la nota: ");
    scanf("%d", &nota);

    if (nota >= 90) {
        printf("Excelente\n");
    } else if (nota >= 70) {
        printf("Aprobado\n");
    } else {
        printf("Reprobado\n");
    }

    return 0;
}
---

```
## Evidencia 

### Caso 1
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/047515c4-8635-4a96-a49f-941329c78754" />

### Caso 2
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/cc503026-aa93-482a-b410-5fe3a7f97c0c" />

### Caso 3
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/88924f90-52ec-4122-b297-6d0d04018b5b" />


## 🔹 4. Switch – Condicional Múltiple

`Switch` compara una variable contra varios valores posibles (casos).  
Es ideal cuando las opciones son **claras y constantes**, haciendo el código más limpio que muchos `if`. [12]

# ✔ Ejemplo 

## 📝 Analisis del problema

Se necesita elaborar un procedimiento que permita ingresar dos números y elegir una operación para mostrar su resultado:
- 1 → Suma  
- 2 → Resta  
- 3 → Multiplicación  
- Cualquier otro número → “Opción no válida”


# Datos de entrada
- Número 1 (entero o real)  
- Número 2 (entero o real)  
- Opción de operación elegida (entero)

# Proceso
3. Evaluar la opción con `switch`:
   - Si es 1 → sumar los números.
   - Si es 2 → restar número1 – número2.
   - Si es 3 → multiplicar los números.
   - Si no es ninguna de las anteriores → mostrar “Opción no válida”.

# Salida
- Resultado de la operación seleccionada, o
- Mensaje: **"Opción no válida"**

# Pruebas de escritorio

| Número 1 | Número 2 | Opción | Operación evaluada | Salida esperada              |
|----------|----------|--------|---------------------|-------------------------------|
| 8        | 4        | 1      | Suma                | 12                            |
| 10       | 3        | 2      | Resta               | 7                             |
| 6        | 7        | 3      | Multiplicación      | 42                            |
| 5        | 2        | 9      | Default             | "Opción no válida"            |

## 🧩 Diagrama de flujo
<img width="300" height="1029" alt="image" src="https://github.com/user-attachments/assets/61b410b4-2796-468a-aeb0-8be75e243772" />

## 💻 Ejercicio en C

```c
#include <stdio.h>

int main() {
    int opcion;
    float num1, num2;

    printf("Ingrese el primer número: ");
    scanf("%f", &num1);

    printf("Ingrese el segundo número: ");
    scanf("%f", &num2);

    printf("1. Suma\n2. Resta\n3. Multiplicación\nSeleccione una opción: ");
    scanf("%d", &opcion);

    switch (opcion) {
        case 1:
            printf("Resultado: %.2f\n", num1 + num2);
            break;
        case 2:
            printf("Resultado: %.2f\n", num1 - num2);
            break;
        case 3:
            printf("Resultado: %.2f\n", num1 * num2);
            break;
        default:
            printf("Opción no válida\n");
            break;
    }

    return 0;
}
```
## Evidencia
# Caso 1
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/e40d46a9-cb97-40e6-9680-f43beaba9e9d" />

# Caso 2
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/b6903d55-25da-4642-af4c-b7fc7abf2e2a" />

# Caso 3
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/915c9828-5720-46c5-a1f5-0a2a26bc12c9" />

# Caso Falso
<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/c0aa936c-191d-4fd9-a9fb-d458f94b7c10" />

---

[Volver a la unidad 2](Unidad2.md)

[Volver al inicio](Inicio.md)




