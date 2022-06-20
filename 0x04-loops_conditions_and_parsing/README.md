SHELLCHECK
----------
Shellcheck, from what I understand is a tool similar to Betty, but in scripts. It will help us to write them properly, besides making recommendations on the syntax and semantics, it will advise us on border cases that we had not thought about. All your Bash scripts must pass Shellcheck without any error to be able to generate points when uploading the exercises of this project.

Installation: https://github.com/koalaman/shellcheck#installing or directly ' sudo apt install shellcheck ' (windows)

GENERATE RSA KEYS 
--------------------
WHAT IS THIS FOR?
------------------
To secure SSH access to your cloud server, the most effective way is to use private and public keys. The public key will be on the server, and the private key will be where we will work locally. The use of these keys makes it impossible for someone to log in using a single password, as long as you configure SSH to deny password-based authentication.

HOW ARE THEY GENERATED?
----------------------
They can be generated directly in the terminal or in the PuTTYgen application.

PUTTYGEN
--------
It is quite simple to create keys with PuTTYGen, this process consists of 4 simple steps.

1- If necessary, download PuTTYgen.

2- Start the program and then click on the Generate button.

3- Enter a passphrase, for added security.

4- Save the public and private keys by clicking on the Save public key and Save private key buttons.

From the Public key field to paste into the OpenSSH authorized keys file at the top of the window, copy all the text (starting with ssh-rsa).

TERMINAL (I RECOMMEND IT)
---------
To generate keys in the terminal simply follow these steps:

1- Type "ssh-keygen -t rsa".

2- Tell it in which file we want to save the keys (the private one will be saved in the one we tell it, for the private one a new file will be created which is an extension of the previous one.

3- Write a phrase (optional).

This is the way that I recommend because it already brings you incorporated in the public key the ssh-rsa and at the end it puts you the user.

-------------------------------------------------------------------------------------------------------------

Using loops in bash
--------------------

do:
----
is the keyword that starts the loops. It will execute the instruction n times, where n is the total number of elements.

done:
-----
stops the loop

The double parenthesis of the loops can be straight parenthesis, I recommend this when using "if", because when we are going to use these, the condition of the cycle will be different, instead of putting "<" in this case it will be "-le".

for :
-----
We have the letter "a" as our iterator, we use the for as a loop to tell it first when we want our variable to start iterating, then the condition and finally to go forward. This is the same as with C, but the difference is that it goes with double parenthesis and without semicolon at the end.

while :
-------
We have the letter "a" as our iterator, first we declare it giving its starting point. Then, as with for we give it the condition using double parenthesis, and finally inside "do" and after telling it what we want it to do if the condition is fulfilled, we tell it to go ahead. An interesting fact about this loop is that when declaring the variable and giving it a value, you don't have to leave spaces around "=". We discovered this thanks to shellcheck.

until :
-------
We use the letter "a" as the beginning, and the letter "b" as the end, that's why before using the loop we give those values. The until loop, is written exactly the same as the while loop, the difference is that the condition is put with the two variables created, and whatever is put inside "do", is going to be done until the condition previously put is fulfilled.

---------------------------------------------------------------
if in Bash
----------
In bash the if is put the same as in C, but what changes is that it is in straight parenthesis, then we put "Then" inside this is where we tell it what we want to do if the condition inside the if is fulfilled, and finally we put "fi" to finish the if.


--------------------------------------------------------------
---------------------------------------------------------------

SHELLCHECK
-----------
Shellcheck, por lo que entiendo es una herramienta similar a Betty, pero en scripts. Nos ayudara a escribirlos adecuadamente, ademas de hacernos recomendaciones sobre la sintaxis y la semantica, nos aconsejara sobre casos border que no habiamos pensado. Todos tus scripts Bash deben pasar Shellcheck sin ningún error para poder generar puntos a la hora de subir los ejercicios de este proyecto.

Instalacion: https://github.com/koalaman/shellcheck#installing o directamente ' sudo apt install shellcheck ' (windows)

GENERAR CLAVES RSA
--------------------
PARA QUE SIRVE ESTO?
-----------------------
Para asegurar el acceso SSH a su servidor en la nube, la manera mas efectiva es usar claves privadas y publicas. La clave publica va a estar en el servidor, y la privada en donde trabajaremos localmente. El uso de estas claves hace que sea imposible que alguien incie sesion usando una sola contrasena, siempre que configure SSH para denegar la autenticacion basada en contrasena.

COMO SE GENERAN?
----------------
Se pueden generar directamente en la terminal o en la aplicacion PuTTYgen.

PUTTYGEN
---------
Es bastante simple crear claves con PuTTYGen, este proceso consta de 4 simples pasos. 

1- Si es necesario, hay que descargar PuTTYgen.

2- Iniciiar el programa y luego hacaer click en el botón Generar.

3- Ingresar una frase de contraseña, para mayor seguridad.

4- Guardar las claves pública y privada haciendo clic en los botones Guardar clave pública y Guardar clave privada.

Desde el campo Clave pública para pegar en el archivo de claves autorizadas de OpenSSH en la parte superior de la ventana, hay que copiar todo el texto (comenzando con ssh-rsa).

TERMINAL (LO RECOMIENDO)
---------
Para generar claves en la terminal simplemente hay que seguir estos pasos:

1- Escribir "ssh-keygen -t rsa".

2- Decirle en que archivo queremos que guarde las claves (la privada se va a guardar en el que nosotros le decimos, para la pulica se va a crear un archivo nuevo que es una extension del anterior.

3- Escribir una frase (opcional).

Esta es la manera que recomiendo porque ya te trae incorporado en la clave publica el ssh-rsa y al final te pone el user.

---------------------------------------------------------------------

Usar bucles en bash
--------------------

do:
----
es la palabra clave que inicia los bucles. Ejecutará la instrucción n veces, siendo n el número total de elementos.

done:
-----
detiene el bucle

Los dobles parentesis de los loops pueden ser parentesis rectos, esto lo recomiendo a la hora de usar "if", ya que cuando vayamos a usar estos, la condicion del ciclo va a ser otra, en vez de poner "<" en este caso va a ser "-le".

for :
-----
Tenemos a la letra "a" como nuestra iteradora, usamos el for como bucle para decirle primero desde cuando queremos que nuestra variable empiece a iterar, luego la condicion y finalmente que vaya avanzando. Esto es igual que con C, pero la diferencia es que va con doble parentesis y sin punto y coma al final.

while :
-------
Tenemos a la letra "a" como nuestra iteradora, primero la declaramos dandole su punto de inicio. Luego, al igual que con for le damos la condicion usando parentesis dobles, y finalmente dentro de "do" y luego de decirle lo que queremos que haga si se cumple la condicion, le decimos que vaya avanzando. Un dato interesante de este ciclo es que al declarar la variable y darle un valor, no hay que dejar espacios alrededor de "=". Esto lo descubrimos gracias a shellcheck.

until :
-------
Utilizamos la letra "a" como el comienzo, y la letra "b" como final, por eso antes de usar el bucle le damos esos valores. El ciclo until, se escribe exactamente igual al ciclo while, la diferencia es que la condicion se pone con las dos variables creadas, y lo que se ponga dentro de "do", se va a realizar hasta que la condición puesta anteriormente se cumpla.

-------------------------------------------------

if en Bash
----------
En bash el if se pone igual que en C, pero lo que cambia es que es en parentesis rectos, luego se pone "Then" dentro de esto es donde le decimos que queremos que hacer si se cumple la condicion dentro del if, y finalmente ponemos "fi" para terminar el if.
