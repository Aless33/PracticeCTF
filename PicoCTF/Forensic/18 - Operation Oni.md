#### Descripción
Download this disk image, find the key and log into the remote machine.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory

##### Pista
Ninguna

#### Solución 
Para este reto lo que usaremos es principalmente lo que hacemos es buscar la clave privada de SSH del usuario ru, por lo que tenemos que explorar las particiones en busca de este. Entonces primero que nada lo que haremos es buscar entre los archivos la palabras ssh: `fls - o 206848 disk.img -r | grep ssh`, en donde 206848 es el id de la particion de linux en donde si lo vemos con `-o` nos mostrar las carpetas y finalmente usaremos grep para encontrar el ssh, obteniendo el id de la carpeta podemos acceder al ssh key, asi que despues de obtenerlo lo pasaremos a un archivo para usarlo despues en la terminal. Esto lo haremos de la siguiente manera, usamos este comando para copiar el contenido de la ssh: `icat disk.img  -o 206848 2345 > key_file` en donde 2345 es el id de el archivo, y la flecha y el key_file es el nombre del archivo y la direccion en donde la queremos mandar. Despues de obtener el àrchivo accedemos a la maquina y solamente tenemos que poner el comando para entrar y el documento en donde se encuentra el ssh, en este caso key_file: `ssh -i key_file -p 58955 ctf-player@saturn.picoctf.net`, si esta correcto nos metera en el sistema y podremos hacer ls para obtener la flag.
```
picoCTF{k3y_5l3u7h_339601ed}
```

