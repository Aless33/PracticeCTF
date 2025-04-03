#### Descripción
This is a really weird text file [TXT](https://jupiter.challenges.picoctf.org/static/e7e5d188621ee705ceeb0452525412ef/flag.txt)? Can you find the flag?
##### Pista
How do operating systems know what kind of file it is? (It's not just the ending!

Make sure to submit the flag as picoCTF{XXXXX}

#### Solución 
En esta solucion recibimos un archivo .txt que al descargar vemos que en vez de contener texto tiene formato y forma de imagen, por lo cual sabemos que este no es el formato original, por lo que ahora lo que hacemos es cambiando usando: `mv` hacemos el cambio de formato y lo pasamos a imagen y abriendo nuevamente nos encontramos con la bandera.
```
picoCTF{now_you_know_about_extensions}
```



#### Notas Adicionales

#### Referencias
