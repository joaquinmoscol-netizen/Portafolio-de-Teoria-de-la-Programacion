# 📘 Unidad 2: Estructuras Algorítmicas de Control
> 📚 *Comprender los principios de las estructuras condicionales y repetitivas en C, desarrollando el pensamiento lógico necesario para controlar el flujo de los programas y resolver problemas mediante algoritmos*

---

## 🎯Objetivos de la unidad 
### 🎯Estructuras Algorítmicas Condicionales

- ✅ Condicional simple: Si … Entonces (if)
- 🔀 Condicional doble: Si … Entonces, Sino … (if-esle)
- 📂 Condicional múltiple: En caso de … (swich/case)
- 🧩 Anidamiento de condicionales

### 🎯Estructuras Algorítmicas Repetitivas

- 🔁 Para (for)
- 🔄 Mientras (while)
- ⏳ Hacer … Mientras (do-while)
- 🧩 Anidamiento de bucles

## 🧩 **Temas Principales**

- ### ✅ Condicional simple: Si … Entonces (if)

   > 📝 *El if es una estructura condicional simple.*
   
   > 🧾 *Es la forma más básica de tomar decisiones dentro de un programa: solo ejecuta un bloque de instrucciones si la condición se cumple.*
   
   > ✅ *Funciona como un guardia lógico:
     si la condición es verdadera, deja pasar el código;
     si es falsa, simplemente no hace nada.*


   > 💡*La condicional simple if en C permite ejecutar un bloque de código solo si se cumple una condición.*

      Estructura básica:
      if (condición) {
      // instrucciones a ejecutar si la condición es verdadera
      }

  
  ### ✅ Características:

   > 🗂️ *La condición se evalúa como verdadera (true) o falsa (false).*
   
   > 📎 *Si la condición es falsa, no se ejecuta nada.*
   
   > 📌 *Se usa cuando se necesita tomar una decisión única en el programa.*

  ### 🧠 Diagrama de Flujo

  <img width="507" height="333" alt="image" src="https://github.com/user-attachments/assets/5f21832d-493c-4584-b81d-bde5611f2791" />

  ### 📌 Codgio en C

  <img width="459" height="257" alt="image" src="https://github.com/user-attachments/assets/b8770256-fcdc-474e-a577-440fc2b44a06" />

---

- ### 🔀 Condicional doble: Si … Entonces, Sino … (if-esle)

   > 🏗️*El if-esle corresponde a una estructura condicional doble.*

   > 📖*En programación, la condicional doble es la que evalúa una condición y ejecuta un bloque si es verdadera, y otro bloque alternativo si es falsa.*
   
   > 🔀 *En C, esa estructura es if–else.*
   
   > 📖 *En palabras simples:
   si se cumple, hace algo;
   si no se cumple, hace otra cosa*
   
   >💡*La condicional doble if–else en C permite ejecutar un bloque de código si la condición se cumple y otro bloque alternativo si la condición es falsa.*

        Estructura básica:
        if (condición) {
           // instrucciones si la condición es verdadera
        } else {
        // instrucciones si la condición es falsa
        }

   ### ✅ Características:

   > 🔀 *Evalúa la condición como verdadera (true) o falsa (false).*

   > 🏗️ *Siempre ejecuta uno de los dos bloques, nunca ambos.*

   > 📖 *Se utiliza cuando el programa debe elegir entre dos acciones posibles.*


   ### 🧠 Diagrama de Flujo

   <img width="507" height="333" alt="image" src="https://github.com/user-attachments/assets/5e10ff84-1d2d-45f0-adb7-92e626bf9cf7" />

   ### 📌Codigo en C
  
  <img width="459" height="257" alt="image" src="https://github.com/user-attachments/assets/3dbdfef7-f098-40d3-854c-c6c1f8df31a8" />

  ---
  
