#### Descripción

Find the flag being held on this server to get ahead of the competition

##### Pista

Maybe you have more than 2 choices

Check out tools like Burpsuite to modify your requests and look at the responses
#### Solución 
En esta solucion lo que tenemos que hacer es usar comando
```
RepugnamShip33-picoctf@webshell:~$ -I http://mercury.picoctf.net:28916/http://mercury.picoctf.net:28916/
-bash: -I: command not found
RepugnamShip33-picoctf@webshell:~$ -X GET http://mercury.picoctf.net:28916/
-bash: -X: command not found
RepugnamShip33-picoctf@webshell:~$ -I http://mercury.picoctf.net:28916/
-bash: -I: command not found
RepugnamShip33-picoctf@webshell:~$ http://mercury.picoctf.net:28916/
-bash: http://mercury.picoctf.net:28916/: No such file or directory
RepugnamShip33-picoctf@webshell:~$ curl -I GET http://mercury.picoctf.net:28916/
curl: (6) Could not resolve host: GET
HTTP/1.1 200 OK
flag: picoCTF{r3j3ct_th3_du4l1ty_70bc61c4}
Content-type: text/html; charset=UTF-8
```
`picoCTF{th3_c0nsp1r4cy_l1v3s_6edb3f5f}`


#### Notas Adicionales
Tambien se podia realizar haciendo una funcion aparte para descifrar por nuestra cuenta la flag.
#### Referencias
