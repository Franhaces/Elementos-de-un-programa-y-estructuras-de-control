# Elementos-de-un-programa-y-estructuras-de-control
Ejercicios Java

## Objetivos
---

-	Utilizar un IDE como Eclipse o NetBeans y depurar sus errores.
-	Reconocer y crear los elementos propios de un programa informático.
-	Reconocer y utilizar conversiones de tipos.
-	Utilizar los comentarios en el código.
-	Utilizar estructuras de control.
-	Crear algoritmos simples.


#### Actividad 1
## *Elementos de un programa*
---

##### **Identificación de los elementos de un programa informático y utilización de las estructuras de control**


1. Configura tu IDE (Eclipse o NetBeans) y crea una nueva clase de nombre  Ejercicio01 dentro de un package de nombre actividad01. Copia el siguiente código y ejecútalo. 

```
public static void main(String[] args) throws IOException {
    // Declaramos dos variables en las que almacenar valores númericos
    //las variables de tipo "int" nos permiten almacenar enteros
    int total_manzanas; 
    int total_peras;

    //guardamos valores enteros en las variables enteras
    total_manzanas=10;
    total_peras=20;

    //modificamos el contenido de las variables enteras porque el granizo las ha mermado
    total_manzanas = total_manzanas -2;
    total_peras = total_peras -10;

    //mostramos por consola el valor de las variables enteras. De forma implícita se convierte de de int a string.
    System.out.println("Quedan "+total_manzanas+" manzanas despues del granizo");
    System.out.println("Quedan "+total_peras+" sandias despues del granizo");

    //Mostramos un mensaje al usuario pidiendole que indique un numero por consola
    System.out.println("Quantas mazanas te quieres comer?");
    //Declaramos una variable compleja de nombre "br" y de tipo "BufferedReader".
    //Las variables del tipo "BufferedReader" contienen funciones para leer datos por consola
    BufferedReader br = new BufferedReader (new InputStreamReader (System.in));
    //utilizamos la función "readLine" de la variable "br" para leer un dato por consola
    //guardamos el número introducido en la variable "valor_escrito"
    String valor_escrito = br.readLine();

    /*Convertimos mediante una conversion explicita la variable "valor_escrito" a un valor entero para poder operar con él    y lo almacenamos en la variable "numero_melones_comer" */
    int numero_manzanas_comer = Integer.parseInt(valor_escrito );

    total_manzanas = total_manzanas -numero_manzanas_comer;
    System.out.println("Finalmente quedan "+total_manzanas+" manzanas");	  
}
```

2. Al código anterior (actividad01.java) añade después del último System.out.println();  un código que pida “cuantas peras se quieren comprar”, se reciba un número escrito por el usuario, se sume  al número de peras disponibles y a continuación muestre cuantas peras quedan. 

3. Ejercicio02.java: Crea una nueva clase de nombre Ejercicio02 dentro del package de nombre actividad01. 
Para cada tipo de dato simple añade dentro de la función main de Ejercicio02  un comentario indicando el tipo de dato. Además  para cada tipo de dato simple declara una variable de ese tipo, asígnale un valor y muestra un mensaje que explique las características del tipo de dato y muestre el valor de la variable. 
Ej:
```
//Tipo de dato entero de 32 bits de longitud
int variableEntera =10;
System.out.println("Variable tipo int muestra datos enteros de 32 bits. Ejemplo:"+variableEntera);
```

4.	Dentro de la clase de nombre Ejercicio02, añade un ejemplo de uso de cada uno de los operadores aritméticos,  relacionales, lógicos, unitarios y de asignación. Indicando con un comentario y con un mensaje por consola cual será el resultado de cada uno de ellos.

5.	Dentro de la clase de nombre Ejercicio02 pide al usuario un número por consola y muestra por consola el valor multiplicado por 100. Muestra también por consola un mensaje que indique una conversión implícita y una explícita que hayas realizado en éste punto.




#### Actividad 2
## *ESTRUCTURAS DE CONTROL*
---

##### **Crea los archivos .java dentro de un package de nombre actividada02**


6. Ejercicio01.java: Crea un programa que pida por consola un número hasta que se introduzca un número superior a 7. Cuando el usuario introduzca un valor superior a 7 muestra por consola los números del 0 al número introducido utilizando la estructura WHILE y luego utilizando la estructura FOR.

7. Ejercicio02.java: Crea un programa que pida dos números decimales por consola y muestre el resultado de dividir el primero por el segundo. Antes de realizar la división, comprueba que el segundo número no es un 0. Si el segundo número es un 0, vuelve a pedir un número al usuario hasta que introduzca un valor distinto a 0.

8. Actividad03.java: Crea un programa que mantenga la cantidad litros de refresco en 2 recipientes inicialmente a 0. Mediante un SWITCH, el programa debe mostrar el siguiente mensaje al usuario:
Introduzca la operación a realizar del siguiente menú de opciones:

			1- Añadir refresco al primer recipiente.
			2-Traspasar refresco del primer al segundo recipiente.
			3- Quitar refresco del segundo recipiente.
			0-Finalizar

    * a.	Si el usuario introduce un 1, el programa ha de pedir un número decimal al usuario y añadirlo al primer recipiente.
    * b.	Si el usuario introduce un 2, el programa ha de pedir un número decimal al usuario y restarlo del primer recipiente y añadirlo al segundo.
    * c.	Si el usuario introduce un 3, el programa ha de pedir un número al usuario y restarlo  del segundo recipiente.
    * d.	Si el usuario introduce un 0, se ha de mostrar un mensaje de despedida y finalizar el programa.

Cada vez que se realice la operación 1, 2, 3  se ha de mostrar por pantalla el estado de los recipientes.
Controla mediante un DO WHILE que una vez realizada la operación seleccionada  se vuelva a mostrar el menú de operaciones excepto si el usuario ha introducido un 0. 
Si se introduce un valor menor a 0, indica que se ha introducido un valor incorrecto y vuelve a mostrar el menú.
Si no queda suficiente refresco al quitar o traspasar, mostrar un mensaje de alerta y no hacer la operación.


