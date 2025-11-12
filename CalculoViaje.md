## 🚌 Calcular costo total de viaje a Baños

**Cuarto Ejercicio:** Un grupo de 8 amigos realiza un viaje a la ciudad de Baños, 3 de ellos se transportan en taxi ejecutivo, 2 de ellos en buseta turística y 3 de ellos en bus regular. El bus regular cuesta un 20% menos que el taxi ejecutivo. Desarrolle un programa que permita calcular el costo total del viaje, considerando el costo de cada tipo de transporte ingresado por el usuario.

### ⚠️ Análisis del problema
* 🎯 El problema no proporciona los costos base, por lo que el programa debe solicitar el costo del "taxi ejecutivo" y el de la "buseta turística" (por persona).
* 🎯 El costo del bus regular se *calcula* (20% menos que el taxi), no se pide.

**📥 Datos de entrada**
* 📝 Dos valores numéricos (reales): `costo_taxi` (por persona) y `costo_buseta` (por persona).

**⚙️ Proceso**
* 🧮 Calcular el costo del bus regular: `costo_bus_regular = costo_taxi * 0.80`
* 🧮 Calcular el costo total para cada grupo:
    * `total_taxi = 3 * costo_taxi`
    * `total_buseta = 2 * costo_buseta`
    * `total_bus_regular = 3 * costo_bus_regular`
* 🧮 Calcular el costo total del viaje: `total_viaje = total_taxi + total_buseta + total_bus_regular`

**📤 Salida**
* 🎯 El `total_viaje` que pagarán los 8 amigos.

**📝 Pseudocódigo (PSeInt)**
```pseint
Algoritmo CostoViajeBanios
	Definir costo_taxi, costo_buseta, costo_bus_regular Como Real
	Definir total_taxi, total_buseta, total_bus_regular, total_viaje Como Real
	
	// Datos de entrada
	Escribir "Ingrese el costo del pasaje en taxi ejecutivo (por persona):"
	Leer costo_taxi
	Escribir "Ingrese el costo del pasaje en buseta turística (por persona):"
	Leer costo_buseta
	
	// Proceso
	costo_bus_regular <- costo_taxi * 0.80 // 20% menos que el taxi
	
	total_taxi <- 3 * costo_taxi
	total_buseta <- 2 * costo_buseta
	total_bus_regular <- 3 * costo_bus_regular
	
	total_viaje <- total_taxi + total_buseta + total_bus_regular
	
	// Salida
	Escribir "El costo total del viaje para los 8 amigos es: $", total_viaje
FinAlgoritmo
```
## Prueba de escritorio
| Costo Taxi | Costo Buseta | Costo Bus Regular | Total Taxi | Total Buseta | Total Bus Regular | Total Viaje|
|---|---|---|---|---|---|---|
| 10 | 8 | 10 * 0.8 = 8 | 10 * 3 = 30 |	8 * 2 = 16 | 8 * 3 = 24 | 30 + 16 +24 = 70 |

# 📤Salida mostrada en Pseint

<img width="724" height="221" alt="image" src="https://github.com/user-attachments/assets/aacac1d4-a758-4c5a-becb-47461ce56529" />

# 🧮Diagrama de Flujo

<img width="492" height="1021" alt="image" src="https://github.com/user-attachments/assets/bb9597e5-e686-44b9-bfe9-e3980fdd9a2e" />

**🖥️ Código en C**

	#include <stdio.h>
	
	int main() {
		float costo_taxi, costo_buseta, costo_bus_regular;
		float total_taxi, total_buseta, total_bus_regular, total_viaje;

		// Datos de entrada
		printf("Ingrese el costo del pasaje en taxi ejecutivo (por persona): ");
		scanf("%f", &costo_taxi);
		printf("Ingrese el costo del pasaje en buseta turística (por persona): ");
		scanf("%f", &costo_buseta);
	
		// Proceso
		costo_bus_regular = costo_taxi * 0.80; // 20% menos
		
		total_taxi = 3 * costo_taxi;
		total_buseta = 2 * costo_buseta;
		total_bus_regular = 3 * costo_bus_regular;
		
		total_viaje = total_taxi + total_buseta + total_bus_regular;
	
		// Salida
		printf("El costo total del viaje para los 8 amigos es: $%.2f\n", 	total_viaje);
		return 0;
	}

# 🔢 Ejecucion en C
<img width="799" height="85" alt="image" src="https://github.com/user-attachments/assets/e219c648-5ea3-4404-9da4-cda4dfd54f96" />

## 💡 Breve explicación
Este código calcula el costo total de un viaje para 8 amigos. Pide al usuario el costo del taxi y la buseta, calcula el costo del bus regular (20% menos que el taxi), y suma los costos de los 3 grupos. 🚌🚕
