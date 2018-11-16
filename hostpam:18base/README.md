# PAM
## @edt ASIX M06-ASO Curs 2018-2019

Repositori d'exemples de containers docker que utilitzen PAM

 * **hostpam:base** exemple bàsic de host que usa pam, autentica contra el container *edtasixm06/ldapserver:18group*.

#### Execució

```
docker run --rm --name host -h host --net ldapnet -it edtasixm06/hostpam:base
```

#### Utilització

```
getnet passwd local01
getent passwd pau
getent passwd

getent group localgrp01
getent group 2asix
getent group
```

