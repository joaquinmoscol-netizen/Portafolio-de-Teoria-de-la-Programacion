## 🧮 Calcular la masa de aire

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

## Prueba de escritorio
| presion | volumen | temperatura | Operación | Masa |
|---|---|---|---|---|
| 100 | 50 | 40 | (100 * 50) / (0.37 * (40 + 460)) | 27.027... |
| 200 | 25 | 0 | (200 * 25) / (0.37 * (0 + 460)) | 29.382... |

**📝 Pseudocódigo (PSeInt)**
```pseint
Algoritmo CalcularMasaAire
	Definir presion, volumen, temperatura Como Entero
	Definir masa Como Real
	
	// 📥 Datos de entrada
	Escribir "Ingrese la presión (entero):"
	Leer presion
	Escribir "Ingrese el volumen (entero):"
	Leer volumen
	Escribir "Ingrese la temperatura (entero):"
	Leer temperatura
	
	// ⚙️ Proceso
	masa <- (presion * volumen) / (0.37 * (temperatura + 460))
	
	// 📤 Salida
	Escribir "La masa de aire es: ", masa
FinAlgoritmo

# 📤Salida mostrada en Pseint
<img width="345" height="337" alt="image" src="https://github.com/user-attachments/assets/3d26284b-36e6-47ec-93c2-9cb820249a71" />

# 🧮Diagrama de Flujo

<<img width="300" alt="Diagrama de Flujo Masa de Aire" src="" />/>


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

 # 💻 Ejecucion en C
 </>
  

## 💡 Breve explicación
Este código toma cuatro notas ingresadas por el usuario, calcula su promedio y muestra el resultado en pantalla. 🎯