- ### 📂 Condicional múltiple: En caso de … (swich/case)

   > ✅ *Swich/Case corresponde a una estructura condicional múltiple.*
      
   > ☑️ *Es el tipo de estructura que se usa cuando hay varias opciones posibles y el programa debe elegir una según el valor de una variable.*

   > 💡*La condicional múltiple switch–case en C permite seleccionar una acción entre varias opciones posibles según el valor de una variable.*
   
        Estructura básica:
        switch (variable) {
            case valor1:
                // instrucciones cuando variable == valor1
                break;
            case valor2:
                // instrucciones cuando variable == valor2
                break;
            ...
            default:
                // instrucciones si ningún caso coincide
        }

   ### ✅ Características:
   
   > 🔀 *Permite manejar varias alternativas sin usar múltiples if–else encadenados.*
   
   > 🏗️ *Evalúa una sola variable y compara su valor con diferentes casos.*
   
   > 🗂️ *Cada caso representa una opción específica y el break evita que el flujo siga a los demás casos.*
   
   > 📎 *El bloque default se ejecuta si no coincide ningún caso, funcionando como una opción por defecto.*

   ### 🧠 Diagrama de Flujo

   <img width="507" height="333" alt="image" src="https://github.com/user-attachments/assets/72b6c1e4-2967-4ecd-98d0-6da717c55a3c" />

   ### 📌Codigo en C
  
   <img width="650" height="450" alt="image" src="https://github.com/user-attachments/assets/666b7757-1c51-4e70-9aab-5b6caacc19f3" />

---
- ### 🧩 Anidamiento de condicionales

   >📝 *El anidamiento de condicionales ocurre cuando colocamos un if dentro de otro if, o cuando un else contiene otro if.*

   > 🧾 *Sirve para tomar decisiones más complejas, donde cada resultado abre la puerta a nuevas verificaciones. Es una estructura de decisiones en niveles, como       un árbol lógico.*

   >✅ *Funciona como una cadena de filtros:
   si la primera condición es verdadera, se evalúa la siguiente;
   si no es verdadera, el else puede contener otro if que establezca un camino alternativo.*

   >💡*El anidamiento permite manejar múltiples escenarios de forma ordenada, usando if dentro de if, y también else que contienen más condicionales.*

      Estructura básica:
      
      if (condición1) {
          if (condición2) {
              // instrucciones si ambas condiciones son verdaderas
          }
      } else {
          if (condición3) {
              // instrucciones si condición1 es falsa pero condición3 es verdadera
          }
      }

   ### ✅ Características:

   >🗂️ Permite evaluar decisiones en cadena, verificando condiciones más específicas según el resultado anterior.

   >📎 El else también puede contener otro if, creando rutas alternativas de evaluación.

   >📌 Se usa cuando el programa necesita explorar varios escenarios posibles dependiendo de múltiples condiciones


   ### 🧠 Diagrama de Flujo

   <img width="507" height="333" alt="image" src="https://github.com/user-attachments/assets/7ea19bc2-7a64-40ec-a29c-1c8f3aa36208" />

   ### 📌Codigo en C

   <img width="459" height="257" alt="image" src="https://github.com/user-attachments/assets/a9e477b8-9454-4ac5-af6a-121a76493f37" />

---
---
---

- ### 🔁 Para (for)

   >📝 *El ciclo for es una estructura repetitiva controlada.*
   
   >🧾 Sirve para ejecutar un bloque de instrucciones un número conocido de veces, avanzando paso a paso según un contador.*
   
   >🔁 *Funciona como un bucle con tres elementos integrados: inicialización, condición y actualización.
   Mientras la condición siga siendo verdadera, el ciclo continúa repitiéndose.*
   
   >💡*El ciclo for en C se utiliza cuando conoces de antemano cuántas veces debe repetirse una acción.*

        Estructura básica:
        for (inicialización; condición; actualización) {
            // instrucciones a ejecutar en cada repetición
        }

   ### ✅ Características:

   > 🗂️ *La inicialización define el valor inicial del contador.*
   
   > 📎 *La condición determina si el ciclo continúa o se detiene.*
   
   > 🔧 *La actualización modifica el contador en cada vuelta (normalmente aumento o disminución).*
   
   > 🚀 *Es ideal para recorrer rangos numéricos, ejecutar procesos por pasos o manejar iteraciones precisas dentro de un programa.*

   ### 🧠 Diagrama de Flujo

   <img width="450" height="275" alt="image" src="https://github.com/user-attachments/assets/5f890c23-2f1b-4573-ad6b-ceec8154845a" />

   ### 📌Codigo en C
  
   <img width="459" height="257" alt="image" src="https://github.com/user-attachments/assets/758fcb0b-fdd2-4019-bc00-25013066d46c" />

---

