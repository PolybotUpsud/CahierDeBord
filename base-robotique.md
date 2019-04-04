# Construction d'une base robotique

Le projet consiste en la création d'une base robotique general-purpose pour les expérimentations du club. Pour des raisons de coût, nous réutilisons du matériel précédemment acheté par le club dans la mesure du possible.

## Matériel utilisé

 * Carte Arduino Due
 * Moteur pas à pas NEMA17
 * Driver moteur pap à base de Texas Instruments DRV8825
 * Carte de développement maison pour ESP12E/ESP8266
 
## Liste Materiel a acheter
- Batterie mobile (2A, 5V) ([Amazon](https://www.amazon.fr/AUKEY-Batterie-Power-Bank-Lightning-Samsung-S8/dp/B017KCFUZA/ref=sr_1_6?ie=UTF8&qid=1543504031&sr=8-6&keywords=batterie+usb))
- Chargeur batterie ([Amazon](https://www.amazon.fr/dp/B07C91WFJG/ref=twister_B07D2BVN4T?_encoding=UTF8&th=1))
- Convertisseurs de puissance 5V & 3V3 ([eBay](https://www.ebay.fr/itm/LM2596S-LM2596-Step-down-Regulateur-de-tension-reglable-5V-12V-24V-1235A/183478544621?_trkparms=aid%3D555017%26algo%3DPL.CASSINI%26ao%3D1%26asc%3D20180221161529%26meid%3Dc51a7cd6ebeb478390f2a8aee46a99c6%26pid%3D100506%26rk%3D1%26rkt%3D1%26%26itm%3D183478544621&_trksid=p2045573.c100506.m3226))
- Vis pololu
- Jumper Breadboard & breadboard ([GoTronic](https://www.gotronic.fr/art-kit-plaque-de-montage-sd80a-25864.htm))
- Assortiment R/C THT ([Résistances, GoTronic](https://www.gotronic.fr/art-assortiment-de-1000-resistances-1-4w-2615.htm) - [Condensateurs, GoTronic](https://www.gotronic.fr/art-assortiment-de-condensateurs-chimiques-3162.htm))
- Connecteur Banane ([GoTronic](https://www.gotronic.fr/art-douille-banane-3266n-15399.htm))
- Plaque de prototypage, au moins 5 pcs ([GoTronic, référence EE80120](https://www.gotronic.fr/cat-plaques-d-essais-1472.htm))
 
## Journal de bord

 * **11/10/2018** : on a fait fonctionner les moteurs pas à pas avec l'Arduino
 * **25/10/2018** : mise en place du GitHub Polybot, essais avec l'ESP8266 pour avoir une console série à distance sur le robot
 * **08/11/2018** : ajout du second moteur, modification du sketch Arduino pour piloter les moteurs avec le périphériques PWM & contrôle à distance avec l'ESP8266
 * **15/11/2018** : usinage d'un premier chassis à partir d'une carcasse d'un lecteur CD, essai des différents modes de pilotage du DRV8825 dans l'optique de limiter la conso électrique, bidouilles (infructueuses) pour fixer des roues au moteurs
 * **22/11/2018** : 
 * **29/11/2018** : Ajout de capacités de découplage sur les drivers de moteurs, toujours des problèmes de courant sur les moteurs PAP (passer sur des moteurs DC ?), prévision budget 2019, essai batterie LiPo 11.1v (elle semble OK)
 * **06/12/2018** : Budget FSDIE, tentative supplémentaire de debug des drivers moteurs PAP
 * **13/12/2018** : Travail sur l'interface de pilotage avec Qt, module capteur de proximité IR, modélisation base
 * **7/02/2019** : Mise en place d'une mailing list, suite de la modelisation 3d et pont en H.
 * **14/02/2019** : Déballage du robot-aspirateur, vérification du bon fonctionnement (commande a la télécommande). Travail sur le modele 3d de la voiture télécommandée.
 * **21/02/2019** : Reprogrammation du robot-aspirateur, controle avec succès des moteurs et des LEDs avant, finalisation du modele 3d de la voiture (imprimante non dispo).
 * **.../03/2019** :
 * **4/04/2019** :

## Tâches à réaliser

 * [ ] Plate-forme mécanique
 * [x] Commande des moteurs 0% CPU avec la PWM
 * [x] Pilotage des moteurs à partir de la liason série
 * [ ] Intégration de capteurs
 * [ ] Alimentation électrique autonome du robot
