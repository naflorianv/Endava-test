i usa protocolo SSH para conectar a los remotos, es posible tener una llave sin clave, lo que permite tranferir la data sin tener que escribir el nombre de usuario y la clave cada vez. Sin embargo, esto no es posible por el protocolo HTTP - cada conexión necesita usuario y contraseña. Incluso se vuelve más complicado para sistemas con autenticación de dos pasos, donde el token que se usa para la clave es generado al azar y no puede ser reutilizado.

Afortunadamente, Git tiene un sistema de credenciales que lo ayuda con esto. Git tiene las siguientes funciones disponibles: