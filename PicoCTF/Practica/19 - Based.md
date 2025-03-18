#### Descripción
To get truly 1337, you must understand different data encodings, such as hexadecimal or binary. Can you get the flag from this program to prove you are on the way to becoming 1337?

PISTAS: I hear python can convert things. 
It might help to have multiple windows open.

#### Solución 
Usando Cyberchef y a su vez tambien python se puede sacar lo que se nos pide, que seria una palabra en binario, otra por una serie de numeros y la ultima hexadecimal.
```
RepugnamShip33-picoctf@webshell:~$ nc jupiter.challenges.picoctf.org 29221
Let us see how data is stored
light
Please give the 01101100 01101001 01100111 01101000 01110100 as a word.
...
you have 45 seconds.....

Input:
light
Please give me the  163 164 162 145 145 164 as a word.
Input:
street
Please give me the 616e696d6174696f6e as a word.
Input:
animation
You've beaten the challenge
Flag: picoCTF{learning_about_converting_values_00a975ff}
```

#### Notas Adicionales

Para este ejercicio se pueden usar las herramientas de python que cuenta con convertidor de binarios y hexadecimales, las palabras son al azar.
#### Referencias
https://gchq.github.io/CyberChef/#recipe=From_Octal('Space'/disabled)From_Hex('None')&input=NjE2ZTY5NmQ2MTc0Njk2ZjZl&ieol=CRLF&oeol=CRLF
