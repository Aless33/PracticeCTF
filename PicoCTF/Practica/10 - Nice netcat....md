#### Descripcion

There is a nice program that you can talk to by using this command in a shell: `$ nc mercury.picoctf.net 7449`, but it doesn't speak English...
	
PISTA: You can practice using netcat with this picoGym problem: [what's a netcat?](https://play.picoctf.org/practice/challenge/34)
PISTA: You can practice reading and writing ASCII with this picoGym problem: [Let's Warm Up](https://play.picoctf.org/practice/challenge/22)
#### Solución 
```
112 
105 
99 
111 
67 
84 
70 
123 
103 
48 
48 
100 
95 
107 
49 
116 
116 
121 
33 
95 
110 
49 
99 
51 
95 
107 
49 
116 
116 
121 
33 
95 
102 
50 
100 
55 
99 
97 
102 
97 
125 
10 

RECIPE. From Decimal.
OUTPUT:

picoCTF{g00d_k1tty!_n1c3_k1tty!_f2d7cafa}

```

##### Notas Adicionales
Usando Cyberchef podemos interpretar los decimales.
Con los numero podemos sacar la respuesta despues de transformarlos
##### Referencias

https://webshell.picoctf.org/

https://gchq.github.io/CyberChef/#recipe=From_Decimal('Space',false)&input=MTEyIA0KMTA1IA0KOTkgDQoxMTEgDQo2NyANCjg0IA0KNzAgDQoxMjMgDQoxMDMgDQo0OCANCjQ4IA0KMTAwIA0KOTUgDQoxMDcgDQo0OSANCjExNiANCjExNiANCjEyMSANCjMzIA0KOTUgDQoxMTAgDQo0OSANCjk5IA0KNTEgDQo5NSANCjEwNyANCjQ5IA0KMTE2IA0KMTE2IA0KMTIxIA0KMzMgDQo5NSANCjEwMiANCjUwIA0KMTAwIA0KNTUgDQo5OSANCjk3IA0KMTAyIA0KOTcgDQoxMjUgDQoxMCA&ieol=CRLF