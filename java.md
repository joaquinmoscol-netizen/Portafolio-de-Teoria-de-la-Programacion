# 🛠️ ¿Qué es Java?

Java se define como un lenguaje de programación **orientado a objetos, de alto nivel y multiplataforma**. Su gran popularidad se debe a su filosofía **"Write Once, Run Anywhere"** (Escríbelo una vez, ejecútalo donde sea).

Esto es posible gracias a su arquitectura interna, compuesta por tres pilares:
1. 🧠 **El Lenguaje:** La sintaxis que escribimos.
2. ⚙️ **La JVM (Máquina Virtual de Java):** El motor que permite ejecutar el programa en Windows, Linux o Mac sin necesidad de modificar el código.
3. 📚 **La API:** Un conjunto robusto de librerías estándar listas para usar.


Se usa ampliamente en:  
- 🏢 Aplicaciones empresariales  
- 📱 Android  
- 🌐 Aplicaciones web  


---

# 🛠️ ¿Cómo compilar y ejecutar un programa Java?

Para trabajar con Java necesitas instalar el **JDK (Java Development Kit)**.

---

## 1️⃣ Crear el archivo `.java`

Crea un archivo llamado igual que la clase pública:

```java
// HolaMundo.java
public class HolaMundo {
    public static void main(String[] args) {
        System.out.println("¡Hola, Mundo!");
    }
}
```
## 2️⃣ Compilar el programa
En la terminal, ejecuta:

javac HolaMundo.java

Esto generará:

HolaMundo.class

## 3️⃣ Ejecutar el programa

java HolaMundo

🔎 No incluyas la extensión .class al ejecutar.

# 🧬 ¿Qué sucede internamente?

javac convierte el archivo .java en bytecode .class.

La JVM interpreta o JIT-compila ese bytecode a código máquina.

Gracias a la JVM, el mismo programa funciona en Windows, Linux o macOS.



# 📌 Ejercicio: Suma de 5 números positivos con validación

Solicitar al usuario que ingrese **5 números positivos**.  
Si el número ingresado es negativo o cero, se vuelve a pedir.  
Al final, mostrar la suma total y el promedio de los números ingresados.

---

### 📝 Análisis del problema

#### 📥 Datos de entrada
- 5 números enteros positivos ingresados por el usuario.

#### ⚙️ Proceso

1. Usar un **bucle `for`** para repetir 5 veces:  
   - Dentro del `for`, usar un **`do...while`** para validar que el número sea positivo.  
   - Sumar el número ingresado a `suma`.  
2. Calcular el promedio (`suma / 5.0`).  

#### 📤 Salida
- Suma total de los números ingresados.  
- Promedio de los números ingresados.

---


### 🧪 Pruebas de escritorio

| Iteración | Número ingresado | Condición `numero <= 0` | Acción/Salida                  |
|-----------|-----------------|------------------------|--------------------------------|
| 1         | 4               | Falso ❌               | Se suma a `suma` (suma = 4)   |
| 2         | 8               | Falso ❌               | Se suma a `suma` (suma = 12)  |
| 3         | 3               | Falso ❌               | Se suma a `suma` (suma = 15)  |
| 4         | 9               | Falso ❌               | Se suma a `suma` (suma = 24)  |
| 5         | 10              | Falso ❌               | Se suma a `suma` (suma = 34)  |
| Final     |                 |                        | Suma total: 34, Promedio: 6.8 |


---

### 🧩 Diagrama de flujo

<img width="300" height="1029" alt="image" src="https://github.com/user-attachments/assets/2a5602c8-7e98-408d-b089-76c5872e9105" />


---

### 💻 Código en Java

```java
import java.util.Scanner;

public class ejercicioporta {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int numero;
        int suma = 0;

        // Bucle for: repetir 5 veces
        for (int i = 1; i <= 5; i++) {
            // Validación: do-while
            do {
                System.out.print("Ingrese un número positivo (" + i + "/5): ");
                numero = sc.nextInt();
            } while (numero <= 0);

            suma += numero;
        }

        double promedio = suma / 5.0;

        System.out.println("Suma total: " + suma);
        System.out.println("Promedio: " + promedio);
        
        sc.close();
    }
}

```
## Evidencia

<img width="500" height="396" alt="image" src="https://github.com/user-attachments/assets/bd30d9cb-2b54-4481-821f-38f322b92ce7" />

---
[Volver a la unidad 2](Unidad2.md)

[Volver al inicio](Inicio.md)
