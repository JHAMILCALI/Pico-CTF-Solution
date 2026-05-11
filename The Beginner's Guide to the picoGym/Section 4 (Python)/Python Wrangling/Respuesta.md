nos da 3 archivos y los descargamos:

## Ejecutamos lo siguinte:

```bash
┌──(kali㉿kali)-[~/Downloads/pruebas/python]
└─$ ls
ende.py  flag.txt.en  password.txt
                                                                                                          
┌──(kali㉿kali)-[~/Downloads/pruebas/python]
└─$ cat password.txt 
720b6ad346f84cd483c60c7464dd95d4
                                                                                                          
┌──(kali㉿kali)-[~/Downloads/pruebas/python]
└─$ python ende.py -d flag.txt.en 
Please enter the password:720b6ad346f84cd483c60c7464dd95d4
picoCTF{4p0110_1n_7h3_h0us3_9c5f9bcf}

```
la flag que se encontro es **picoCTF{4p0110_1n_7h3_h0us3_9c5f9bcf}**
