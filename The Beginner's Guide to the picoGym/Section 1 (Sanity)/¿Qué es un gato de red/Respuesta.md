#### Pregunta
Usar netcat (nc) será bastante importante. ¿Puedes conectarte a fickle-tempest.picoctf.net en el puerto 51482 ¿para conseguir la bandera?
**Para esto hay que instalar netcat (mi caso Kali linux)**
**Ejecutamso lo sigunte = **
```bash
nc fickle-tempest.picoctf.net 51482
```
### Solcuion completa
```bash                                     
┌──(kali㉿kali)-[~]
└─$ sudo apt install netcat-openbsd
Installing:                     
  netcat-openbsd

Summary:
  Upgrading: 0, Installing: 1, Removing: 0, Not Upgrading: 1278
  Download size: 38.7 kB
  Space needed: 108 kB / 62.8 GB available

Get:1 http://kali.download/kali kali-rolling/main amd64 netcat-openbsd amd64 1.234-2 [38.7 kB]
Fetched 38.7 kB in 1s (66.0 kB/s)   
Selecting previously unselected package netcat-openbsd.
(Reading database… 426154 files and directories currently installed.)
Preparing to unpack …/netcat-openbsd_1.234-2_amd64.deb…
Unpacking netcat-openbsd (1.234-2)…
Setting up netcat-openbsd (1.234-2)…
update-alternatives: using /bin/nc.openbsd to provide /bin/nc (nc) in auto mode
Processing triggers for kali-menu (2026.1.5)…
Processing triggers for man-db (2.13.1-1)…
                                                                                                                                                                
┌──(kali㉿kali)-[~]
└─$ nc fickle-tempest.picoctf.net 51482
You're on your way to becoming the net cat master
picoCTF{nEtCat_Mast3ry_aC66D475}
        
```

## Flag encontrada **picoCTF{nEtCat_Mast3ry_aC66D475}**