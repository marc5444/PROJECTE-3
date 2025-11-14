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

![image](/Tasca04/Tasca04_41.png)

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

Hem  d'afegir el usuari el grup corresponent.

Per fer aixo , farem clic en el botó Edit groups y, un cop dintre, mourem el grup tech (en aquest cas) a la secció Selected groups per asignarlo correctament al usuari.

Per últim, hem de crear una contrasenya per a que el usuari de domini pugui iniciar sessió.

Per fer-ho, farem clic en el botó Set password, introduuirem la contrasenya 1234 y marcarem la casilla que obliga al usuari a cambiarla en el primer inici de sesió.

![image](/Tasca04/Tasca04_42.png)

Un cop completats aquests pasos, guardarem,el nou usuari fent clic en el boto Save.

A continuació, repetirem el mateix proces amb el usuari i el grup manager01, hem obtingut  el següent resultat:

![image](/Tasca04/Tasca04_43.png)


7️⃣ **Configuració del client (ZorinOS)**  
Per comprovar que el servidor LDAP funciona correctament, configurarem un client ZorinOS.

A aquest client li crearem una segona interfície de xarxa en mode *host-only*, perquè es pugui comunicar amb el servidor.

Un cop dins del client, haurem de configurar el nom de l’equip perquè formi part del mateix domini que el servidor.

Com que no disposem d’un servei DNS, editarem el fitxer `/etc/hosts` del client perquè pugui resoldre correctament el nom del servidor.

![image](/Tasca04/Tasca04_44.png)

Ara comprovarem que els noms es resolen correctament executant les següents ordres:

### Verificar el nom de *host* del client
Per assegurar-nos que el nom de l’equip s’ha canviat correctament:

```bash
hostname -f


![image](/Tasca04/Tasca04_45.png)