- ### 🔄 Mientras (while)

   >📝 *El ciclo while es una estructura repetitiva condicional.*
   
   >🧾 *Se utiliza cuando no sabes cuántas veces se repetirá el proceso; la repetición depende de que la condición siga siendo verdadera.*
   
   >🔄 *Funciona como un vigilante lógico:
   mientras la condición sea verdadera, el ciclo continúa;
   cuando se vuelve falsa, el ciclo termina.*
   
   >💡*El ciclo while en C permite ejecutar un bloque de código mientras una condición se mantenga verdadera.*

        Estructura básica:
        while (condición) {
            // instrucciones que se repiten mientras la condición sea verdadera
        }

   ### ✅ Características:

   >🗂️ *Evalúa la condición antes de ejecutar el bloque, por eso se le conoce como ciclo de prueba previa.*
   
   >🔎 *Si la condición empieza siendo falsa, el ciclo nunca se ejecuta.*
   
   >🔧 *Ideal cuando la cantidad de repeticiones depende de un evento externo, del usuario o de un resultado lógico que cambia dentro del ciclo.*
   
   >⚠️ *Requiere actualizar la condición dentro del bloque para evitar ciclos infinitos.*

   ### 🧠 Diagrama de Flujo

   <img width="450" height="333" alt="image" src="https://github.com/user-attachments/assets/273da72d-cbfb-4655-af50-e6452779fc0d" />

   ### 📌Codigo en C

   <img width="459" height="257" alt="image" src="https://github.com/user-attachments/assets/f8d9a1b5-a460-4269-bd7b-8275bcd8c92e" />

---

- ### ⏳ Hacer … Mientras (do-while)
  
   >📝 *El ciclo do…while es una estructura repetitiva de prueba posterior.*
   
   >🧾 *A diferencia del while tradicional, este garantiza que el bloque de instrucciones se ejecute al menos una vez antes de verificar la condición.*
   
   >⏳ *Funciona como un bucle que primero actúa y después pregunta:
   ejecuta el código, luego revisa si debe repetirlo.*
   
   >💡*El ciclo do…while en C se usa cuando necesitas que una acción se realice mínimo una vez, sin importar la condición inicial.*

        Estructura básica:
        do {
            // instrucciones que se ejecutan al menos una vez
        } while (condición);

   ### ✅ Características:

   >🗂️ *Evalúa la condición después de ejecutar el bloque, por eso siempre corre al menos una vez.*
   
   >🔁 *Ideal cuando debes asegurar una primera ejecución, como menús interactivos, lecturas de usuario o procesos que requieren validación posterior.*
   
   >🔄 *Continúa repitiéndose mientras la condición sea verdadera.*
   
   >⚠️ *Como cualquier repetitiva, requiere actualizar la condición dentro del bloque para evitar ciclos infinitos.*

   ### 🧠 Diagrama de Flujo

  <img width="507" height="333" alt="image" src="https://github.com/user-attachments/assets/a1888f28-d5e8-4426-b9f2-d8f09ad6c2bd" />

   ### 📌Codigo en C

   <img width="459" height="257" alt="image" src="https://github.com/user-attachments/assets/75d07c38-9296-4111-81de-91000030f44c" />


---

- ### 🧩 Anidamiento de bucles

   >📝 *El anidamiento de bucles consiste en colocar un ciclo dentro de otro ciclo.*
   
   >🧾 *Permite ejecutar procesos repetitivos en varias dimensiones, donde cada vuelta del ciclo externo contiene múltiples repeticiones del ciclo interno.*
   
   >🧩 *Funciona como un engranaje doble:
   el bucle externo avanza paso a paso,
   y en cada paso el bucle interno realiza todas sus iteraciones.*
   
   >💡*El anidamiento de bucles en C se utiliza cuando necesitas recorrer estructuras más complejas, como matrices, tablas, patrones o múltiples niveles de repetición.*

        Estructura básica:
        for (condición externa) {
            for (condición interna) {
                // instrucciones del ciclo interno
            }
        }

   ### ✅ Características:

   >🗂️ *El ciclo interno se ejecuta completamente en cada iteración del ciclo externo.*
   
   >🔄 *Se puede anidar cualquier combinación: for dentro de for, while dentro de while, for dentro de while, etc.*
   
   >🔧 *Ideal para trabajar con arreglos bidimensionales, generar patrones numéricos o repetir procesos dependientes entre sí.*
   
   >⚠️ *Se debe controlar cuidadosamente la condición de ambos ciclos para evitar tiempos de ejecución excesivos.*

   ### 🧠 Diagrama de Flujo

   <img width="507" height="333" alt="image" src="https://github.com/user-attachments/assets/6f4f272d-0c5b-41ca-813c-04b1b7841378" />

   ### 📌Codigo en C

   <img width="459" height="257" alt="image" src="https://github.com/user-attachments/assets/b6680ee2-abb5-497c-8180-de315736db38" />

