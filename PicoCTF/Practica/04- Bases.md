#### Descripcion
What does this `bDNhcm5fdGgzX3IwcDM1` mean? I think it has something to do with bases.

PISTA: Submit your answer in our flag format. For example, if your answer was 'hello', you would submit 'picoCTF{hello}' as the flag.
#### Solución 
```
>>> base64.b64decode('bDNhcm5fdGgzX3IwcDM1')
b'l3arn_th3_r0p35'
>>> 
KeyboardInterrupt
>>> 
```
##### Notas Adicionales
Usando base64 introducimos el formato para decodear y sacar la flag-
##### Referencias

https://webshell.picoctf.org/