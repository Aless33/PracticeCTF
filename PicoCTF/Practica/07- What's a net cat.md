#### Descripcion
Using netcat (nc) is going to be pretty important. Can you connect to `jupiter.challenges.picoctf.org` at port `25103` to get the flag?

PISTA: nc [tutorial](https://linux.die.net/man/1/nc)
#### Solución 
```
RepugnamShip33-picoctf@webshell:~$ which nc
/usr/bin/nc
RepugnamShip33-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 25103
You're on your way to becoming the net cat master
picoCTF{nEtCat_Mast3ry_d0c64587}
```
##### Notas Adicionales
Usamos NetCat podemos sacar junto con el puerto para sacar correctamente la respuesta
##### Referencias

https://webshell.picoctf.org/