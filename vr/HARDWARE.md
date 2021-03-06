## Hardware voor Virtual Reality
Voor de gemiddelde consument is VR hardware nog maar relatief kort (zie [Oculus Development Kit](https://en.wikipedia.org/wiki/Oculus_Rift#Development_Kit_1)) op de markt. De verschillende soorten VR apparaten focussen elk op andere prijssegmenten en verschillende kenmerken. Tien jaar geleden was het niet geheel ongewoon dat ‘liefhebbers’ verschikkelijk veel geld uitgaven voor dergelijke systemen. Vanaf 2012 (komst Oculus en dus Consumer Grade) lag de prijs rond de €1000,-. Deze prijzen zijn de afgelopen jaren nog verder gedaald, zoals blijkt uit de [Tweakers Pricewatch](https://tweakers.net/pricewatch/480416/htc-vive.html), een [HTC vive head-mounted display](https://www.vive.com/eu/) is al voor €600,- te bestellen.

De meeste VR hardware kits hebben over het algemeen vier componenten ([Tony Parisi, Learning Virtual Reality](http://shop.oreilly.com/product/0636920038467.do)):

* **Stereoscopic displays:** Head-mounted display (HMD), een beeldscherm dat op het hoofd gedragen wordt. Vaak in de vorm van een helm.
* **Motion tracking:** Component dat meet of we ons hoofd of lichaam bewegen. Vaak een combinatie van sensoren in de bril en externe camera's.
* **Input devices:** Een controller, vaak gebasseerd op een game controller. Ook wel motion controllers genoemd.
* **Deskop of Mobiel platform:** Rekenkracht die de applicatie (software) kan uitvoeren.

*Onderstaande afbeeldingen zijn van een [Playstation VR](https://www.playstation.com/en-ae/explore/playstation-vr/) die op het moment voor €300,- vekrijgbaar is.*

**Head-mounted display:**  
Het hoofdingredïent van VR, een beeldscherm dat elke seconde 60 frames genereert aan afbeeldingen. Voor elk oog één afzonderlijk scherm die net iets van elkaar afstaan om de natuurlijke positie van de ogen na te bootsen.

![hardware-1](/resources/hardware-1.jpg)

**Motion Tracking Hardware:**  
Meet de beweging van het hoofd met een *[‘inertial measurement unit’](https://en.wikipedia.org/wiki/Inertial_measurement_unit) (IMU)*. Vaak een combinatie van verschillende meetapparaten, zoals de accelerometer en gyroscope, in veel smartphones te vinden zijn. 

![hardware-2](/resources/hardware-2.jpg)

**Input devices:**  
Omdat de beeldschermen onze ogen bedekken is het niet gemakkelijk om een muis of toetsenbord als input te gebruiken. Vaak hebben verschillende merken hun eigen [game controllers](https://vrscout.com/news/state-of-input-vr-hands/).

![hardware-3](/resources/hardware-3.jpg)

**Computing platforms:**  
Al deze randapparatuur sluiten de gebruikers vaak aan op hardware (computers, smartphones) die de software applicatie draait.

![hardware-4](/resources/hardware-4.jpg)

## Scene
Elke VR omgeving heeft een *‘point of view’ (POV)*: het punt van waar de gebruiker de omgeving bekijkt. 3D systemen gebruiken hiervoor over het algemeen een virtuele camera, een object dat bepaald waar in de scene een gebruiker is gepositioneerd.

In VR moeten we het renderen van de POV dubbel doen, voor elk oog.
* Bepalen positie van de hoofdcamera in de scene.
* Vanaf deze hoofdcamera twee cameras renderen die iets van elkaar afstaan (linker en rechteroog).
* Twee viewports renderen in de head-mounted display.

# Low-cost Virtual Reality

De aanschafprijs van hardware en componenten is voor veel consumenten een vrij grote drempel om overheen te stappen. Met de komst van de *[‘Cardboard’](https://vr.google.com/cardboard/)* is er een hele nieuwe groep consumenten en ontwikkelaars van [VR ervaringen](https://experiments.withgoogle.com/collection/webvr) ontstaan. 

Cardboard refereert naar de techniek waarbij je een bestaande smartphone omzet in een *[‘VR box’](https://www.quora.com/What-is-a-VR-box)*. De smartphone stop je in een *‘drop-in viewer’* waardoor er een head-mounted display ontstaat.

Het is een minder meeslepende ervaring ten opzichte van dure hardware, en veel mensen die al langer met Virtual Reality bezig zijn vinden het een inferieure ervaring ([Tony Parisi, Learning Virtual Reality](http://shop.oreilly.com/product/0636920038467.do)), maar het is voor veel consumenten wel de eerste aanraking met Virtual Reality.

Deze lower-end ervaringen zijn vooral geschikt voor kortere sessies. Door de lagere resolutie van de schermen en een kleinere field of view onstaat er [volgens Chris Hoffman](https://www.howtogeek.com/232520/google-cardboard-lets-you-preview-virtual-reality-but-its-not-all-that-great/) bij veel gebruikers [Motion Sickness](https://designguidelines.withgoogle.com/cardboard/designing-for-google-cardboard/physiological-considerations.html#physiological-considerations-head-tracking).

