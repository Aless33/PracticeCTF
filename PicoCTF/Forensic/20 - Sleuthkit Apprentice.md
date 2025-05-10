#### Descripción
Download this disk image and find the flag.Note: if you are using the webshell, download and extract the disk image into `/tmp` not your home directory.

##### Pista
Ninguna

#### Solución 
Para esta solucion, igualmente tenemos que partir de la particion que tenemos presente, por lo que ahora tendremos que usar un comando para usar y obtener la flag: `icat -i raw -f ext4 -o 360448 disk.flag.img 2371`
```
picoCTF{by73_5urf3r_2f22df38}
```

