#### Descripción

Someone's commits seems to be preventing the program from working. Who is it?

###### Pistas
- In collaborative projects, many users can make many changes. How can you see the changes within one file?
- Read the chapter on Git from the picoPrimer.
- You can use `python3 <file>.py` to try running the code, though you won't need to for this challenge.
#### Solución 

En este reto tenemos que saber quien fue la persona que hizo cmabios al documento que se encuentra en el paquete que nos da el reto. Hacemos uso del comando `unzip` para descomprimir el paquete. Ahora nos dirigimos a la carpeta:

- `cd drop-in` Observamos que tenemos un solo archivo, pero que en su interior no tiene nada que nos interese por lo tanto.
- Hacemos uso del comando `log`en el cual git muestra el historial de las personas que hicieron cambios en el documento.
Con esto hecho podemos ver que en el documento esta el autor de este git y vemos que es la bandera.
```
commit 9ae3e1bc67ad0143c611c5f65399b79850d20983
Author: picoCTF{@sk_th3_1nt3rn_b64c4705} <ops@picoctf.com>
Date:   Sat Mar 9 21:09:01 2024 +0000

    optimize file size of prod code

commit f3cec26cf7f80f91b5c3d1972f14dd4e9f97ec83
Author: picoCTF <ops@picoctf.com>
Date:   Sat Mar 9 21:09:01 2024 +0000
```
#### Referencias
