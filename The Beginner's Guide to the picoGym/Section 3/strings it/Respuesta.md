Ese comando tiene **2 partes**:

```bash
strings ./strings | grep pico
```

### 1. `strings ./strings`

`strings` es un comando de Linux que busca texto legible dentro de un archivo, aunque el archivo sea binario.

En tu caso:

```bash
./strings
```

es el archivo que descargaste.

Entonces:

```bash
strings ./strings
```

significa:

> “Muéstrame todos los textos legibles que hay dentro del archivo llamado `strings`”.

Por ejemplo, dentro de un binario puede haber textos como:

```text
Hello World
error
password
picoCTF{...}
```

---

### 2. `|`

La barra vertical se llama **pipe**.

Sirve para mandar la salida de un comando como entrada de otro comando.

O sea:

```bash
strings ./strings | grep pico
```

significa:

> “Primero saca todos los textos legibles del archivo, y luego filtra solo las líneas que contengan `pico`”.

---

### 3. `grep pico`

`grep` busca texto.

Entonces:

```bash
grep pico
```

muestra solamente las líneas que tengan la palabra:

```text
pico
```

---

En resumen:

```bash
strings ./strings | grep pico
```

quiere decir:

> “Busca todos los textos legibles dentro del archivo `strings` y muéstrame solo los que contengan `pico`”.



```bash
┌──(kali㉿kali)-[~/Downloads/pruebas]
└─$ wget https://challenge-files.picoctf.net/c_fickle_tempest/fd00e7cc9b263f22c323572d2d5fc37d170f8e58e99a91f8991d0f07c69b21ff/strings
--2026-05-07 22:15:48--  https://challenge-files.picoctf.net/c_fickle_tempest/fd00e7cc9b263f22c323572d2d5fc37d170f8e58e99a91f8991d0f07c69b21ff/strings
Resolving challenge-files.picoctf.net (challenge-files.picoctf.net)... 3.175.45.107, 3.175.45.70, 3.175.45.110, ...
Connecting to challenge-files.picoctf.net (challenge-files.picoctf.net)|3.175.45.107|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 784424 (766K) [application/octet-stream]
Saving to: ‘strings’

strings                      100%[============================================>] 766.04K  1.39MB/s    in 0.5s    

2026-05-07 22:15:50 (1.39 MB/s) - ‘strings’ saved [784424/784424]

                                                                                                                  
┌──(kali㉿kali)-[~/Downloads/pruebas]
└─$ ls
strings  warm

┌──(kali㉿kali)-[~/Downloads/pruebas]
└─$ strings ./strings | grep pico
picoCTF{5tRIng5_1T_FB7D7Bb6}
```

Flag encontrada : **picoCTF{5tRIng5_1T_FB7D7Bb6}**