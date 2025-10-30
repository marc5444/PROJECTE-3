# 🧾 Explicació de la tasca: Diagnosi de Noms DNS

Aquesta pràctica tracta sobre l'ús d'eines de línia de comandes per
analitzar i diagnosticar el funcionament del sistema DNS en diferents
sistemes operatius.\
L'objectiu és entendre com es converteixen noms de domini en adreces IP,
quins servidors intervenen i quina informació ofereixen les eines DNS.

------------------------------------------------------------------------

## 🔧 Eines utilitzades

-   **`dig`** (Linux / macOS) --- eina avançada per consultes DNS
-   **`nslookup`** (Windows / Linux) --- eina per fer consultes DNS i
    canviar servidors

------------------------------------------------------------------------

## 🧪 Tasques a realitzar

### 1️⃣ Diagnosi amb `dig`

Es faran diverses consultes per obtenir i analitzar:

  -----------------------------------------------------------------------
  Tipus de consulta                              Objectiu
  ---------------------------------------------- ------------------------
  Registre **A**                                 Obtenir la IP d'un
                                                 domini

  Registres **NS**                               Saber quins són els
                                                 servidors de noms del
                                                 domini

  Registre **SOA**                               Informació
                                                 administrativa
                                                 (responsable, número de
                                                 sèrie, etc.)

  Resolució inversa (**PTR**)                    Obtenir el nom associat
                                                 a una IP
  -----------------------------------------------------------------------

Cal analitzar elements com: IP de resposta, TTL, servidor que ha
respost, etc.

------------------------------------------------------------------------

### 2️⃣ Diagnosi amb `nslookup` (mode interactiu)

-   Seleccionar tipus de consulta (**A**)
-   Fer una consulta i observar si és **autoritària** o **no
    autoritària**
-   Canviar manualment el servidor DNS amb `server IP`
-   Tornar a fer la consulta i comparar els resultats

------------------------------------------------------------------------

## 🎯 Objectius d'aprenentatge

✅ Comprendre el funcionament del DNS\
✅ Distingir entre respostes **autoritàries** i **no autoritàries**\
✅ Interpretar registres DNS bàsics: A, NS, SOA, PTR\
✅ Fer diagnosi de noms amb `dig` i `nslookup`

------------------------------------------------------------------------

## 🖥️ Requisits tècnics

-   Sistema Zorin OS amb:
    -   NAT + Adaptador Pont
-   Eines instal·lades: `dig`, `nslookup`

------------------------------------------------------------------------

> Aquest document descriu la tasca, però no inclou les execucions ni
> resultats reals.
