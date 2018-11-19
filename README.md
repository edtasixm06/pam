# pam

## @edt ASIX M06 2018-2019


Podeu trobar les imatges docker al Dockehub de [edtasixm06](https://hub.docker.com/u/edtasixm06/)

ASIX M06-ASO Escola del treball de barcelona

### Imatges:

* **pamhost:18base** host pam que autentica els usuaris contra ldap. Usar el container *ldapserver:18group*.

* **pamhost:18auth** host pam amb authenticació ldap. utilitza l'ordre authconfig per configurar l'autenticació.

#### Execució

```
docker run --rm --name host -h host --net ldapnet -it edtasixm06/hostpam:18base 
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

