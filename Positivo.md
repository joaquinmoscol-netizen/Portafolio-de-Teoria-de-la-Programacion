# 🧮 Un número perfecto

**Ejercicio:** Realice un programa que determine si un número entero positivo n es o no perfecto. Un número perfecto es un entero que es igual a la suma de los divisores positivos menores que él mismo. Ejemplo 6 = 1+2+3.

## ⚠️ Prueba de escritorio

**Variables iniciales:**
* `n` = 6
* `suma` = 0
* `i` = (Variable del ciclo)

| Iteración | Valor de `i` | Condición `i < n` | ¿`n % i == 0`? | Acción | Nuevo valor de `suma` |
| :--- | :--- | :--- | :--- | :--- | :--- |
| 1 | 1 | Verdadero (1 < 6) | Sí | `suma = suma + i` | **1** (0 + 1) |
| 2 | 2 | Verdadero (2 < 6) | Sí | `suma = suma + i` | **3** (1 + 2) |
| 3 | 3 | Verdadero (3 < 6) | Sí | `suma = suma + i` | **6** (3 + 3) |
| 4 | 4 | Verdadero (4 < 6) | No | Ninguna | 6 |
| 5 | 5 | Verdadero (5 < 6) | No | Ninguna | 6 |
| 6 | 6 | Falso (6 < 6) | - | Fin del ciclo | 6 |

**Resultado:** `suma` (6) es igual a `n` (6) -> **Es perfecto**.

## 🖥️ Código en C  
	
	#include <stdio.h>

	int main() {
    int n, i, suma = 0;

    printf("Ingrese un numero entero positivo:");
    scanf("%d", &n);

    for(i = 1; i < n; i++) {
        if(n % i == 0) {
            suma = suma + i;
        }
    }

    if(suma == n) {
        printf("\n %d Es un numero perfecto.\n", n);
    } else {
        printf("\n %d No es un numero perfecto.\n", n);
    }

    return 0;
	}


**🔢 Ejecucion en C**

<<img width="483" height="90" alt="image" src="https://github.com/user-attachments/assets/31fc6c34-bc15-4a3d-bb5c-6bd51266f710" />

## 💡 Breve explicación
El código suma todos los divisores de un número (menores que él) y comprueba si esa suma es igual al número original para determinar si es "perfecto" 🎯

[Volver a la unidad 2](Unidad2.md)

[Volver al inicio](Inicio.md)
