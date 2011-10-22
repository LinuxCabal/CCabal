Bibliotecas
===========
Las bibliotecas contienen funciones para facilitar la programación.

Normalmente, una biblioteca viene como un paquete con un nombre que contiene "-devel". Una vez instladas, podemos incluirlas en nuestros programas.

Para incluir una librería, es necesario usar la orden #include; seguida por el nombre del archivo header. Por ejemplo:

    #include <stdio.h>


Funciones
=========
Es un lenguaje de funciones.

Las funciones son estructuras sencillas del lenguaje. El formato es el siguiente:

    int main(void)
    {
        printf( "Hola, mundo!\n" );
        return 0;
    }

int es lo que regresa la función. En éste caso, main debe regresar un entero.

main es el nombre de la función que corre automáticamente cuando corres un programa hecho en C. Es la función global.

Lo que está entre las llaves es el contenido de la función. En otras palabras, son las órdenes que se van a correr. 


Manuales
========
Los manuales de las librerías se encuentran en la sección 3 del manual. Ejemplo:

    man 3 printf


Compilación
===========
Normalmente, vamos a compilar utilizando gcc. Para compilar un programa, solo debemos pasarle el nombre del archivo.c a compilar. Por ejemplo:

    gcc archivo.c

Ésto generará un ejecutable llamado a.out. Si queremos ejecutarlo, solo usamos ./a.out. Si queremos darle nombre, usamos -o nombre. Por ejemplo:

    gcc -o mi_programa archivo.c

Ahora, para que nos advierta de todos los errores de compilación, usemos -Wall

    gcc -Wall -o mi_programa archivo.c
