# Capteur d'enneigement ❄️🌨️

<div align="center">
  <picture>

  <source 
      media="(prefers-color-scheme: dark)" 
      srcset="https://github.com/lorenzor0912/Projet-IT-Neige/blob/0a817e1d05e45fb6e63a99a292cdd9ac2ce48b34/ReadMe_IMG/It%20neige.svg" />
    
  <img 
      src="https://github.com/lorenzor0912/Projet-IT-Neige/blob/0a817e1d05e45fb6e63a99a292cdd9ac2ce48b34/ReadMe_IMG/It%20neige.svg" 
      alt="Logo principal" 
      width="400" 
      height="400" />
  </picture>
</div>


## Table des matières 📖

- [Hardware 🛠️](#hardware)
  - [Capteur 📸](#capteur)
  - [Carte 📺](#carte)
  - [Communications 📡](#communications)
  - [Stockage 💾](#Stockage)
  - [Batterie 🔋](#Batterie)
  - [Fonction Webcam Possible ? 🎥](#Webcam)
  - [Matériaux](#Matériaux)
- [Software 🦠](#hardware) 

## Hardware 🛠️

### Capteur

SEN0313 par DF Robot aussi connu sous A01NYUB (identique) [DF Robot](https://www.dfrobot.com/product-1934.html)

<details>

<summary>Specifications Techniques</summary>


- Type : Capteur de distance ultrasonique étanche (waterproof & dustproof, IP67)

- Etanchéité : cretification IP67

- Courant : <15mA 

- Plage de mesure : 28 cm à 750 cm (soit jusqu'à 7,5 mètres)

- Resolution : 1cm 

- Interface de communication : UART (série asynchrone, très simple à utiliser)

- Tension d'alimentation : 3,3 V à 5 V (compatible Arduino, Raspberry Pi, etc.)

- Sortie : Valeur de distance directement disponible en UART (pas besoin de calculer le temps de vol soi-même)

- Autres points forts :

  - Livré avec un cône (bell mouth) amovible pour optimiser la portée et la directivité
  - Résistant à la poussière, au brouillard, à la fumée (meilleure pénétration que les HC-SR04 classiques)

</details>


![Image Alt](https://github.com/lorenzor0912/Projet-IT-Neige/blob/f1702dfe2ce56fabe681698466927644a630968b/ReadMe_IMG/SEN0313.JPG)

### Carte

All in One (Esp seulement)




### Communications

- Via 4g
- possibitlité et intéret pour relais/émetteur [meshtastic](https://meshtastic.org/) ???
- Possibilité LoRaWan

### Stockage

Sachant que nos deux microcontrolleurs (qui représente le choix le plus economique puissant et logique) ont tous deux un port de carte sd il ne faut plus que coder et avoir une carte sd!

Estimation d'espace necessaire :

- On sait que:
  - le système doit tenir 4 mois
  - toute 30 sec estimation sur 3 mois de 552 Ko

**Carte SD Haute endurance**

  - [Sd Sandisk Industrial XI 8Go de 85° a -40 13€ ](https://www.mouser.fr/ProductDetail/SanDisk/SDSDQAF3-008G-XI?qs=F5EMLAvA7IAdyu9puKxNsg%3D%3D)
  - SanDisk High Endurance microSDXC
  - Lexar microSDHC/microSDXC UHS-I High Endurance Card
  - Samsung PRO Endurance microSDXC UHS-I U3
  - PNY Pro Elite™ High Endurance C10 U3 V30 A2 MicroSDXC Memory Card
  - Kingston High Endurance microSDXC95R
  - Micro SD KIOXIA EXCERIA High Endurance UHS-I C10 R98





---
### Batterie

Estimation de 






---

### Webcam

certains carte all in one on meme des mini camera (par ex waveshare) donc peut se reveler interessant

[Waveshare Demo](https://www.youtube.com/watch?v=z_u_RoW-mEs)

![Image Alt](https://github.com/lorenzor0912/Projet-IT-Neige/blob/d28ecf070d6103b8d8a0e5f1bddaf87ee4db1f34/ReadMe_IMG/Waveshare%20Cam.jpg)




---


### Matériaux




---

### Comparaison filaments extrêmes : -30°C / 10 ans neige/UV/humidité ❄️⛄

| Critère                              | ASA-CF       | PETG-CF      | PET          | ABS          | PLA          | ASA (std)    | PC           | PETG (std)   | Nylon (PA)   |
|--------------------------------------|--------------|--------------|--------------|--------------|--------------|--------------|--------------|--------------|--------------|
| Résiste bien à -30°C (pas cassant)   | ✅✅         | ✅✅         | ✅           | ✅           | ❌❌         | ✅✅         | ✅✅ (souplissime) | ✅✅         | ✅✅ (flexible) |
| Durée 10 ans UV + intempéries/neige  | ✅✅ (UV top + CF boost) | ✅ (bon UV, CF aide) | ❌ (dégrade) | ❌ (jaunit/craque) | ❌❌ (détruit vite) | ✅✅ (UV leader) | ✅ (bon, mais moins UV) | ❌ (jaunit après années) | ❌ / ✅ (si PA12, bon si protégé) |
| Étanchéité / neige & humidité        | ✅✅ (~0.3-0.5% absorption) | ✅✅ (hydrophobe) | ✅           | ✅           | ❌ (gonfle)  | ✅           | ✅ (mais hygro) | ✅✅ (très hydrophobe) | ❌ (absorbe beaucoup, sauf PA12) |
| Reste étanche/dimension stable longtemps | ✅✅         | ✅✅         | ✅           | ✅ (shrink)  | ❌           | ✅✅         | ✅           | ✅✅         | ❌ (sauf PA12) |
| Facile à imprimer                    | ❌ (boîtier + nozzle hard) | ❌ (abrasif) | ✅           | ❌ (warping) | ✅✅ (facile) | ❌ (boîtier) | ❌❌ (dur)   | ✅✅ (facile) | ❌ (séchage + boîtier) |
| Rigidité / résistance chocs au froid | ✅✅ (très rigide) | ✅✅ (boost CF) | ✅           | ✅           | ✅ / ❌ (cassant) | ✅           | ✅✅ (top chocs) | ✅           | ✅✅ (abrasion + flex) |

**Verdict rapide pour ton usage (-30°C, neige, 10 ans dehors)**  
✅ **ASA-CF** → Le gagnant global : UV imbattable (10+ ans dehors sans jaunir/craquer), faible absorption humidité, tient -30°C sans casser, rigidité boostée par CF. Idéal pour pièces exposées neige/soleil (ex: boîtiers, supports extérieurs).  

✅ **PETG-CF** → Très bon compromis : super hydrophobe (ne gonfle pas en neige), flexible au froid, UV correct (mieux que PETG std), facile relatif. Moins cher/simple que ASA-CF.  

✅ **PC** → Si priorises chocs violents au froid extrême (reste souple, pas cassant).  

✅ **ASA (std)** → Si pas besoin de CF ultra-rigide, c'est le roi UV/long terme sans complications.  

❌ **PLA / ABS / PET** → À éviter pour 10 ans dehors ou froid extrême (cassent/jaunissent/dégradent).  

❌ **Nylon** → OK si PA12 (faible humidité), sinon absorbe trop l'eau en neige → gonfle/déforme.  

Pour max étanchéité/UV sur 10 ans, coating époxy ou peinture UV après impression. ASA-CF + coating = quasi-indestructible en environnement neigeux !


<div style="line-height: 0.9; font-family: 'Courier New', Courier, monospace; white-space: pre; color: #d0d0d0;">
<pre>
   _____ _   _ ___  _____    _           _         
  / ____| | (_)__ \|  __ \  | |         | |        
 | (___ | |_ _   ) | |  | | | |     __ _| |__  ___ 
  \___ \| __| | / /| |  | | | |    / _` | '_ \/ __|
  ____) | |_| |/ /_| |__| | | |___| (_| | |_) \__ \
 |_____/ \__|_|____|_____/  |______\__,_|_.__/|___/
                                                   
                                                   
</pre>
</div>

 <img 
      src="https://github.com/Lorenzo-x64/Projet-IT-Neige/blob/a68dd4287c40711deb7713e88d299c58865ecca4/ReadMe_IMG/Sti%20Labs.svg" 
      alt="Logo principal" 
      width="600" 
      height="600" />

<div align="right">
  <a href="#top">↑ Retour en haut</a>
</div>
