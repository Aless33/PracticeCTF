#### Descripción
Don't power users get tired of making spelling mistakes in the shell? Not anymore! Enter Special, the Spell Checked Interface for Affecting Linux. Now, every word is properly spelled and capitalized... automatically and behind-the-scenes! Be the first to test Special in beta, and feel free to tell us all about how Special streamlines every development process that you face. When your co-workers see your amazing shell interface, just tell them: That's Special (TM)Start your instance to see connection details.

Additional details will be available after launching your challenge instance.

###### Pistas
- Experiment with different shell syntax

#### Solución 

- La shell "Special" convierte la primera letra de cada palabra en mayúscula, lo que rompe la ejecución de comandos (`ls → Is`, `clear → Clear`).
- Los operadores `;` y `&` permiten ejecutar comandos en secuencia, permitiendo que algunos comandos funcionen correctamente incluso si otros fallan.
- **El comando `find` fue clave** para encontrar `flag.txt`, ya que `find` no se vio afectado por la capitalización automática.
- Finalmente, `cat` permitió leer el contenido de la flag.
El reto se basa en entender cómo la shell "Special" modifica los comandos y encontrar una forma de ejecutar los correctos. Utilizando `find` para localizar archivos y `cat` para leer la flag.
```
Special$ ls
Is 
sh: 1: Is: not found
Special$ clear
Clear 
sh: 1: Clear: not found
Special$ clear; ls
Clear is 
sh: 1: Clear: not found
Special$ clear & ls
Clear & is 
sh: 1: is: not found
sh: 1: Clear: not found
Special$ clear & find
Clear & find 
sh: 1: Clear: not found
.
./blargh
./blargh/flag.txt
./.cache
./.cache/motd.legal-displayed
Special$ clear & cat ./blargh/flag.txt            
Clear & cat ./blargh/flag.txt 
sh: 1: Clear: not found
picoCTF{5p311ch3ck_15_7h3_w0r57_6a2763f6}
```
#### Notas Adicionales
Cada que corregia se podria encontrar y probar otro tipo de comando para ver como se podria realizar

#### Referencias
https://www.ibm.com/docs/es/aix/7.2?topic=concepts-restricted-shell