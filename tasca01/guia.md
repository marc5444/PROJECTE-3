# Guia d'Ús Tècnica – Fase 2 (Bitwarden)


---


## 📌 Introducció


Aquesta guia està destinada al **personal tècnic** per garantir un ús correcte i segur de **Bitwarden**, el gestor de contrasenyes seleccionat en la Fase 1.
Inclou instruccions pas a pas per a la instal·lació, configuració, generació de contrasenyes segures, ús quotidià i còpies de seguretat.


> **Nota:** Les imatges de suport han d’estar dins de la carpeta `img/` del repositori.


---


## 1. Instal·lació i Configuració Inicial


### 1.1 Descàrrega i instal·lació


1. Accedeix a la pàgina oficial de Bitwarden: [https://bitwarden.com/download/](https://bitwarden.com/download/)
2. Descarrega l’aplicació corresponent al teu sistema operatiu (Windows, macOS, Linux, mòbil).
3. Executa l’instal·lador i segueix els passos habituals.


```text
Exemple: Windows → bitwarden-setup.exe → Next → Install → Finish
```


### 1.2 Creació del compte mestre


1. Obre l’aplicació Bitwarden.
2. Clica a **Crear compte**.
3. Introdueix:
- Correu electrònic corporatiu
- Contrasenya mestra segura
- Confirmació de contrasenya
4. Desa les dades i inicia sessió.


**Captura d’exemple:**
![Instal·lació Bitwarden](img/bitwarden_instalacio.png)


---


## 2. Generació de Contrasenyes Segures


1. Accedeix a **Eines → Generador de contrasenyes**.
2. Configura:
- Longitud mínima: 16 caràcters recomanats
- Caràcters especials: activats
- Majúscules i números: activats
3. Prem **Generar** i copia la contrasenya generada al registre de la credencial.


**Captura d’exemple:**
![Generador de contrasenyes](img/bitwarden_generador.png)


> **Consell:** Sempre utilitza el generador per a cada compte, mai reutilitzis contrasenyes.


---


## 3. Exemples d’Ús i Emplenament Automàtic


### 3.1 Desa una credencial de correu electrònic


1. Obre Bitwarden i selecciona **Afegir element**.
2. Introdueix:
- Nom del compte: `Correu corporatiu`
- Usuari / Correu: `usuari@empresa.com`
- Contrasenya: copiada del generador
3. Desa l’element.


**Captura d’exemple:**
![Afegir credencial](img/bitwarden_afegir_credencial.png)


### 3.2 Desa una credencial d’una aplicació o servei web


- Repeteix els passos anteriors indicant el nom del servei (ex. GitHub, Jira, etc.)
- Desa la contrasenya generada o existent.


### 3.3 Emplenament automàtic al navegador


1. Instal·la l’extensió de Bitwarden al navegador: [https://bitwarden.com/download/#browser](https://bitwarden.com/download/#browser)
2. Inicia sessió amb el teu compte mestre.
3. Quan accedeixis a un formulari de login, prem l’icona de Bitwarden i selecciona la credencial corresponent per **emplenar automàticament**.


**Captura d’exemple:**
![Autofill navegador](img/bitwarden_autofill.png)
