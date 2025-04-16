#### Descripción

BookShelf Pico, my premium online book-reading service. I believe that my website is super secure. I challenge you to prove me wrong by reading the 'Flag' book!

Additional details will be available after launching your challenge instance.
###### Pistas
- Maybe try to find the JWT Signing Key ("secret key") in the source code? Maybe it's hardcoded somewhere? Or maybe try to crack it?
- The 'role' and 'userId' fields in the JWT can be of interest to you!
- The 'controllers', 'services' and 'security' java packages in the given source code might need your attention. We've provided a README.md file that contains some documentation.
- Upgrade your 'role' with the _new_ (cracked) JWT. And re-login for the new role to get reflected in browser's localStorage.

#### Solución 
Para este reto lo que tenemos que hacer es ver la informacion que tiene la pagina a la hora de ver el libro bloqueado, como podemos ver este utiliza jwt en donde puede codear los requisitos para restringir algo sin ser usuario admin, por eso vamos a tener que modificar utilizando jwt para poder realizar el ejercicio, en donde lo tenemos que dejar de la siguiente manera:

```
{
  "role": "Admin",
  "iss": "bookshelf",
  "exp": 1745373931,
  "iat": 1744769131,
  "userId": 2,
  "email": "admin"
}
```

transformandolo en el codigo este lo ponemos en la pagina y recargamos, asi nos dara acceso al libro que contiene la flag.
`picoCTF{w34k_jwt_n0t_g00d_6e5d7df5}`