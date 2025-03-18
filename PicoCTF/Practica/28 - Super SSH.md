#### Descripción

Using a Secure Shell (SSH) is going to be pretty important.

Additional details will be available after launching your challenge instance.
#### Solución 

Para este problema es solamente usar el servidor y el comando de SSH para realizar y obtener la bandera, introduciendo el dominio y la direccion, asi como tambien el puerto usando `-p` con el puerto a continuacion para obtener la  key.
```
RepugnamShip33-picoctf@webshell:~$ ssh ctf-player@titan.picoctf.net -p 57760 
The authenticity of host '[titan.picoctf.net]:57760 ([3.139.174.234]:57760)' can't be established.
ED25519 key fingerprint is SHA256:4S9EbTSSRZm32I+cdM5TyzthpQryv5kudRP9PIKT7XQ.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[titan.picoctf.net]:57760' (ED25519) to the list of known hosts.
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_3e293eea}
Connection to titan.picoctf.net closed.
```
#### Notas Adicionales

#### Referencias
