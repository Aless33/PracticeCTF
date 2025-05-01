#### Descripción
We found this [packet capture](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/capture.pcap) and [key](https://jupiter.challenges.picoctf.org/static/0c84d3636dd088d9fe4efd5d0d869a06/picopico.key). Recover the flag.

##### Pista
- Try using a tool like Wireshark.
- How can you decrypt the TLS stream?

#### Solución 
Para esta solucion usaremos wireshark, en donde podemos ver varias http de paquetes que hay, para eso usaremos la key que nos proporcionaron, con esta podemos realizar la busqueda de la flag, asi que nos tenemos que ir a preferencias del sistema wireshark en el apartado de editar, ahi buscaremos todas las TLS e introduciremos la key proporcionada, con esto hecho podemos desencriptar los paquetes relacionados y solo tenemos que buscar la flag usando el filtro de wireshark, accediendo asi a su flag
```
picoCTF{nongshim.shrimp.crackers}
```

