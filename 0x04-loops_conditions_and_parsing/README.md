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


--------------------------------------------------------------

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
