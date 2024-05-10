---
title: "Domotica aansturing"
date: 2023-04-17T18:12:01+01:00
weight: 50
---

De veelzijdige [Raspberry Pi](https://www.raspberrypi.com/), vormt het kloppende hart van onze domotica oplossingen. Met deze krachtige en flexibele controller heeft u de controle over alle aspecten van uw woning.

Aangezien de Raspberry Pi uitgebreidt kan worden met een ontelbare hoeveelheid aan hardware en software is de Raspberry Pi de ideale aansturing van uw woning.

![Photo of Raspberry Pi by Harrison Broadbent on Unsplash](/images/harrison-broadbent-hSHNPyND_dU-unsplash.jpg)

# Hardware

In de basis maken wij gebruiken van WiFi en Zigbee voor al onze domotica oplossingen.

## WiFi

Aangezien WiFi in alle woningen reeds beschikbaar is, maakt dit uw woning instapklaar voor vele domotica producten. Waaronder de producten van [Shelly](https://shelly.cloud/) voor het schakelen van al uw inbouw verlichting.

## Zigbee

Wij vertrouwen in Zigbee vanwege de open source eigenschappen. Gezien de 2,4 GHz frequentie kan het interfereren met WiFi. Echter zorgen de slimme Zigbee stopcontacten (smart socket/plugs) ervoor dat het Zigbee mesh netwerk uitgebreid wordt en dekkend is voor uw gehele woning.

De [Deconz Conbee 2 Zigbee stick](https://phoscon.de/en/conbee2) stelt de Raspberry Pi in staat via Zigbee te kunnen communiceren met andere apparaten. Ofwel dit maakt een IKEA, Philips Hue, of andere Zigbee hub overbodig. Alle Zigbee apparaten, ongeacht het merk, zijn aan te sturen via de Raspberry Pi.

## Andere protocollen

Ondersteuning voor andere protocollen zoals Z-wave en Thread is optioneel ook mogelijk.

## Sirene

Indien u kiest voor een alarmsysteem sturen we met behulp van de GPIO van de Pi en een MOSFET de bedrade sirene aan. Met een volume van 110 dB is de sirene niet te missen.

# Software

Bij ons staan Home Assistant en Node-RED aan de basis van uw slimme woning.

## Home Assistant

Home Assistant is volledig open source waarbij lokale controle en privacy voorop staan. Dit platform maakt het mogelijk om alle domotica producten in uw woning samen te voegen in één platform. Het dashboard van Home Assistant is volledig naar uw eigen hand te zetten.

De Home Assistant app is beschikbaar voor iOS en Android.

Lees meer over Home Assistant op [home-assistant.io](https://www.home-assistant.io/).
![Dashboard](/images/dashboard.png)

## Node-RED

De kracht van domotica zit 'm in de automatiserings mogelijkheden. 

Door gebruik te maken van Node-RED kunnen wij maatwerk leveren. Met deze grafische programmeertaal bouwen we automatiseringen op basis van uw specifieke behoeften en wensen, zodat uw thuiservaring precies is zoals u het wilt.
![Automatisering](/images/nodered.webp)

## Tailscale

Ongeacht uw router configuratie, is het mogelijk om te verbinden met uw thuisnetwerk dankzij Tailscale.

Lees meer over hoe Tailscale werkt op [tailscale.com](https://tailscale.com/blog/how-tailscale-works).
