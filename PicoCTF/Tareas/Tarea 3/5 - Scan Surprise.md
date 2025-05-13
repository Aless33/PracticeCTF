#### Descripción
I've gotten bored of handing out flags as text. Wouldn't it be cool if they were an image instead?You can download the challenge files here.

Additional details will be available after launching your challenge instance.
##### Pista
1. QR codes are a way of encoding data. While they're most known for storing URLs, they can store other things too.
2. Mobile phones have included native QR code scanners in their cameras since version 8 (Oreo) and iOS 11
3. If you don't have access to a phone, you can also use zbar-tools to convert an image to text

#### Solución 
Nos conectamos al server con `ssh`
Aplicamos un ls, ahi se encuentra flag.png, que es un código de barras.

El comando `zbarimg` sirve para leer y decodificar códigos de barras y códigos QR contenidos en una imagen, obteniendo la flag.
```
picoCTF{p33k_@_b00_7843f77c}
```


#### Notas Adicionales

#### Referencias
