#### Descripción
Can you invoke help flags for a tool or binary?
#### Solución 
Para el resolver este problema vamos a tener que usar el comando wget para obtenerlo en la terminal, despues de eso debemos darle permisos usando `chmod +x warm` con esto le damos permiso de ejecucion en nuestro sistema, dando asi y que podamos usarlo usando: ./warm para ejecutar y nos muestre el mensaje en donde lo ejecutamos con -h para que nos de la flag
```
RepugnamShip33-picoctf@webshell:~$ wget https://mercury.picoctf.net/static/a14be2648c73e3cda5fc8490a2f476af/warm
--2025-03-17 23:54:21--  https://mercury.picoctf.net/static/a14be2648c73e3cda5fc8490a2f476af/warm
Resolving mercury.picoctf.net (mercury.picoctf.net)... 18.189.209.142
Connecting to mercury.picoctf.net (mercury.picoctf.net)|18.189.209.142|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 10936 (11K) [application/octet-stream]
Saving to: 'warm'

warm                                            100%[======================================================================================================>]  10.68K  --.-KB/s    in 0s      

2025-03-17 23:54:21 (292 MB/s) - 'warm' saved [10936/10936]

RepugnamShip33-picoctf@webshell:~$ /warm 
-bash: /warm: No such file or directory
RepugnamShip33-picoctf@webshell:~$ bshell:~$ /warmchmod +x warm
-bash: bshell:~$: command not found
RepugnamShip33-picoctf@webshell:~$ chmod +x warm
RepugnamShip33-picoctf@webshell:~$ ./warm
Hello user! Pass me a -h to learn what I can do!
RepugnamShip33-picoctf@webshell:~$ ./warm -h
Oh, help? I actually don't do much, but I do have this flag here: picoCTF{b1scu1ts_4nd_gr4vy_755f3544}
RepugnamShip33-picoctf@webshell:~$ 
```

#### Notas Adicionales


#### Referencias