---
---
---

   ## 🧩 Ejercicico en Java 

   > 📌Realicé una calculadora básica en Java 🧮 capaz de ejecutar las cuatro operaciones fundamentales: suma ➕, resta ➖, multiplicación ✖️ y división      ➗. El programa utiliza estructuras de control anidadas 🔁 para gestionar tanto la selección de la operación como la validación de los datos ingresados     por el usuario ✔️. Además, incorpora un sistema de verificación 🚫 que evita errores comunes, como intentar dividir entre cero, solicitando                 nuevamente los valores cuando sea necesario 🔍.El propósito de esta calculadora es demostrar el uso práctico de bucles, condicionales y manejo de            entradas en Java 💻, permitiendo al usuario realizar varias operaciones dentro del mismo flujo del programa 🌀 de manera segura y controlada.

  ### 🧠 Diagrama de Flujo

   <img width="539" height="920" alt="image" src="https://github.com/user-attachments/assets/78ff08fd-a67b-4560-8530-37818734640d" />

   ### 📌 Codigo en Java 

   <img width="550" height="350" alt="image" src="https://github.com/user-attachments/assets/f3c0e141-c027-4b12-b620-afad8f082658" />


   <img width="550" height="350" alt="image" src="https://github.com/user-attachments/assets/9731dc1e-1a72-4305-8f71-a84e0f41d43f" />


   <img width="450" height="333" alt="image" src="https://github.com/user-attachments/assets/68db6955-24aa-46ac-b1b4-b0cef6532f22" />


   ### ⚠️ Verificación 

   <img width="539" height="450" alt="image" src="https://github.com/user-attachments/assets/1865aeac-769a-460c-b36a-3c79a6d5d80f" />

---

## ⚠️ Principales Dificcultades 
   > ✔️*Mi mayor dificultad surge cuando trato de decidir cual de los operadores lógicos ||, && y ! uso, especialmente durante un período de tiempo. También       tengo un trabajo difícil porque no siempre sé en qué situaciones necesito usarlo o cómo aplicarlo correctamente. Tambien suele suceder con las               estructuras if donde a veces me confundo y no puedo interpretar la condición correctamente. Además, suelo tener problemas para romper los bucles, lo         que demuestra que todavía necesito fortalecer mi gestión de relaciones y mi lógica en general.*
---
## 🌀 Reflexión crítica

   > 🗂️ *El manejo de condicionales y bucles sigue siendo uno de los desafíos más importantes en mi proceso de aprendizaje. Las dificultades que encuentro,          como no saber cuándo usar operadores lógicos, confundir el comportamiento de estructuras como if, while o do, o crear bucles infinitos, muestran que         todavía necesito fortalecer mi pensamiento lógico. Estos errores no sólo afectan la correcta ejecución de los programas, sino que también muestran la        importancia de comprender la lógica de cada decisión y cada repeticion. Reconozco que aprender estas estructuras es esencial para progresar en la            programación, por lo que necesito continuar practicando, analizando casos y desarrollando la capacidad de elegir cuidadosamente la estructura adecuada       para cada problema. Así, cada error se convierte en un paso necesario para crear una lógica más estable y confiable.*


---

## ⚙️ACD - Aprendizaje Contacto con el Docente

- ACD Control de aprendizaje de programas utilizando estructuras condicionales.

   -🔗 [ACD →](Aprendizaje.md)

## 🧰 APE - Aprendizaje Práctico Experimental

- APE1. Aplicación de estructuras condicionales en la resolución de problemas
   - 🗂️ [APE 1.](APE1RicardoOchoa.pdf)
- APE2. Aplicación de estructuras repetitivas en la resolución de problemas
   - 🗂️ [APE 2.](APE2RicardoOchoa.pdf)


## 🧰 AA - Aprendizaje Autónomo 
- AA 1. Diferencias entre los tipos de estructuras condicionales
   - 🗂️ [Tarea 1](Tarea1RicardoMathiasOchoaArmijos.pdf)
- AA 2. Cuadro comparativo entre las estructuras repetitivas
   - 🗂️ [Tarea 2](Tarea2RicardoOchoa.pdf)

[Portafolio](portafolio.md)
