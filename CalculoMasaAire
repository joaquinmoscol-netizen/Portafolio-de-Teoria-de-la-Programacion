## 🧮 Calcular la masa de aire

*Ejercicio: Escriba un programa que permita calcular la masa de aire con la siguiente fórmula: masa = (presión * volumen) / (0.37 * (temperatura + 460)). El ingreso de la masa, presión y volumen son cantidades enteras ingresadas por el usuario.

### ⚠️ Análisis del problema
* 🎯 El problema indica que "El ingreso de la masa, presión y volumen son cantidades enteras". Esto parece un error en el
planteamiento, ya que la **masa** es el resultado a calcular. 

**📥 Datos de entrada**
* 📝 Tres valores numéricos enteros ingresados por el usuario: `presion`, `volumen`, `temperatura`.
* 🔢 Asumiremos que los datos de entrada son **presión, volumen y temperatura** como enteros.

**⚙️ Proceso**
* 🧮 Fórmula: `masa = (presion * volumen) / (0.37 * (temperatura + 460))`
* El cálculo involucra una división y un número decimal (0.37), por lo que el resultado (`masa`) será un número real.

**📤 Salida**
* 🎯 El valor de la `masa` de aire (un valor real/decimal).

**📝 Pseudocódigo (PSeInt)**
```pseint
Algoritmo CalcularMasaAire
	Definir presion, volumen, temperatura Como Entero
	Definir masa Como Real
	
	// Datos de entrada
	Escribir "Ingrese la presión (entero):"
	Leer presion
	Escribir "Ingrese el volumen (entero):"
	Leer volumen
	Escribir "Ingrese la temperatura (entero):"
	Leer temperatura
	
	// Proceso
	masa <- (presion * volumen) / (0.37 * (temperatura + 460))
	
	// Salida
	Escribir "La masa de aire es: ", masa
FinAlgoritmo
```
## Prueba de escritorio
| presion | volumen | temperatura | Operación | Masa |
|---|---|---|---|---|
| 100 | 50 | 40 | (100 * 50) / (0.37 * (40 + 460)) | 27.027... |

# 📤Salida mostrada en Pseint
<img width="345" height="337" alt="image" src="https://github.com/user-attachments/assets/4ef75e75-b9e9-4fbd-9e40-3fbe164402a5" />

# 🧮Diagrama de Flujo

<img width="300" alt="Diagrama de Flujo Masa de Aire" src="https://github.com/user-attachments/assets/d4d2ee3c-b603-45aa-a14b-48d5b7e9ce25" />


**🖥️ Código en C**  
	
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


 # 🔢 Ejecucion en C
 <img width="467" height="119" alt="image" src="https://github.com/user-attachments/assets/29a15c82-f1cd-473c-b0fe-bd43613dc866" />


## 💡 Breve explicación
Este código toma tres datos ingresadas por el usuario como es la presion, la temperatura y el volumen, calcula la masa del aire y muestra el resultado en pantalla. 🎯
