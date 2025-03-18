#### Descripción
Unzip this archive and find the file named 'uber-secret.txt'

#### Solución 
Usamos el comando find para realizar las busquedas para encontrar el txt de "uber-secret.txt"
tenemos que usar una lista de comandos de find para decirle que debe buscar, empezando por el tipo que es un archivo .txt y el nombre del archivo. 
Por ultimo usamos cat para con la direccion del archivo obtenida podamos ver la flag.
```
RepugnamShip33-picoctf@webshell:~$ unzip files.zip      
Archive:  files.zip
   creating: files/
   creating: files/satisfactory_books/
   creating: files/satisfactory_books/more_books/
  inflating: files/satisfactory_books/more_books/37121.txt.utf-8  
  inflating: files/satisfactory_books/23765.txt.utf-8  
  inflating: files/satisfactory_books/16021.txt.utf-8  
  inflating: files/13771.txt.utf-8   
   creating: files/adequate_books/
   creating: files/adequate_books/more_books/
   creating: files/adequate_books/more_books/.secret/
   creating: files/adequate_books/more_books/.secret/deeper_secrets/
   creating: files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/
 extracting: files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt  
  inflating: files/adequate_books/more_books/1023.txt.utf-8  
  inflating: files/adequate_books/46804-0.txt  
  inflating: files/adequate_books/44578.txt.utf-8  
   creating: files/acceptable_books/
   creating: files/acceptable_books/more_books/
  inflating: files/acceptable_books/more_books/40723.txt.utf-8  
  inflating: files/acceptable_books/17880.txt.utf-8  
  inflating: files/acceptable_books/17879.txt.utf-8  
  inflating: files/14789.txt.utf-8   
RepugnamShip33-picoctf@webshell:~$ find uber-secret-txt  
find: 'uber-secret-txt': No such file or directory
RepugnamShip33-picoctf@webshell:~$ find -type f -name "uber-secret-txt" 
RepugnamShip33-picoctf@webshell:~$ find -type f -name "uber-secret-txt"^C
RepugnamShip33-picoctf@webshell:~$ find -type f -name "uber-secret.txt"
./files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
RepugnamShip33-picoctf@webshell:~$ cat ./files/adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
picoCTF{f1nd_15_f457_ab443fd1}
RepugnamShip33-picoctf@webshell:~$ ^C
```


#### Notas Adicionales


#### Referencias
