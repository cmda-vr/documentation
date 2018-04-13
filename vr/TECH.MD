# Virtual Reality op het Web
Vrijwel alle applicaties die draaien op dure hardware zijn zogeheten *'native'* applicaties die specifiek voor een bepaald platform worden gemaakt. 

Naast een native applicatie is het mogelijk om een Virtual Reality applicatie te maken die draait in een browser. Dit heeft voor zowel gebruikers en ontwikkelaars voordelen. 

Het doel van WebVR is om het voor zowel ontwikkelaars als gebruikers toegankelijker (drempelvrij) te maken om Virtual Reality te ervaren. Ongeacht de devices en input die ze tot hun beschikking hebben.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Jzrqrji_2xk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Implementation

Na de aankoop van Oculus VR door Facebook begon Mozilla te werken aan een implementatie hiervan in Browsers. WebVR was geboren.

## Gebruikers
Voor gebruikers is het een stuk toegankelijker om VR te ervaren.

* **Korte opstart:** er hoeft geen aparte applicatie geinstalleerd te worden. Het opstarten van een ervaring kan dus simpelweg om naar een link te gaan in de browser.
* **Cross-platform compabiliteit:** je zit niet verbonden aan specifieke hardware of bestaande platformen.
* **Kosten hardware:** een gebruiker kan in veel gevallen met bestaande hardware (smartphone) VR ervaren

## Ontwikkelaars
Voor ontwikkelaars is het ook een stuk toegankelijker geworden om een VR applicatie op het web te ontwikkelen. 

* **Huidige infrastructuur:** we maken gebruik van bestaande Web Technieken waardoor we veel van bestaande infrastructuur (die het web ons biedt) kunnnen gebruiken. Denk bijvoorbeeld aan het toevoegen van data uit andere webbronnnen of gebruik maken van *open-source tools en frameworks*.
* **Snellere livegang:** de applicatie kan costant worden geupdate met de bestaande links zonder dat dit via een App Store moet.
* **Cross-platform compabiliteit:** je hoeft niet te ontwikkelen voor een specifiek operating system of hardware device. De applicatie draait in een web browser.

### Technische obstakels
* **Browser vendors:** willen het onderling nog wel eens oneens zijn met implementaties van een bepaalde techniek. Bij WebVR is dit niet anders, niet elke browser ondersteund in dezelfde mate de WebVR techniek. Deze scope zal dus ook aangepast moeten worden naar de browsers de eindgebruikers zullen gebruiken.
* **Performance:** Een applicatie is mede afhankelijk van omgevingsfactoren, bijvoorbeeld de snelheid van een internetverbinding op dat moment.
* **Progressive Enhancement:** Vanwege de verschillende manieren van input die een gebruiker kan hebben zou ik eerst moeten aftasten (detecteren) wat voor soort input een gebruiker kan geven.

Elke front-end developer zou (met behulp van frameworks) een VR applicatie op het web kunnen ontwikkelen.