#### Descripción

Can you find the flag on this website.

Additional details will be available after launching your challenge instance.
Can you find the flag on this website.
##### Pista
SQLiLite

#### Solución 
Para solución de este problema, primero nos dan un formulario de inicio de sesion, despues esto podemos usar `' or 1 = 1 ` para acceder mediante una validacion en el SQL, despues nos envia a otra pagina donde nos sale una tabla con bloque de busqueda, podemos usar una inyeccion a SQLLite `' union select 1,id,flag from more_table;` para sacar la tabla en donde esta escondida la flag.

```
picoCTF{G3tting_5QL_1nJ3c7I0N_l1k3_y0u_sh0ulD_62aa7500}
```


#### Notas Adicionales

#### Referencias
