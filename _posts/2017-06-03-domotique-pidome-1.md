---
layout: post
title:  "PiDome & MySensors & Compteur EDF"
date:   2017-06-03 18:00
categories: DIY Arduino Domotique
---


![Pidome - Compteur Wh](/images/pidome2.png)

# Présentation
## Pidome

[PiDome](http://pidome.org) est une plateforme domotique open source développé pour le Raspberry Pi. Personnellement j'utilise un Raspberry Pi 3 (60€ tout compris).
J'ai choisi PiDome parmi tant d'autres (Domoticz, OpenHAB,...) pour son interface récente et jolie, le fait qu'il tourne sur Raspi et qu'il soit compatible avec MySensors.

## MySensors

[MySensors](https://www.mysensors.org/) est une plateforme logicielle permettant de créer des objets connectés avec des Arduino, Raspi et sans fil (NRF24, ESP8266,...).


## Compteur EDF

Pour récupérer les informations du compteur EDF, j'utilise une photorésistance positionnée en face de la LED clignotante sur le compteur.
Avec un LM355 monté en comparateur, j'utilise une interruption sur l'arduino pour calculer le temps entre chaque clignotement.

En sachant que je consomme 1Wh/blink, si il y a une seconde entre deux blink, cela me fait une consommation instantanée de 3600W, une minute égal 60W, une heure égal 1W...

Pour mes graphiques, je relève ma consommation toute les minutes.

# Dans la pratique

## Installer PiDome
