#### Descripción
In RSA, a small `e` value can be problematic, but what about `N`? Can you decrypt this? [values](https://mercury.picoctf.net/static/bf5e2c8811afb4669f4a6850e097e8aa/values)

##### Pista
Bits are expensive, I used only a little bit over 100 to save money

#### Solución 
Tenemos unos parametros del metodo RSA, por lo que usaremos una pagina para desencriuptar RSA: "https://www.dcode.fr/rsa-cipher". Asi obtenemos la flag
```
picoCTF{sma11_N_n0_g0od_55304594}
```

