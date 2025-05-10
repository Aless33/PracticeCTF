#### Descripción
Use `srch_strings` from the sleuthkit and some terminal-fu to find a flag,

##### Pista
- Have you ever used `file` to determine what a file was?
- Relevant terminal-fu in picoGym: https://play.picoctf.org/practice/challenge/85
- Mastering this terminal-fu would enable you to find the flag in a single command: https://play.picoctf.org/practice/challenge/48
- Using your own computer, you could use qemu to boot from this disk!

#### Solución 
Para este problema lo primero que tenemos que hacer es realizar el unzip del archivo, para eso podemos utilizar `gunzip`, despues de descomprimir, usaremos `srch_strings` que lo que hace es recorrer la imagen en bruto en cusca de secuencias imprimibles, es por eso que lo que vamos a hacer es decirle que ponga las strings que encuentre en un archivo .txt: `srch_strings dds1-alpine.flag.img > cadena.txt`, con esto todo lo que se paso a texto estara en el documendo de cadena, por lo que podemos usar `grep` en el archivo para obtener la flag.
```
picoCTF{f0r3ns1c4t0r_n30phyt3_a69a712c}
```

