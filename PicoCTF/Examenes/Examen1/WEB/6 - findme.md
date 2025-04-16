#### Descripción

Help us test the form by submiting the username as `test` and password as `test!`
###### Pistas
- any redirections?

#### Solución 
Para este reto vemos que el reto nos da un usuario y contraseña predefinidos, con una pista que dice si hay alguna redireccion, para eso usaremos burpsite para interceptar estas direcciones, como podemos ver en una nos da un codigo de 64, con esto podemos obtener la primera parte de la flag: `cGljb0NURntwcm94aWVzX2Fs` de la direccion antes de ser redireccionada, para la ultima lo que hice fue retornar de la pagina que me llevo en redireccionada y ahi estaba la otra parte de la flag: `bF90aGVfd2F5X2JlNzE2ZDhlfQ==` completando la flag y despues usando un decode64 podemos obtener la flag completa:

```
picoCTF{proxies_all_the_way_be716d8e}
```

