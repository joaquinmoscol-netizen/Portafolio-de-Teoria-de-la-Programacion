## 💰 Calcular nuevo sueldo con incremento

**Tercer Ejercicio:** Un empleado de la empresa "Mi tienda es tuya" recibe un sueldo mensual, por su trabajo ha recibido un incremento del 25% sobre su sueldo anterior. Desarrolle un programa que permita calcular el nuevo sueldo del empleado.

### ⚠️ Análisis del problema
* 🎯 El problema es directo: se debe leer un sueldo y calcular su valor + 25%.

**📥 Datos de entrada**
* 📝 Un valor numérico real ingresado por el usuario: `sueldo_anterior`.

**⚙️ Proceso**
* 🧮 Fórmula: `nuevo_sueldo = sueldo_anterior * 1.25`
* (Esto es lo mismo que `sueldo_anterior + (sueldo_anterior * 0.25)`)

**📤 Salida**
* 🎯 El valor del `nuevo_sueldo` (real).

**📝 Pseudocódigo (PSeInt)**
```pseint
Algoritmo CalcularNuevoSueldo
	Definir sueldo_anterior, nuevo_sueldo Como Real
	
	// Datos de entrada
	Escribir "Ingrese el sueldo anterior:"
	Leer sueldo_anterior
	
	// Proceso
	nuevo_sueldo <- sueldo_anterior * 1.25
	
	// Salida
	Escribir "El nuevo sueldo con 25% de incremento es: $", nuevo_sueldo
FinAlgoritmo
```
## Prueba de escritorio
| sueldo anterior | operacion | sueldo actual | 
|---|---|---|
| 1000 | 1000 * 1.25 | 1250 | 

# 📤Salida mostrada en Pseint
<img width="540" height="152" alt="image" src="https://github.com/user-attachments/assets/bc8fbcc4-1cf3-4f3f-9e62-830e1c006f06" />

# 🧮Diagrama de Flujo
<img width="854" height="1026" alt="image" src="https://github.com/user-attachments/assets/5f08097c-2350-40fe-94f2-d5fc2f3fd528" />

**🖥️ Código en C**  
	
	#include <stdio.h>
  
	int main() {
	  float sueldo_anterior, nuevo_sueldo;
	
  	// Datos de entrada
  	printf("Ingrese el sueldo anterior: ");
  	scanf("%f", &sueldo_anterior);
  	
  	// Proceso
  	nuevo_sueldo = sueldo_anterior * 1.25;
  	
  	// Salida
  	// Se usa %% para imprimir un solo %
  	printf("El nuevo sueldo con 25%% de incremento es: $%.2f\n", nuevo_sueldo);
  	
	  return 0;
    }

 # 🔢 Ejecucion en C
<img width="661" height="75" alt="image" src="https://github.com/user-attachments/assets/85fc3450-40b0-42f4-b58e-cf7b6a4b8856" />

## 💡 Breve explicación
Este código toma el sueldo actual de un empleado, le aplica un incremento del 25% y muestra el nuevo sueldo total. 📈💸
