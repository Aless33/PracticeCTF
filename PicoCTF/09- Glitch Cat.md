#### Descripcion
Our flag printing service has started glitching!

Additional details will be available after launching your challenge instance.

PISTA 1: ASCII is one of the most common encodings used in programming
PISTA 2:We know that the glitch output is valid Python, somehow!
PISTA 3:Press Ctrl and c on your keyboard to close your connection and return to the command prompt.
#### Solucion
- Nos conectamos al puerto y recibimos una cadena
- Luego nos pasamos a Python y pegamos la cadena
```
RepugnamShip33-picoctf@webshell:~$ nc saturn.picoctf.net 60432
'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'
^C
RepugnamShip33-picoctf@webshell:~$ ^C
RepugnamShip33-picoctf@webshell:~$ 'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'

-bash: syntax error near unexpected token `('
RepugnamShip33-picoctf@webshell:~$ ^C
RepugnamShip33-picoctf@webshell:~$ 'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'

-bash: syntax error near unexpected token `('
RepugnamShip33-picoctf@webshell:~$ picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '} 
-bash: picoCTF{gl17ch_m3_n07_ + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + }: command not found
RepugnamShip33-picoctf@webshell:~$ python
Python 3.10.12 (main, Sep 11 2024, 15:47:36) [GCC 11.4.0] on linux
Type "help", "copyright", "credits" or "license" for more information.
>>> 'picoCTF{gl17ch_m3_n07_' + chr(0x61) + chr(0x34) + chr(0x33) + chr(0x39) + chr(0x32) + chr(0x64) + chr(0x32) + chr(0x65) + '}'
'picoCTF{gl17ch_m3_n07_a4392d2e}'
```
##### Notas Adicionales
Usando Python podemos concatenar para obtener el resultado
##### Referencias

https://webshell.picoctf.org/