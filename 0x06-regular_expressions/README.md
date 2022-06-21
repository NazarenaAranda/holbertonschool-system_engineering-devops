¿Qué son las expresiones regulares y para qué son útiles?
--------------------------------------------------------
Las expresiones regulares pueden ser todo lo complicado que uno quiera, pero en realidad son muy sencillas de crear.
Es ir creando patrones donde cadenas de caracteres vayan entrando o no entrando. Y estos patrones van a ir atacando una línea o un input, siempre y cuando sea una
cadena de caracteres. Solo van a mirar una línea de un archivo a la vez. Cuando hacemos un patrón de expresiones regulares, comparamos ese patrón línea a línea, 
quedándonos con las que son iguales al patrón, y dejando las que no se parecen.Una vez que se han comparado todas las líneas con el patrón, ya se pueden operar con los datos con los que nos hemos quedado.
Hay que ser cuidadoso con las expresiones regulares, ser tan específicos y estrictos como necesitemos. Las expresiones regulares son muy útiles tanto para quedarnos conpartes de textos importantes, en el backend o en el frontend, pero es tanto o más importante lo que vamos descartando, ya que, si tenemos archivos gigantes, con mucha 
información basura, nos es muy fácil limpiarlo con las expresiones regulares. Al limpiar estos archivos estamos ahorrando de una manera impresionante espacio en los 
discos, tiempo de procesamiento, etc.Una de las ventajas de las expresiones regulares es que estan atadas a casi todos los lenguajes de programación. Todos los 
lenguajes tienen una librería o un módulo de este tipo. Con las expresiones regulares vamos a hacer selección o descarte de datos que quiero o no quiero en mi programa.
Otra de las ventajas es que, tras extraer los datos, podemos operar directamente con ellos.

Las expresiones regulares sirven en pocas palabras, para buscar.

Aplicaciones de las expresiones regulares
-----------------------------------------
Permiten filtrar texto, buscar patrones, validar formularios, etc. de forma sencilla y eficiente. filtrando con mucha velocidad enormes cantidades de texto.

Entre las aplicaciones de las expresiones regulares tenemos:
---------------------------------------------------------
buscar informacion en los archivos log de un servidor, ya que son archivos tan enormes es muy probable que los editores de texto no lo puedan abrir.
En archivos de texto plano con mas de un millon de lineas, quizas quieras traer solamente las lineas que inician con un log de un usuario que inice con la letra “a” porejemplo.

Validar patrones, por ejemplo en un formulario definir el formato de un correo electronico y evaluar el texto que escribe el usuario con ese formato para saber si es uncorreo electronico valido.

----------------------------------------------------------------------------------------------------------------------------------------------------------

Con las expresiones regulares vamos a solucionar problemas reales. Con los patrones buscamos la forma con la que ciertos datos son presentados.
Un uso también es cambiar un carácter por otro.
Primero vamos haciendo un patrón con lo que queremos buscar, para después darle la forma en la que se presentan los datos que queremos buscar.

Hay editores de texto como Visual o Atom que tienen su propia funcion de expresiones regulares, este lo encontramos ctrl + f. En este programa hay algunos atajos como:

Punto (.) Encuentra todo lo que sea un carácter.

Punto + espacio (. ) Encuentra todos los caracteres que tengan un espacio subsecuente.

**Puntos consecutivos (………….) **Resalta el número de caracteres de acuerdo al número de puntos especificados.

-------------------------------------------------------------------------------------------------------------------------
| Regex |	Qué hace  |	Descripción  |	Inverso |
| -------|----------|---------------|----------|
| .  |	Character  | Cualquier caracter, selecciona cada uno de los caracteres	|     |
| /d | Digit | Digits: (d minúscula) Encuentra todos los dígitos (número) de 0 a 9, es equivalente a poner [0-9].  |	\D |
| /w  |	Word |	All word characters, Encuentra todos los caracteres que son parte de una palabra, tanto letras (minúsculas o mayúsculas) como números, es          equivalente a poner [a-zA-Z0-9_].  |	\W  |
| /s |Space | WhiteSpaces, Encuentra todos los espacios (los saltos de línea y tabuladores también son espacios.  | \S  |
| [0-9]	| Specific Digit | Encuentra todos los dígitos de 0 a 9. |  	|
| [0-9a-zA-Z]	| Specific Word Character  | Encontrará todos los caracteres que estén del 0-9 o que sean letras mayúsculas o minúsculas | (\w)	|
|[a-zA-Z]	|	| nos encontrará solamente las letras, tanto mayúsculas como minúsculas.|	|
| \  |	Diagonal invertida	| Escapa los caracteres, permite que un carácter especial se muestre|   |
