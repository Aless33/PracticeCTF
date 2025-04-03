#### Descripción

How about trying to match a regular expression

Additional details will be available after launching your challenge instance.
##### Pista
Access the webpage and try to match the regular expression associated with the text field

#### Solución 
En esta solucion, lo que tenemos que hacer es realizar un escaneo y ver el codigo fuente de la pagina y podemos observar el siguiente codigo:
```
|---|
|function send_request() {|
||let val = document.getElementById("name").value;|
||// ^p.....F!?|
||fetch(`/flag?input=${val}`)|
||.then(res => res.text())|
||.then(res => {|
||const res_json = JSON.parse(res);|
||alert(res_json.flag)|
||return false;|
||})|
||return false;|
||}|
```
En este codigo podemos ver que si el input contiene la palabra PicoCTF este devuelve la flag por lo cual en el input introducimos esto y nos regresa la flag.
```
picoCTF{succ3ssfully_matchtheregex_0694f25b}
```


#### Notas Adicionales

#### Referencias
