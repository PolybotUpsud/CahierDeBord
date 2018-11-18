# Construction d'une base robotique

Le projet consiste en la création d'une base robotique general-purpose pour les expérimentations du club. Pour des raisons de coût, nous réutilisons du matériel précédemment acheté par le club dans la mesure du possible.

## Matériel utilisé

 * Carte Arduino Due
 * Moteur pas à pas NEMA17
 * Driver moteur pap à base de Texas Instruments DRV8825
 * Carte de développement maison pour ESP12E/ESP8266
 
## Journal de bord

 * **11/10/2018** : on a fait fonctionner les moteurs pas à pas avec l'Arduino
 * **25/10/2018** : mise en place du GitHub Polybot, essais avec l'ESP8266 pour avoir une console série à distance sur le robot
 * **08/11/2018** : ajout du second moteur, modification du sketch Arduino pour piloter les moteurs avec le périphériques PWM & contrôle à distance avec l'ESP8266
 * **15/11/2018** : usinage d'un premier chassis à partir d'une carcasse d'un lecteur CD, essai des différents modes de pilotage du DRV8825 dans l'optique de limiter la conso électrique, bidouilles (infructueuses) pour fixer des roues au moteurs

## Tâches à réaliser

 * [ ] Plate-forme mécanique
 * [x] Commande des moteurs 0% CPU avec la PWM
 * [x] Pilotage des moteurs à partir de la liason série
 * [ ] Intégration de capteurs
 * [ ] Alimentation électrique autonome du robot
