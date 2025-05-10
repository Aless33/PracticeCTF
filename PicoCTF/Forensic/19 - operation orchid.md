#### Descripción
Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

##### Pista


#### Solución 
Para esta soluicion, tendremos que adentrarnos en la particion de un disco, por lo que usaremos ahora es el siguiente comando. `fls -o 411648 disk.flag.img`, con ese vemos que podemos observar los archivos del disco, peor el que nos interesa el el de root, para ahi ver si esta la flag, encontramos la flag en la carpeta pero el problema es que esta encriptada, por lo que nos toca buscar en donde podria estar su llave o el comando que nos ayude a abrirlo, para eso usaremos string para buscar todo lo relacionado con la flag: `strings -t d disk.flag.img | grep -iE "flag.txt"`, viendo que ahi esta el comando que queriamos primero moveremos el archivo encriptaqdo de la flag a uno creado por nosotros usando el siguiente comando: `cat disk.flag.img -o 411648 1782 > flag.txt.enc
, después ahora usamos el comando que encontramos en donde tambien contiene la key o la contraseña para desencriptar. Por lo cual usamos el comando: ` openssl aes256 -d -salt -in flag.txt.enc -out flag.txt -k unbreakablepassword1234567; cat flag.txt`, mostrando asi la flag.
```
picoCTF{h4un71ng_p457_1d02081e} 
```

