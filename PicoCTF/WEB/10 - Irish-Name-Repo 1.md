#### Descripción

Do you think you can log us in? Try to see if you can login!

##### Pista

There doesn't seem to be many ways to interact with this. I wonder if the users are kept in a database?

Check out tools like Burpsuite to modify your requests and look at the responses
#### Solución 
Para esta solucion vemos que es una pagina que tiene un formulario de usuario, las pistas nos dicen que esta conectada a la base de datos, para eso lo que vamos a hacer es usar los parametros de SQL para poder darnos siempre True, haciendo que aunque no se el usuario esperado podamos entrar debido a la validacion del SQL.
En esta ocacion solo use el admin' --, lo que hicimos comentar todo el sql, dandonos acceso debido a la validacion aceptada.
```
Your flag is: picoCTF{s0m3_SQL_fb3fe2ad}
```


#### Notas Adicionales

#### Referencias
