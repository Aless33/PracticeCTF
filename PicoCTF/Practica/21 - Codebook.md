#### Descripción

Run the Python script `code.py` in the same directory as `codebook.txt`.

PISTA: On the webshell, use `ls` to see if both files are in the directory you are in
PISTA: The `str_xor` function does not need to be reverse engineered for this challenge.
#### Solución 
Lo unico que hay que hacer es tener ambos archivos en la misma carpeta, despues de esto usando python ejecutamos el archivo .py `python3 code.py`

```
RepugnamShip33-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/2/code.py
--2025-03-18 00:54:09--  https://artifacts.picoctf.net/c/2/code.py
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.128, 3.160.22.43, 3.160.22.92, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.128|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 1278 (1.2K) [application/octet-stream]
Saving to: 'code.py'

code.py                                         100%[======================================================================================================>]   1.25K  --.-KB/s    in 0s      

2025-03-18 00:54:09 (639 MB/s) - 'code.py' saved [1278/1278]

RepugnamShip33-picoctf@webshell:~$ ls
Addadshashanammu      README.txt     big-zip-files.zip  datos     files      ltdis.sh  static.1                  static.ltdis.x86_64.txt  warm
Addadshashanammu.zip  big-zip-files  code.py            enc_flag  files.zip  static    static.ltdis.strings.txt  strings
RepugnamShip33-picoctf@webshell:~$ wget https://artifacts.picoctf.net/c/2/codebook.txt
--2025-03-18 00:54:33--  https://artifacts.picoctf.net/c/2/codebook.txt
Resolving artifacts.picoctf.net (artifacts.picoctf.net)... 3.160.22.43, 3.160.22.128, 3.160.22.16, ...
Connecting to artifacts.picoctf.net (artifacts.picoctf.net)|3.160.22.43|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 27 [application/octet-stream]
Saving to: 'codebook.txt'

codebook.txt                                    100%[======================================================================================================>]      27  --.-KB/s    in 0s      

2025-03-18 00:54:33 (17.5 MB/s) - 'codebook.txt' saved [27/27]

RepugnamShip33-picoctf@webshell:~$ pyhton3 code.py
-bash: pyhton3: command not found
RepugnamShip33-picoctf@webshell:~$ python3 code.py
picoCTF{c0d3b00k_455157_7d102d7a}
```

#### Notas Adicionales

#### Referencias
