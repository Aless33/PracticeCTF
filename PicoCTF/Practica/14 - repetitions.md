#### Descripción
Can you make sense of this file?

PISTA: Multiple decoding is always good.
#### Solución 
Para solucionar esto tenemos que usar el base64, que se trata de decodificar el archivo que descargamos, pero como se puede ver una vez que intentamos decodificar, nuevamente sale codificado, entonces siguiendo la pista, tendremos que decodificar varias veces. Hasta encontrar la flag.
```
RepugnamShip33-picoctf@webshell:~$ cat enc_flag
VmpGU1EyRXlUWGxTYmxKVVYwZFNWbGxyV21GV1JteDBUbFpPYWxKdFVsaFpWVlUxWVZaS1ZWWnVh
RmRXZWtab1dWWmtSMk5yTlZWWApiVVpUVm10d1VWZFdVa2RpYlZaWFZtNVdVZ3BpU0VKeldWUkNk
MlZXVlhoWGJYQk9VbFJXU0ZkcVRuTldaM0JZVWpGS2VWWkdaSGRXCk1sWnpWV3hhVm1KRk5XOVVW
VkpEVGxaYVdFMVhSbFZhTTBKUFdXdGtlbVF4V2tkWGJYUllDbUY2UWpSWmEyaFRWakpHZEdWRlZs
aGkKYlRrelZERldUMkpzUWxWTlJYTkxDZz09Cg==
RepugnamShip33-picoctf@webshell:~$ cat enc_flag | base64 --decode 
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlVaM0JPWWtkemQxWkdXbXRYCmF6QjRZa2hTVjJGdGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==
RepugnamShip33-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode
V1RCa2MyRnRTWGRVYkZaVFltNVNjRmRXYUU5aVJUVnhWVzFhYVdGck5UWmFSVkpQWVRGbmVWVnVR
bHBsYTBweVUxWmpNRTVHWjNsVgpXR1JyVFdwV2VsUlZVbE5oTURCNVZXMWFUZ3BOYkdzd1ZGWmtX
azB4YkhSV2FteEVXbm93T1VOblBUMEsK
RepugnamShip33-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode | base64 --decode
WTBkc2FtSXdUbFZTYm5ScFdWaE9iRTVxVW1aaWFrNTZaRVJPYTFneVVuQlpla0pyU1ZjME5GZ3lV
WGRrTWpWelRVUlNhMDB5VW1aTgpNbGswVFZkWk0xbHRWamxEWnowOUNnPT0K
RepugnamShip33-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode | base64 --decode | base64 --decode
Y0dsamIwTlVSbnRpWVhObE5qUmZiak56ZEROa1gyUnBZekJrSVc0NFgyUXdkMjVzTURSa00yUmZN
Mlk0TVdZM1ltVjlDZz09Cg==
RepugnamShip33-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode | base64 --decode | base64 --decode | base64 --decode
cGljb0NURntiYXNlNjRfbjNzdDNkX2RpYzBkIW44X2Qwd25sMDRkM2RfM2Y4MWY3YmV9Cg==
RepugnamShip33-picoctf@webshell:~$ cat enc_flag | base64 --decode | base64 --decode | base64 --decode | base64 --decode | base64 --decode | base64 --decode
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_3f81f7be}
```

#### Notas Adicionales


#### Referencias
https://ubunlog.com/base64-codificacion-decodificacion-terminal/