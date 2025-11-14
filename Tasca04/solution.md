# GUIA LDAP

**Per Començar instal·lem LDAP**

![image](/Tasca04/Tasca04_1.1.png)

![image](/Tasca04/Tasca04_2.png)


**Ara mirem el status**

![image](/Tasca04/Tasca04_3.png)


**Amb sudo slapcat comprovem que els directoris s'hagin creat amb el nom que volem**

![image](/Tasca04/Tasca04_4.png)


**Configurem LDAP**

![image](/Tasca04/Tasca04_5.png)

![image](/Tasca04/Tasca04_6.png)

**Introduim el nom del domini DNS**

![image](/Tasca04/Tasca04_7.png)



**Posem la contrasenya de l'administrador**

![image](/Tasca04/Tasca04_8.png)




**A continuació instalarem el manager de comptes de LDAP**



![image](/Tasca04/Tasca04_15.png)

**Afegim usuaris i grups**

![image](/Tasca04/Tasca04_13.png)

![image](/Tasca04/Tasca04_14.png)

**Ara canviem la configuració**

![image](/Tasca04/Tasca04_12.png)




**Utilitzarem "ldapsearch"**

![image](/Tasca04/Tasca04_14.png)

Ara farem la instalació del gestor LDAP


![image](/Tasca04/Tasca04_16.png)

Un cop dintre hem d'accedir a Edit server profiles per començár la configuració del perfil del servidor.

![image](/Tasca04/Tasca04_40.png)

En aquest apartat configurarem les opcions generals del gestor, com el idioma, la compte de administrador y altres parámetres básics.

![image](/Tasca04/Tasca04_18.png)

A la segona pestanya Account Types, definirem els DN dels usuaris y dels grups, incluyent una OU per els usuaris y un  altre per els grups.



![image](/Tasca04/Tasca04_23.png)

A continuació, apareixera el panell de inici de sessió, al que accedirem amb el usuari administrador del domini:

Usuari: admin  
Contrasenya: p@ssw0rd

![image](/Tasca04/Tasca04_22.png)

6️⃣ Creació de grups y usuaris i Grups

Un cop dintre del panell de administració, hem de crear dos grups de seguretat en el directori: tech y manager.

Per fer-ho, anirem a Accounts → Groups.

Un cop dintre d'aquest apartat, farem clic en New group per crear els dos grups.

![image](/Tasca04/Tasca04_25.png)

Creació dels grups de seguretat tech i manager dins del LAM.

Despres de configurarlos, clickem Save per guardar els cambis.

![image](/Tasca04/Tasca04_26.png)


Per últim, ja tenim creats els dos grupos en el directori.


Usuaris

Repetirem el mateix proces per crear un usuari per cada grup, que es diuen tech01 y manager01.

Per fer-ho, ens dirigirem a Accounts → Users y farem clic en New user.

En el interior del formulari hem d'introducr la informació personal del usuari, com la dirección, el teléfon, la fotografía y altres dades básiques.

![image](/Tasca04/Tasca04_21.png)

També configurarem la informació Unix, necessaria per que el usuari pugui iniciar sessió en el client.

![image](/Tasca04/Tasca04_28.png)

En aquest pas, hem de crear el grup primari amb el mateix nom que el usuari.

![image](/Tasca04/Tasca04_41.png)

Deberemos añadir el usuario al grupo correspondiente.

Para ello, haremos clic en el botón Edit groups y, una vez dentro, moveremos el grupo tech (en este caso) en la sección Selected groups para asignarlo correctamente al usuario.

Por último, deberemos crear una contraseña para que el usuario de dominio pueda iniciar sesión.

Para ello, haremos clic en el botón Set password, introduciremos la contraseña 1234 y marcaremos la casilla que obliga al usuario a cambiarla en el primer inicio de sesión.

![image](/Tasca04/Tasca04_42.png)


**Ara ja podem entrar a la compte**

![image](/Tasca04/Tasca04_19.png)


**Crearem dos Grups i dos Usaris**

![image](/Tasca04/Tasca04_20.png)

![image](/Tasca04/Tasca04_21.png)

![image](/Tasca04/Tasca04_22.png)


**Ara configurem el nom del client**

![image](/Tasca04/Tasca04_23.png)


**Comprovem que els noms funcionen correctament**

![image](/Tasca04/Tasca04_24.png)


**Ara instal·lem els moduls necessaris**

![image](/Tasca04/Tasca04_25.png)


**Ara els configurem**

![image](/Tasca04/Tasca04_26.png)

![image](/Tasca04/Tasca04_27.png)

![image](/Tasca04/Tasca04_28.png)

![image](/Tasca04/Tasca04_29.png)

![image](/Tasca04/Tasca04_30.png)

![imagen](img/Tasca01_4.1.png)

![imagen](img/Tasca01_4.1.png)
