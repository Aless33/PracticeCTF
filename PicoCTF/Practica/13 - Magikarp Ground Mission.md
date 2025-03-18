#### Descripción
Do you know how to move between directories and read files in the shell? Start the container, `ssh` to it, and then `ls` once connected to begin. Login via `ssh` as `ctf-player` with the password, `a13b7f9d`

Additional details will be available after launching your challenge instance.

Pista: Finding a cheatsheet for bash would be really helpful!

#### Solución 
Para la solucion de este reto, nos conectaremos a una maquina, en donde tenemos que explorar con sus archivos para encotrar las 3 partes de la flag, una al inicio en donde estamos en la maquina, la segunda en la raiz, y la ultima en la carpeta home de la maquina, haciendo que podamos juntar las tres partes.

```
ctf-player@pico-chall$ ls
1of3.flag.txt  instructions-to-2of3.txt
ctf-player@pico-chall$ cat 1of3.flag.txt
picoCTF{xxsh_
ctf-player@pico-chall$ cat instructions-to-2of3.txt
Next, go to the root of all things, more succinctly `/`
ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ ls
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
ctf-player@pico-chall$ cd ~
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cat 3of3.flag.txt
71be5264}
ctf-player@pico-chall$ ^C
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ ls / 
2of3.flag.txt  bin  boot  dev  etc  home  instructions-to-3of3.txt  lib  lib64  media  mnt  opt  proc  root  run  sbin  srv  sys  tmp  usr  var
ctf-player@pico-chall$ cat 2of3.flag.txt
cat: 2of3.flag.txt: No such file or directory
ctf-player@pico-chall$ ls
3of3.flag.txt  drop-in
ctf-player@pico-chall$ cd /
ctf-player@pico-chall$ cat 2of3.flag.txt
0ut_0f_\/\/4t3r_

```

picoCTF{xxsh_0ut_0f_\/\/4t3r_71be5264}
#### Notas Adicionales


#### Referencias
