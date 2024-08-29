---
title: "Onze domotica aansturing"
date: 2023-04-17T18:12:01+01:00
---

De veelzijdige [Raspberry Pi](https://www.raspberrypi.com/) - een mini computer, vormt het kloppende hart van onze domotica oplossingen. Met deze krachtige en flexibele controller heeft u de controle over alle aspecten van uw woning.

Aangezien de Raspberry Pi uitgebreidt kan worden met een ontelbare hoeveelheid aan hardware en software is de Raspberry Pi de ideale aansturing van uw woning.

![Photo of Raspberry Pi by Harrison Broadbent on Unsplash](/images/harrison-broadbent-hSHNPyND_dU-unsplash.jpg)

Door gebruik te maken van de Raspberry Pi kunnen we koppelen met alle populaire bestaande apparaten zoals die van IKEA, Sonos, Philips Hue, Somfy, Fibaro en vele andere merken. 

# Hardware

In de basis maken wij gebruiken van WiFi en Zigbee voor al onze domotica oplossingen.

## WiFi

Aangezien WiFi in alle woningen reeds beschikbaar is, maakt dit uw woning instapklaar voor vele domotica producten. Waaronder de producten van [Shelly](https://shelly.cloud/) voor het schakelen van al uw inbouw verlichting.

## Zigbee

Wij vertrouwen in Zigbee vanwege de open source en mesh netwerk eigenschappen. Onze Zigbee smart sockets zorgen ervoor dat het mesh netwerk uitgebreid wordt en dekkend is voor alle sensoren in uw gehele woning.

De [Deconz Conbee 2 Zigbee stick](https://phoscon.de/en/conbee2) stelt de Raspberry Pi in staat via Zigbee te communiceren met andere apparaten. Dit maakt een IKEA, Philips Hue, of andere Zigbee hubs overbodig. Alle Zigbee apparaten, ongeacht het merk, zijn aan te sturen met onze domotica oplossing.

## Andere protocollen

Ondersteuning voor andere protocollen zoals Z-wave en Thread is optioneel ook mogelijk.

## Sirene

Indien u kiest voor een alarmsysteem sturen we met behulp van de Raspberry Pi de bedrade sirene aan. Met een volume van 110 dB is de sirene niet te missen. Optioneel is het ook mogelijk om te kiezen voor een draadloze sirene.

# Software

Bij ons staan Home Assistant en Node-RED aan de basis van uw slimme woning.

## Home Assistant

Home Assistant is volledig open source waarbij lokale controle en privacy voorop staan. Dit platform maakt het mogelijk om alle domotica producten in uw woning samen te voegen in één platform. Het dashboard van Home Assistant is volledig naar uw eigen hand te zetten.

De Home Assistant app is gratis beschikbaar voor iOS en Android.

Lees meer over Home Assistant op [home-assistant.io](https://www.home-assistant.io/).
![Dashboard](/images/dashboard.png)

## Node-RED

De kracht van domotica zit 'm in de automatiserings mogelijkheden. 

Door gebruik te maken van [Node-RED](https://nodered.org/) kunnen wij maatwerk leveren. Met deze grafische programmeertaal bouwen we automatiseringen op basis van uw specifieke behoeften en wensen, zodat uw thuiservaring precies is zoals u het wilt.
![Automatisering](/images/nodered.webp)

Enerzijds werken wij met standaard, herbruikbare bouwblokken. Waaronder de automatisering voor het alarmsysteem. Anderzijds bouwen wij volledig op maat gemaakte automatiserings scenario's, want iedereen zijn wensen zijn uniek.

## Cloudflare

Ongeacht uw router configuratie, is het mogelijk om te verbinden met Home Assistant op uw thuisnetwerk dankzij Cloudflare.

Lees meer over hoe Cloudflare werkt op [cloudflare.com](https://www.cloudflare.com/).

{% include call.html show_button=true %}