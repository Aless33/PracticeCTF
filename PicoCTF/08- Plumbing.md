#### Descripcion
Sometimes you need to handle process data outside of a file. Can you find a way to keep the output from this program and search for the flag? Connect to `jupiter.challenges.picoctf.org 14291`.

PISTA: Remember the flag format is picoCTF{XXXX}
PISTA: What's a pipe? No not that kind of pipe... This [kind](http://www.linfo.org/pipes.html)
#### Solución 
```
Again, I really don't think this is a flag
This is defintely not a flag
This is defintely not a flag
Not a flag either
Again, I really don't think this is a flag
Not a flag either
Not a flag either
^C      
RepugnamShip33-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 14291 > datos
^C
RepugnamShip33-picoctf@webshell:~$ ls
README.txt  datos
RepugnamShip33-picoctf@webshell:~$ cat datos | grep pico
picoCTF{digital_plumb3r_ea8bfec7}
```
##### Notas Adicionales
Creamos un archivo en linuk para guardar el documento y usando cat y pico podemos filtrar y usar para sacar la respuesta.
##### Referencias

https://webshell.picoctf.org/
http://www.linfo.org/pipes.html