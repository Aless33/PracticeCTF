#### Descripción
A group of underground hackers might be using this legit site to communicate. Use your forensic techniques to uncover their messageTry it [here](http://standard-pizzas.picoctf.net:59908/)!
##### Pista
In the country that doesn't exist, the flag persists

#### Solución 
Se ingresa al sitio.
Se busca el país que no existe.
Al hacer una búsqueda rápida, el país upanzi no existe. Por lo tanto inspeccionamos el código para buscar la ruta.
Descargamos la imágen y La herramieta `stepic` es una herramienta de estenografía para imágenes que permite ocultar y extraer imágenes dentro de bits menos significativos. Con `-d` le indica que debe decodificar un mensaje oculto, y con `-i` se especifica que la imagen de entrada es upz.png. Obteniendo la flag
```
picoCTF{fl4g_h45_fl4g4a37da4c}
```


#### Notas Adicionales

#### Referencias
