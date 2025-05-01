#### Descripción
We found this [file](https://mercury.picoctf.net/static/09a86202e72dbdb5bf4d1b5d2c6a5b86/tunn3l_v1s10n). Recover the flag.

##### Pista
- Weird that it won't display right...

#### Solución 
Para esta solucion vemos que la imagen no se puede abrir por lo que necesitamos ver la infromacion de el archivo, tal parece que esta en formato incorrecto por lo que usaremos `hexedit` para modificar el archivo por sus exadecimales, encontrandonos que aparentemente no esta bien configurado para mostrar la imagen por lo que primero que tenemos que hacer es modificar de la 4ta columna ya que en si da 53454 byte lo cual no cuadra ya que tenemos que hacer que el infoheader sea adecuado, que seria de 40 byes, por lo que lo cambiamos a 28 00 00, con esto hecho podemos abrir la imagen pero tal parece que no es suficiente para descubrir la flag, entonces en ese momento regresamos a editar el archivo, con esto hecho podemos ver que el DataOffse esta mal configurado, por lo que tenemos que hacer es modificar la segunda fila de la primera columa, los que contiene el 65 04 00 00, este lo tenemos que modificar a 32 03 00 00, ya que esto hara que los pixeles puedan actuar adecuadamente para lo que buscamos en la imagen, haciendo esto podemos obtener la flag de la imagen que muestra el archivo.
```
picoCTF{qu1t3_a_v13w_2020} 
```

