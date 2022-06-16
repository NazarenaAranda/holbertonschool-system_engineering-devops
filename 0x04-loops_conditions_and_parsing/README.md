SHELLCHECK
-----------
Shellcheck, por lo que entiendo es una herramienta similar a Betty, pero en scripts. Nos ayudara a escribirlos adecuadamente, ademas de hacernos recomendaciones sobre la sintaxis y la semantica, nos aconsejara sobre casos border que no habiamos pensado. Todos tus scripts Bash deben pasar Shellcheck sin ningún error para poder generar puntos a la hora de subir los ejercicios de este proyecto.

Instalacion: https://github.com/koalaman/shellcheck#installing o directamente ' sudo apt install shellcheck ' (windows)

GENERAR CLAVES RSA CON SSH USANDO PUTTYGEN
------------------------------------------
PARA QUE SIRVE ESTO?
-----------------------
Para asegurar el acceso SSH a su servidor en la nube, la manera mas efectiva es usar claves privadas y publicas. La clave publica va a estar en el servidor, y la privada en donde trabajaremos localmente. El uso de estas claves hace que sea imposible que alguien incie sesion usando una sola contrasena, siempre que configure SSH para denegar la autenticacion basada en contrasena.

COMO SE GENERAN?
----------------

Es bastante simple crear claves con PuTTYGen, este proceso consta de 3 simples pasos. 

1- Si es necesario, hay que descargar PuTTYgen.

2- Iniciiar el programa y luego hacaer click en el botón Generar.

3- Ingresar una frase de contraseña, para mayor seguridad.

4- Guardar las claves pública y privada haciendo clic en los botones Guardar clave pública y Guardar clave privada.

Desde el campo Clave pública para pegar en el archivo de claves autorizadas de OpenSSH en la parte superior de la ventana, hay que copiar todo el texto (comenzando con ssh-rsa).

