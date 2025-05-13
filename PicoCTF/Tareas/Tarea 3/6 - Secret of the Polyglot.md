#### Descripción
The Network Operations Center (NOC) of your local institution picked up a suspicious file, they're getting conflicting information on what type of file it is. They've brought you in as an external expert to examine the file. Can you extract all the information from this strange file?Download the suspicious file [here](https://artifacts.picoctf.net/c_titan/96/flag2of2-final.pdf).
##### Pista
This problem can be solved by just opening the file in different ways

#### Solución 
Abrimos el pdf, con el comando `open`
Al momento de ver el pdf, nos dan la mitad de la flag
Con el comando `convert` permite manipular imágenes desde diferente formatos, en este caso se convierte un archivo PD en una imágen PNG. Obteniendo la flag completa.
```
picoCTF{f1u3n7_1n_pn9_&_pdf_90974127}
```


#### Notas Adicionales

#### Referencias
