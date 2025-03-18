#### Descripción
Unzip this archive and find the flag.

PISTA: Can grep be instructed to look at every file in a directory and its subdirectories?
#### Solución 
Utilizando el comando de "wget" descargamos el archivo mediante el enlace, para que despues usando el comando de  "unzip big-zip-files" podemos ver lo que contiene mediante las lineas de la terminal, pero al ver que es mucha informacion podemos usar el comando grep que nos ayuda a buscar iterando buscando una palabra o patrón y se imprimirá la línea o líneas que la contengan entre el archivo hasta encontrar la palabra picoCTF.
```
RepugnamShip33-picoctf@webshell:~$ grep -r 
Usage: grep [OPTION]... PATTERNS [FILE]...
Try 'grep --help' for more information.
RepugnamShip33-picoctf@webshell:~$ grep -r 'picoCTF'
big-zip-files/folder_pmbymkjcya/folder_cawigcwvgv/folder_ltdayfmktr/folder_fnpfclfyee/whzxrpivpqld.txt:information on the record will last a billion years. Genes and brains and books encode picoCTF{gr3p_15_m4g1c_ef8790dc}
```

#### Notas Adicionales

Es importante primero verificar si se puede iterar o no.
El comando grip puede identificar todo tipo de busquedas.
#### Referencias

https://webshell.picoctf.org/
https://www.hostinger.com/mx/tutoriales/comando-grep-linux