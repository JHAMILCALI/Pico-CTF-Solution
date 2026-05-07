Abre una terminal y escribe este comando:

**ssh ctf-player@titan.picoctf.net -p 51516**

Luego te preguntará algo como:

Are you sure you want to continue connecting (yes/no/[fingerprint])?

Escribe:

**yes**

Después te pedirá la contraseña. Copia y pega esta:

**83dcefb7**

```bash
jhamilcali-picoctf@webshell:~$ ssh ctf-player@titan.picoctf.net -p 51516
The authenticity of host '[titan.picoctf.net]:51516 ([3.139.174.234]:51516)' can't be established.
ED25519 key fingerprint is SHA256:4S9EbTSSRZm32I+cdM5TyzthpQryv5kudRP9PIKT7XQ.
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[titan.picoctf.net]:51516' (ED25519) to the list of known hosts.
ctf-player@titan.picoctf.net's password: 
Welcome ctf-player, here's your flag: picoCTF{s3cur3_c0nn3ct10n_8969f7d3}
Connection to titan.picoctf.net closed.
```

la Flag encontrada es =  **picoCTF{s3cur3_c0nn3ct10n_8969f7d3}**