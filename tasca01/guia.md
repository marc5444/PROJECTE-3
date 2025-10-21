# Guia d'Ús Tècnica – Fase 2 (Bitwarden)

---

## Índex

1. [Introducció](#introducció)
2. [Instal·lació i Configuració Inicial](#instal·lació-i-configuració-inicial)
   1. [Descàrrega i instal·lació](#descàrrega-i-instal·lació)
   2. [Creació del compte mestre](#creació-del-compte-mestre)
3. [Generació de Contrasenyes Segures](#generació-de-contrasenyes-segures)
4. [Exemples d’Ús i Emplenament Automàtic](#exemples-dús-i-emplenament-automàtic)
   1. [Desa una credencial de correu electrònic](#desa-una-credencial-de-correu-electrònic)
   2. [Desa una credencial d’una aplicació o servei web](#desa-una-credencial-duna-aplicació-o-servei-web)
   3. [Emplenament automàtic al navegador](#emplenament-automàtic-al-navegador)
5. [Gestió de Còpies de Seguretat (Backup)](#gestió-de-còpies-de-seguretat-backup)
   1. [Exportació de la base de dades](#exportació-de-la-base-de-dades)
   2. [Millors pràctiques d’emmagatzematge](#millors-pràctiques-demmagatzematge)
6. [Materials i Enllaços de Suport](#materials-i-enllaços-de-suport)
7. [Autor i Dades](#autor-i-dades)

---

## Introducció

Aquesta guia està destinada al **personal tècnic** per garantir un ús correcte i segur de **Bitwarden**, el gestor de contrasenyes seleccionat en la Fase 1. Inclou instruccions pas a pas per a la instal·lació, configuració, generació de contrasenyes segures, ús quotidià i còpies de seguretat.

> Nota: Les imatges de suport s’han d’incloure en la carpeta `img/` si es volen afegir al document.

---

## Instal·lació i Configuració Inicial

### Descàrrega i instal·lació

1. Accedeix a la pàgina oficial de Bitwarden: [https://bitwarden.com/download/](https://bitwarden.com/download/)  
2. Descarrega l’aplicació corresponent al teu sistema operatiu (Windows, macOS, Linux, mòbil).  
3. Executa l’instal·lador i segueix els passos habituals.

**Exemple Windows:**  
`bitwarden-setup.exe → Next → Install → Finish`

### Creació del compte mestre

1. Obre l’aplicació Bitwarden.  
2. Clica a **Crear compte**.  
3. Introdueix:  
   - Correu electrònic corporatiu  
   - Contrasenya mestra segura  
   - Confirmació de contrasenya  
4. Desa les dades i inicia sessió.

---

## Generació de Contrasenyes Segures

Bitwarden inclou un **generador de contrasenyes** integrat:

1. Accedeix a **Eines → Generador de contrasenyes**.  
2. Configura:  
   - Longitud mínima: 16 caràcters recomanats  
   - Caràcters especials: activats  
   - Majúscules i números: activats  
3. Prem **Generar** i copia la contrasenya generada al registre de la credencial.

> Consell: Sempre utilitza el generador per a cada compte, mai reutilitzis contrasenyes.

---

## Exemples d’Ús i Emplenament Automàtic

### Desa una credencial de correu electrònic

1. Obre Bitwarden i selecciona **Afegir element**.  
2. Introdueix:  
   - Nom del compte: `Correu corporatiu`  
   - Usuari / Correu: `usuari@empresa.com`  
   - Contrasenya: copiada del generador  
3. Desa l’element.

### Desa una credencial d’una aplicació o servei web

- Repeteix els passos anteriors indicant el nom del servei (ex. GitHub, Jira, etc.)  
- Desa la contrasenya generada o existent.

### Emplenament automàtic al navegador

1. Instal·la l’extensió de Bitwarden al navegador: [https://bitwarden.com/download/#browser](https://bitwarden.com/download/#browser)  
2. Inicia sessió amb el teu compte mestre.  
3. Quan accedeixis a un formulari de login, prem l’icona de Bitwarden i selecciona la credencial corresponent per emplenar automàticament.

---

## Gestió de Còpies de Seguretat (Backup)

### Exportació de la base de dades

1. Obre Bitwarden i accedeix a **Eines → Exportar dades**.  
2. Introdueix la contrasenya mestra per validar.  
3. Desa l’arxiu **xifrat** en una ubicació segura.

### Millors pràctiques d’emmagatzematge

- Emmagatzema la còpia de seguretat en **una unitat USB xifrada**.  
- Opcionalment, utilitza **emmagatzematge xifrat al núvol** amb accés restringit.  
- No comparteixis la contrasenya mestra ni l’arxiu amb tercers.

---

## Materials i Enllaços de Suport

- **INCIBE:** Gestió de contrasenyes segures  
  [https://www.incibe.es/protege-tu-empresa/seguridad-en-la-empresa/gestores-de-contrasenas](https://www.incibe.es/protege-tu-empresa/seguridad-en-la-empresa/gestores-de-contrasenas)  
- **Pàgina oficial de Bitwarden:** [https://bitwarden.com/](https://bitwarden.com/)  
- **Pàgina oficial de KeePassXC:** [https://keepassxc.org/](https://keepassxc.org/)  
- **INCIBE:** Gestores de contraseñas: qué son y cómo pueden mejorar la seguridad de las empresas  
  [https://www.incibe.es/protege-tu-empresa/seguridad-en-la-empresa/gestores-de-contrasenas](https://www.incibe.es/protege-tu-empresa/seguridad-en-la-empresa/gestores-de-contrasenas)

---

## Autor i Dades

**Autor:** marc.azañedo  
**Curs:** 2n B  
**Professor/a:** Isabel Bosch  
**Data:** Octubre 2025

