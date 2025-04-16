#### Descripción

Can you win in a convincing manner against this chess bot? He won't go easy on you!
###### Pistas
- Try understanding the code and how the websocket client is interacting with the server

#### Solución 

Para este reto se nos presenta una pagina con un pez en el que podemos jugar al ajedrez, en este vemos que tiene diferentes frases dependiendo de su posicion y ventaja en el juego, con esto hecho podemos asumir que en el codigo viene definido cuando esta realizando un movimiento fuerte o no, asi que nos ayudamos usando la consola de comandos para poder realizar la tarea, ya que vemos que en el codigo fuente se basa en dos parametros que sera `eval` y `mate` en donde se puede saber y cambiar su comentario para cuando vaya perdiendo o ganando, con esto dicho usaremos la consola para introducir lo siguiente: `SendMessege("eval -1000000000000000")` haciendo que detecte que perdio debido a la evaluacion negativa en la tabla, antes tendremos que hacer unos movimientos con el para que active la funcion pero despues de que empiece a cambiar sus comentarios se introduce el mensaje y te da la flag aceptando su derrota como el menso pez de mar que es:
```
picoCTF{c1i3nt_s1d3_w3b_s0ck3t5_50441bef}
```

