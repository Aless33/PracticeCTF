#### Descripción

The factory is hiding things from all of its users. Can you login as Joe and find what they've been looking at?
#### Solución 
En esta solucion nos metemos a inspeccionar la pagina, como es un login vemos que siempre trafica los datos para comprobar los datos introducidos, en esto vemos que se transportan las cookies entonces verificamos el almacenamiento de la pagina y vemos que la cookie almacena el usuario, el admin y la contraseña, podemos configurar para dar Admin a True, lo que nos desbloquea la flag.

`ppicoCTF{th3_c0nsp1r4cy_l1v3s_6edb3f5f}`


#### Notas Adicionales
Tambien se podia realizar haciendo una funcion aparte para descifrar por nuestra cuenta la flag.
#### Referencias
