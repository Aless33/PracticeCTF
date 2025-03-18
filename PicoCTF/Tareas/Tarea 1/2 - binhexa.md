#### Descripción

How well can you perfom basic binary operations?

Additional details will be available after launching your challenge instance.
#### Solución 
Para esto tenemos que recurrir a pagina como cyberchef que me ayudaran a sacar los resultados correctos, con esto hecho podemos usar python para realizar los and y or y los mayores y menores, con esto hecho solo queda usar una vez mas cyberchef para sacar el hexadecimal y asi obtener la flag.
```
Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 10101101
Binary Number 2: 11011111


Question 1/6:
Operation 1: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00101011
Incorrect. Try again
Enter the binary result: 110001100
Correct!

Question 2/6:
Operation 2: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 1001011010110011
Correct!

Question 3/6:
Operation 3: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00
Incorrect. Try again
Enter the binary result: 0
Incorrect. Try again
Enter the binary result: 1
Incorrect. Try again
Enter the binary result: |

Incorrect input. Provide the right input
Enter the binary result: 0.0110001010111001111110010001110010110011000101011101

Incorrect input. Provide the right input
Enter the binary result: 0.0110001010111001111110010001110010110011000101011101

Incorrect input. Provide the right input
Enter the binary result: 1111111111
Incorrect. Try again
Enter the binary result: 11111111
Correct!

Question 4/6:
Operation 4: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 101011010
Correct!

Question 5/6:
Operation 5: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 10001101
Correct!

Question 6/6:
Operation 6: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 01101111
Correct!

Enter the results of the last operation in hexadecimal: 6F

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_d6f8047e}
```

#### Notas Adicionales

#### Referencias
https://numerosbinarios.net/396-en-binario
https://es.planetcalc.com/911/
https://gchq.github.io/CyberChef/#recipe=From_Decimal('Space',false)&input=MTEyIA0KMTA1IA0KOTkgDQoxMTEgDQo2NyANCjg0IA0KNzAgDQoxMjMgDQoxMDMgDQo0OCANCjQ4IA0KMTAwIA0KOTUgDQoxMDcgDQo0OSANCjExNiANCjExNiANCjEyMSANCjMzIA0KOTUgDQoxMTAgDQo0OSANCjk5IA0KNTEgDQo5NSANCjEwNyANCjQ5IA0KMTE2IA0KMTE2IA0KMTIxIA0KMzMgDQo5NSANCjEwMiANCjUwIA0KMTAwIA0KNTUgDQo5OSANCjk3IA0KMTAyIA0KOTcgDQoxMjUgDQoxMCA&ieol=CRLF