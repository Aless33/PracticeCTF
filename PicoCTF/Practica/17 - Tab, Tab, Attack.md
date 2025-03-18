#### Descripción
Using tabcomplete in the Terminal will add years to your life, esp. when dealing with long rambling directory structures and filenames

Pista: After `unzip`ing, this problem can be solved with 11 button-presses...(mostly Tab)...

#### Solución 
Usando el `unzip` al ver que contamos con varios directorios lo que vamos a hacer es usando cd y el tab del teclado vemos

```
RepugnamShip33-picoctf@webshell:~$ cd^C
RepugnamShip33-picoctf@webshell:~$ cd  Addadshashanammu
RepugnamShip33-picoctf@webshell:~/Addadshashanammu$ cd Almurbalarammi/
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi$ cd Ashalmimilkala/
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala$ cd Assurnabitashpi/
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi$ cd Maelkashishi/
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi$ cd Onnissiralis/
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis$ cd Ularradallaku/
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ cd 
RepugnamShip33-picoctf@webshell:~$ ls
Addadshashanammu      README.txt     big-zip-files.zip  enc_flag  files.zip  static    static.ltdis.strings.txt  strings
Addadshashanammu.zip  big-zip-files  datos              files     ltdis.sh   static.1  static.ltdis.x86_64.txt
RepugnamShip33-picoctf@webshell:~$ cd Ularradallaku/
-bash: cd: Ularradallaku/: No such file or directory
RepugnamShip33-picoctf@webshell:~$ cd  Addadshashanammu
RepugnamShip33-picoctf@webshell:~/Addadshashanammu$ cd Almurbalarammi/  
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi$ cd Ashalmimilkala/
8#TT 1tt$DNp33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala$ cd Assurnabitashpi/
0)@ugnam(;RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ chmod +x fang-of-haynekhtnamet
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ ./fang-of-haynekhtnamet
*ZAP!* picoCTF{l3v3l_up!_t4k3_4_r35t!_2bcfb2ab}mmu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis$ cd Ularradallaku/
RepugnamShip33-picoctf@webshell:~/Addadshashanammu/Almurbalarammi/Ashalmimilkala/Assurnabitashpi/Maelkashishi/Onnissiralis/Ularradallaku$ ls 
```
#### Notas Adicionales

Con el tab podemos ingresar a la carpeta siguiente si es que existe una adentro de otra
#### Referencias
