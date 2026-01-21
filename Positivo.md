# 🧮 Un número perfecto

**Ejercicio:** Realice un programa que determine si un número entero positivo n es o no perfecto. Un número perfecto es un entero que es igual a la suma de los divisores positivos menores que él mismo. Ejemplo 6 = 1+2+3.

## ⚠️ Prueba de escritorio
| presion | volumen | temperatura | Operación | Masa |
|---|---|---|---|---|
| 100 | 50 | 40 | (100 * 50) / (0.37 * (40 + 460)) | 27.027... |

## 🖥️ Código en C  
	
	#include <stdio.h>
	
	int main() {
		int presion, volumen, temperatura;
		float masa;
		
		// Datos de entrada
		printf("Ingrese la presión (entero): ");
		scanf("%d", &presion);
	
		printf("Ingrese el volumen (entero): ");
		scanf("%d", &volumen);
		
		printf("Ingrese la temperatura (entero): ");
		scanf("%d", &temperatura);
		
		getchar();
		
		// Proceso
		
		masa = (float)(presion * volumen) / (0.37 * (temperatura + 460));
		
		// Salida
		
		printf("La masa de aire es: %.3f\n", masa);
		
		getchar();
		
		return 0;
	}


**🔢 Ejecucion en C**

<img width="467" height="119" alt="image" src="https://github.com/user-attachments/assets/29a15c82-f1cd-473c-b0fe-bd43613dc866" />


## 💡 Breve explicación
Este código toma tres datos ingresadas por el usuario como es la presion, la temperatura y el volumen, calcula la masa del aire y muestra el resultado en pantalla. 🎯

[Volver a la unidad 2](Unidad2.md)

[Volver al inicio](Inicio.md)
