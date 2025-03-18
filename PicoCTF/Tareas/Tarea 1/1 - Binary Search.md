#### Descripción

Want to play a game? As you use more of the shell, you might be interested in how they work! Binary search is a classic algorithm used to quickly find an item in a sorted list. Can you find the flag? You'll have 1000 possibilities and only 10 guesses.Cyber security often has a huge amount of data to look through - from logs, vulnerability reports, and forensics. Practicing the fundamentals manually might help you in the future when you have to write your own tools!
###### Pistas
- Have you ever played hot or cold? Binary search is a bit like that.
- You have a very limited number of guesses. Try larger jumps between numbers!
- The program will randomly choose a new number each time you connect. You can always try again, but you should start your binary search over from the beginning - try around 500. Can you think of why?

#### Solución 
Usando la logica, podemos hacer uso de la formula. de busqueda binaria $$ \frac{min + max}{2} = x $$ para descartar la mitad de resultados, ya sea por ejemplo que sea mas alto o mas bajo, en ese caso es buscar el punto medio para descartar nuevamente. 

```
Welcome to the Binary Search Game!
I'm thinking of a number between 1 and 1000.
Enter your guess: 500
Lower! Try again.
Enter your guess: 200
Lower! Try again.
Enter your guess: 100
Higher! Try again.
Enter your guess: 150
Lower! Try again.
Enter your guess: 125
Higher! Try again.
Enter your guess: 135
Higher! Try again.
Enter your guess: 140
Higher! Try again.
Enter your guess: 146
Lower! Try again.
Enter your guess: 144
Lower! Try again.
Enter your guess: 142
Congratulations! You guessed the correct number: 142
Here's your flag: picoCTF{g00d_gu355_2e90d29b}
Connection to atlas.picoctf.net closed.
```

#### Notas Adicionales

#### Referencias