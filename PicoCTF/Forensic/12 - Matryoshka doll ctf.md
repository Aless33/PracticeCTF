#### Descripción
Matryoshka dolls are a set of wooden dolls of decreasing size placed one inside another. What's the final one?

##### Pista
- Wait, you can hide files inside files? But how do you find them?
- Make sure to submit the flag as picoCTF{XXXXX}

#### Solución 
Para este problema lo que tenemos que hacer es descargar la imagen de una matrioshka rusa, estas se caracterizan por tener muchas muñecas una adentro de otra, por lo que el nombre nos puede dar una pista, con esto podemos investigar la imagen, en mi caso usare `binwalk -e` para obtener el extraible de la imagen y aqui es donde nos da otra carpeta en donde accedemos que contiene una carpeta con una imagen de una matrioshka y un zip, entonces descomprimimos el zip y podemos ver que la carpeta se remplaza mostrando ahora la siguiente imagen, entonces repetimos usando `binwalk -e` accediendo mas en la imagen nuevamente y otra vez obteniendo el zip y extrayendolo, esto lo podemos realizar un total de 4 veces, en donde en la 4 iteracion nos da un archivo .txt que tiene la flag.
```
picoCTF{e3f378fe6c1ea7f6bc5ac2c3d6801c1f} 
```

