#### Descripción
Files can always be changed in a secret way. Can you find the flag? 
##### Pista
Look at the details of the file Make sure to submit the flag as picoCTF{XXXXX}

#### Solución 
Utilizamos el comando hexeditor  para ver y editar archivos en foramto hexadecimal.
Posiblemente ahí se encuentre la bandera, pero en formato hexadecimal

`resource='cGljb0NURnt0aGVfbTN0YWRhdGFfMXNfbW9kaWZpZWR9`

Utilizamos el cyber chef. Asi obtenemos la flag.

```
 picoCTF{the_m3tadata_1s_modified}
```


#### Notas Adicionales

#### Referencias
