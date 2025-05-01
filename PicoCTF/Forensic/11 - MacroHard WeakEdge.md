#### Descripción
I've hidden a flag in this file. Can you find it?[](https://mercury.picoctf.net/static/52da699e0f203321c7c90ab56ea912d8/Forensics is fun.pptm)
##### Pista
None

#### Solución 
Para esta solucion vemos que el archivo esta en formato pptm, que es el formato de powerpoint, en este podemos suponer que tiene macro que seria realizar un conjunto de instrucciones en el documento para poder realizar comandos en el archivo, por lo que nuestro objetivo se encuentra ahi. Con esto hecho podemos suponer que el formato ppt se puede descomprimir si le cambiamos el zip, con esto hecho podemos obtener todo del documento, y se ve que solo son archivos .xlm y .rel, lo cual no contiene nada, pero nos topamos con un archivo bin, en donde intentamos acceder usando `cat ppt/vbaProject.bin`, pero tal parece que no es aqui donde esta la llave, entonces seguimos buscando hasta encontrar la carpeta slideMasters que contiene un hidden file, con esto abirmos el archivo nuevamente con `cat hidden` mostrando un codigo que tal parece esta en base 64, con esto hecho podemos pasar a decodearlo y asi sacamos la flag.
```
picoCTF{D1d_u_kn0w_ppts_r_z1p5}
```

