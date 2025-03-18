#### Descripción

My team has been working very hard on new features for our flag printing program! I wonder how they'll work together?
###### Pistas
- `git branch -a` will let you see available branches
- How can file 'diffs' be brought to the main branch? Don't forget to `git config`!
- Merge conflicts can be tricky! Try a text editor like nano, emacs, or vim.
#### Solución 
En este se solucina cambiando entre ramas, recordando como cada una puede tener diferente control de versiones, se identifica en cada una de esas el diferente tipo de archivo, viendo que aunque tengan el mismo nombre, no todos tienen la misma informaicon, haciendo asi que por partes este la flag.
 ```
 RepugnamShip33-picoctf@webshell:~$ cd drop-in
RepugnamShip33-picoctf@webshell:~/drop-in$ git branch -a
RepugnamShip33-picoctf@webshell:~/drop-in$ git checkout feature/part-1
Switched to branch 'feature/part-1'
RepugnamShip33-picoctf@webshell:~/drop-in$ ls
flag.py
RepugnamShip33-picoctf@webshell:~/drop-in$ python3 flag.py
Printing the flag...
picoCTF{t3@mw0rk_RepugnamShip33-picoctf@webshell:~/drop-in$ 
RepugnamShip33-picoctf@webshell:~/drop-in$ git checkout feature/part-2
Switched to branch 'feature/part-2'
RepugnamShip33-picoctf@webshell:~/drop-in$ python3 flag.py
Printing the flag...
m@k3s_th3_dr3@m_RepugnamShip33-picoctf@webshell:~/drop-in$ git checkout feature/part-3
Switched to branch 'feature/part-3'
RepugnamShip33-picoctf@webshell:~/drop-in$ python3 flag.py
Printing the flag...
w0rk_7ffa0077}
```

#### Notas Adicionales

#### Referencias
