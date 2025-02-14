---
title: "Troubleshooting Home Assistant: Een reis door interference en dongles"
date: 2025-02-14
author: "Loe Hendriks"
---
Ik ben de afgelopen twee weken meerdere avonden bezig geweest om de home automation problemen van mijn vader op te lossen. Hij belde me een paar dagen geleden op om te vertellen dat zijn lampen niet meer automatisch uit gingen. Dus toen kon ik aan de slag.

Het systeem van mijn vader (dat ik enkele maanden geleden heb geïnstalleerd) draait Home Assistant op een Raspberry Pi met een SSD. Verder zit er een Zigbee Sonoff Dongle Plus-E via een USB verlengkabel verbonden met de Raspberry Pi.

![Photo of Zigbee Sonoff Dongle Plus-E](/images/sonoff.jpg){:width="50%"}

Het eerste wat ik geprobeerd heb is de hele handel power cyclen. Als iemand met een technische achtergrond is dit uiteraard het eerste wat je doet. Dit loste het probleem niet op, dus moest ik gaan zoeken. Het eerste wat ik gecontroleerd heb is vragen of er recentelijk nog nieuwe elektrische apparaten geplaatst zijn in de buurt van deze Raspberry Pi installatie. Want ik dacht, mocht er iets geïnstalleerd zijn dat gebruikmaakt van USB 3.0 dan zou dat zomaar voor interference kunnen zorgen. Dit was niet het geval. Vervolgens heb ik nog gekeken of de antenne van de Sonoff dongle niet verkeerd stond maar dit leek ook niet het geval.

Omdat we bij deze installatie toentertijd voor een vrij korte USB verlengkabel (10cm) gekozen hebben leek het me slim om dit uit te sluiten, Ik heb deze toen vervangen door een kabel van twee meter. Dit zorgde voor vooruitgang! Ik kon de lampen weer bereiken, of ja sommige lampen. Het systeem reageerde nog best vreemd. Alle lampen die ik kon aansturen, reageerden pas na 1 minuut op de trigger die gestuurd werd. Hier was toch meer aan de hand…

Ondertussen was er weer een week voorbij gegaan voordat ik weer de mogelijkheid had om verder te gaan met mijn onderzoek.. Ondertussen heb ik me royaal ingelezen over alle mogelijke oorzaken voor interference. Ik ben na gaan denken over wat de verschillen zijn tussen de Home Assistant installatie bij mijn vader tegenover mijn eigen installatie, want ik heb zelf ook een Home Assistant installatie draaien op een Raspberry Pi met een SSD. Hier waren een paar verschillen: 
Om de SSD met de Raspberry Pi te verbinden heb ik bij mijn vader een SATA naar USB 3 kabel gebruikt omdat dit goedkoper was dan de behuizing die ik zelf gebruik. Ik heb mijn systeem toen uitgezet omdat ik deze behuizing bij mijn vader wilde proberen. Dit loste het probleem niet op. 
De USB kabel die ik zelf thuis gebruikte leek een stuk dikker dan de korte en lange kabel die ik geprobeerd heb bij mijn vader. Mijn gedachtegang hierachter was dat mijn dikkere kabel dan misschien wat betere shielding zou hebben. Dus deze wilde ik ook gaan proberen. Dus kabeltje meegenomen, kabeltjes uitgewisseld, maar nee hoor, dit loste het ook niet op.
Het derde verschil tussen onze installaties was dat mijn installatie niet in mijn meterkast zit maar op mijn kantoor ligt. Dus ik heb geprobeerd alles op een andere plek te plaatsen waar hij verder weg zou liggen van de router die voor interference zou kunnen zorgen maar ook dit was tevergeefs. Zelf niet toen ik 2.4 Ghz op de router uitgezet heb.


Aan het einde van de avond was er meer stuk gemaakt ten opzichte van het oorspronkelijke probleem, er was geen enkel Zigbee apparaat meer te vinden door het systeem…

Toen ben ik er in het weekend nogmaals naar toe gegaan met een aantal ideeën. Ik had een nieuwe Zigbee dongle bij me: de SMLight SLZB-07. Ik ben toen begonnen met de migratie van de oude Sonoff dongle naar de nieuwe. Dit lukte vrijwel zonder problemen (behalve dat de nieuwe dongle alle entiteiten in het Nederlands verwachtte in plaats van in het Engels).

![Photo of SMLight SLZB-07](/images/SLZB-07.png)

Met deze nieuwe dongle kon ik in ieder geval weer alle apparaten bereiken, wel bestond het probleem nog steeds dat het allemaal ontzettend langzaam was. Toen bedacht ik me dat ik laatst met iemand gesproken had die problemen heeft gehad met de apparaten van Ikea die draadloos werken. Mijn volgende stap was als volgt: Ik heb alle apparaten van Ikea uit Home Assistant gehaald en ben deze een voor een weer toe gaan voegen. De lampen kon ik zonder probleem toevoegen en waren daarna ook nog snel aan te sturen. 

Maar, en nu komt de grote onthulling: zodra ik de “Tradfri” schakelaars toevoeg aan het systeem, werd alles direct weer langzaam. Haal ik ze uit het systeem, dan is alles meteen weer snel.

![Photo of SMLight SLZB-07](/images/tradfri.png){:width="50%"}

Het lijkt er dus op dat het probleem tweeledig was, zowel de Sonoff dongle was niet top en de Ikea Tradfri draadloze devices zorgden voor problemen. Nu waren deze Tradfri schakelaars ook nog best lelijk, dus was de oplossing overschakelen op andere draadloze schakelaars. Wij hebben voor de schakelaars van Aqara gekozen.

<em><small>Door: Loe Hendriks</small></em>