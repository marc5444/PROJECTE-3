# 🧾 Explicació de la tasca 06: Fonaments Del Servei DNS

Aquesta pràctica consisteix en utilitzar eines de diagnosi DNS per entendre com es resolen noms de domini i com treballen els servidors DNS.  
L’objectiu és analitzar diferents tipus de consultes i diferenciar entre respostes autoritatives i no autoritatives.

---

## 🔧 Eines utilitzades

- **dig** (Linux / macOS)  
  Utilitzat per fer consultes DNS detallades.

- **nslookup** (Windows / Linux)  
  Permet fer consultes DNS i canviar servidors DNS manualment.

---

## 🧪 Tasques a realitzar

### 1️⃣ Consultes amb `dig`

S’hauran d'executar diverses consultes per analitzar:

| Tipus de registre | Ús |
|-------------------|----|
| A | Obtenir l’adreça IP d’un domini |
| NS | Mostrar els servidors de noms autoritatius |
| SOA | Informació del responsable del domini i número de sèrie |
| PTR (invers) | Obtenir el nom associat a una IP |

**Objectiu:** identificar IP, TTL, servidor que respon i informació del domini.

---

### 2️⃣ Consultes amb `nslookup` en mode interactiu

- Seleccionar el tipus A (`set type=A`)
- Fer consulta del domini i observar si és **no autoritativa**
- Canviar el servidor DNS manualment (`server <IP>`)
- Tornar a fer la consulta per obtenir una resposta **autoritaria**

**Objectiu:** veure la diferència entre respostes cachejades i autoritatives.

---

## 🎯 Objectius d’aprenentatge

- Comprendre el funcionament del DNS
- Distingir entre servidors **autoritaris** i **no autoritaris**
- Identificar i interpretar registres A, NS, SOA i PTR
- Utilitzar `dig` i `nslookup` per diagnosi de xarxa

---

## 🖥️ Requisits

- Màquina Zorin OS amb:
  - NAT
  - Adaptador Pont configurat
- Eines instal·lades: `dig`, `nslookup`

---

> El document explica la pràctica però no inclou els resultats de les comandes.

