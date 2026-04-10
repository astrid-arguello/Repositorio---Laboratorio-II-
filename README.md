# Repositorio---Laboratorio-II-
Laboratorio de Programación Computacional de Computo II  

Integrantes:
Astrid Marcela Arguello Guzman - SMSS029224
Karen Beatriz Jandres Chavez - SMSS013424
Yessica Raquel Reyes Juarez - SMSS042624

Apartado #4: Preguntas y Respuestas

1.	¿De qué forma manejaste el login de usuarios? Explica con tus palabras porque en tu página funciona de esa forma.
R// El login lo manejamos usando PHP y una base de datos MySQL. Cuando el usuario ingresa su usuario y contraseña, estos datos se envían a un archivo PHP que los compara con los registros guardados en la base de datos. Si coinciden, se crea una sesión para mantener al usuario dentro del sistema. Funciona de esta forma porque PHP permite validar datos y las sesiones ayudan a controlar el acceso a las páginas.

2.	¿Por qué es necesario para las aplicaciones web utilizar bases de datos en lugar de variables?
R// Es necesario usar bases de datos porque permiten guardar la información de forma permanente. Las variables solo almacenan datos temporalmente y se pierden cuando se cierra la página o se recarga. En cambio, la base de datos mantiene la información guardada, como usuarios o movimientos, aunque se cierre el sistema.

3.	¿En qué casos sería mejor utilizar bases de datos para su solución y en cuáles utilizar otro tipo de datos temporales como cookies o sesiones?
R// Las bases de datos se utilizan cuando necesitamos guardar información importante y permanente, como cuentas de usuarios o registros. En cambio, las sesiones o cookies se usan para datos temporales, como mantener al usuario logueado o guardar información mientras navega en la página. Por eso, cada uno se usa según el tipo de información que se necesita manejar.

4.	Describa brevemente sus tablas y los tipos de datos utilizados en cada campo; justifique la elección del tipo de dato para cada uno.
R// En nuestra base de datos utilizamos dos tablas:
La tabla usuarios, que contiene:
id (INT): identificador único para cada usuario
usuario (VARCHAR): para guardar el nombre del usuario
password (VARCHAR): para guardar la contraseña

La tabla movimientos, que contiene:
id (INT): identificador del movimiento
tipo (VARCHAR): para indicar si es depósito o retiro
monto (DECIMAL): para guardar cantidades de dinero con precisión
fecha (TIMESTAMP): para registrar automáticamente la fecha
usuario_id (INT): para relacionar el movimiento con el usuario

Elegimos estos tipos de datos porque permiten guardar correctamente cada tipo de información, por ejemplo, VARCHAR para texto y DECIMAL para valores monetarios.
