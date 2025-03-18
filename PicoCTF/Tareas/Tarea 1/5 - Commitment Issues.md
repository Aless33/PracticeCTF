#### Descripción
I accidentally wrote the flag down. Good thing I deleted it!
###### Pistas
- Version control can help you recover files if you change or lose them!
- Read the chapter on Git from the picoPrimer [here](https://primer.picoctf.org/#_git_version_control)
- You can 'checkout' commits to see the files inside them
#### Solución 

Para este problema vemos que ahora es un mensaje de texto que dice TOP SECRET, y verificando los commits se ve que se creo la flag pero luego se borro, por lo cual usando `git checkout` podemos ir a esa version de el txt. Y ahi vemos la flag.
```
RepugnamShip33-picoctf@webshell:~$ cd drop-in 
RepugnamShip33-picoctf@webshell:~/drop-in$ ls
message.txt
RepugnamShip33-picoctf@webshell:~/drop-in$ cat message.txt
TOP SECRET
RepugnamShip33-picoctf@webshell:~/drop-in$ git log message.txt
RepugnamShip33-picoctf@webshell:~/drop-in$ git log message.txt
RepugnamShip33-picoctf@webshell:~/drop-in$ git checkout 87b85d7dfb839b077678611280fa023d76e017b8
Note: switching to '87b85d7dfb839b077678611280fa023d76e017b8'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 87b85d7 create flag
RepugnamShip33-picoctf@webshell:~/drop-in$ ls
message.txt
RepugnamShip33-picoctf@webshell:~/drop-in$ cat message.txt
picoCTF{s@n1t1z3_ea83ff2a}
```
#### Notas Adicionales

#### Referencias
