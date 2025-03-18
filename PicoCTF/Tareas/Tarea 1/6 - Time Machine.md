#### Descripción

What was I last working on? I remember writing a note to help me remember...

###### Pistas
- The `cat` command will let you read a file, but that won't help you here!
- Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control).
- When committing a file with git, a message can (and should) be included.

#### Solución 
Para este reto lo que tenemos que hacer es realizar una busqueda usando el git log, para ver las versiones del mensaje, con eso vemos que ahi esta la flag en el comentario,
```
RepugnamShip33-picoctf@webshell:~$ cd drop-in
RepugnamShip33-picoctf@webshell:~/drop-in$ ls
message.txt
RepugnamShip33-picoctf@webshell:~/drop-in$ cat message.txt
This is what I was working on, but I'd need to look at my commit history to know why...RepugnamShip33-picoctf@webshell:~/drop-in$   
RepugnamShip33-picoctf@webshell:~/drop-in$ git log message.txt
picoCTF{t1m3m@ch1n3_d3161c0f}
```

#### Notas Adicionales

#### Referencias
