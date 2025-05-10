#### Descripción
Download the disk image and use `mmls` on it to find the size of the Linux partition. Connect to the remote checker service to check your answer and get the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

##### Pista
Ninguna
#### Solución 
Para esta solucion lo que tenemos que hacer es primero descargar el archivo y descomprimirlo usando `gunzip` con esto podemos ver que solo es la imagen del disco, podemos analizarla con `mmls disk.img` con esto vemos el tamaño de el secto que seria de 202752, por lo cual podemos meternos a netcat con la direccion y el puerto para introducior el tamaño del sector, para asi obtener la flag.
```
picoCTF{mm15_f7w!}
```

