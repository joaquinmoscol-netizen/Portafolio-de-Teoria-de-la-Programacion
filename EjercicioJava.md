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


# 🧩 Ejercicico en Java 

## 🧮 Calculadora básica en Java 
Esta es una calculadora básica en Java capaz de ejecutar las cuatro operaciones fundamentales: suma, resta, multiplicación y división. 
El programa utiliza estructuras de control anidadas para gestionar tanto la selección de la operación como la validación de los datos ingresados por el usuario. Además, incorpora un sistema de verificación que evita errores comunes, como intentar dividir entre cero, solicitando nuevamente los valores cuando sea necesario. 
El propósito de esta calculadora es demostrar el uso práctico de bucles, condicionales y manejo de entradas en Java, permitiendo al usuario realizar varias operaciones dentro del mismo flujo del programa de manera segura y controlada.

### 🧠 Diagrama de Flujo

<img width="539" height="920" alt="image" src="https://github.com/user-attachments/assets/78ff08fd-a67b-4560-8530-37818734640d" />

### 📌 Codigo en Java 

<img width="1043" height="923" alt="image" src="https://github.com/user-attachments/assets/a7c5d55a-a35a-487a-8f97-b68169231634" />

<img width="1417" height="839" alt="image" src="https://github.com/user-attachments/assets/8b285694-169d-4da4-a482-d94763c13ef2" />

<img width="750" height="550" alt="image" src="https://github.com/user-attachments/assets/68db6955-24aa-46ac-b1b4-b0cef6532f22" />


### ⚠️ Verificación 

<img width="634" height="690" alt="image" src="https://github.com/user-attachments/assets/7a102a1f-1768-4fa1-acbf-08f188f6020d" />

[Volver a la unidad 2](Unidad2.md)

[Volver al inicio](Inicio.md)
