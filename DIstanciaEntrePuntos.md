## 🚗 Calcular comisiones de concesionaria

**Segundo Ejercicio:** En una concesionaria de vehículos se realizaron tres ventas de vehículos de alta gama a 3 clientes. Cada vehículo cuesta 30000, 29000 y 33000 usd. El gerente desea saber cuál es porcentaje (comisión) que cada vendedor se llevaría, lo que le pagará a cada uno de ellos (considerando el 4% por cada vendedor) y lo que le pagarán en conjunto (total).

### ⚠️ Análisis del problema
* 🎯 El problema indica "cada vendedor", por lo que asumiremos que fue un vendedor distinto para cada una de las 3 ventas.
* 🎯 El porcentaje de comisión es un valor constante (4% o 0.04).
* 🎯 Aunque el problema da valores fijos (30000, 29000, 33000), un programa más útil pedirá al usuario que ingrese los 3 montos de las ventas.

**📥 Datos de entrada**
* 📝 Tres valores numéricos reales ingresados por el usuario: `venta1`, `venta2`, `venta3`.

**⚙️ Proceso**
* 🧮 Fórmula: `comision = monto_venta * 0.04`
* Calcular comisión para cada venta:
    * `comision1 = venta1 * 0.04`
    * `comision2 = venta2 * 0.04`
    * `comision3 = venta3 * 0.04`
* Calcular el total: `total_comisiones = comision1 + comision2 + comision3`

**📤 Salida**
* 🎯 El valor de la `comision1` (real).
* 🎯 El valor de la `comision2` (real).
* 🎯 El valor de la `comision3` (real).
* 🎯 El valor del `total_comisiones` (real).

**📝 Pseudocódigo (PSeInt)**
```pseint
Algoritmo CalcularComisiones
	Definir venta1, venta2, venta3 Como Real
	Definir comision1, comision2, comision3, total_comisiones Como Real
	
	// Datos de entrada
	Escribir "Ingrese el monto de la venta 1:"
	Leer venta1
	Escribir "Ingrese el monto de la venta 2:"
	Leer venta2
	Escribir "Ingrese el monto de la venta 3:"
	Leer venta3
	
	// Proceso
	comision1 <- venta1 * 0.04
	comision2 <- venta2 * 0.04
	comision3 <- venta3 * 0.04
	total_comisiones <- comision1 + comision2 + comision3
	
	// Salida
	Escribir "La comisión de la venta 1 es: $", comision1
	Escribir "La comisión de la venta 2 es: $", comision2
	Escribir "La comisión de la venta 3 es: $", comision3
	Escribir "El total a pagar en comisiones es: $", total_comisiones
FinAlgoritmo
```
