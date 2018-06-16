# Virtual Reality op het Web
Vrijwel alle applicaties die draaien op [dure hardware](https://www.vive.com/eu/product/vive-pro/) zijn zogeheten *'native'* applicaties die specifiek voor een bepaald platform worden gemaakt. Naast een native applicatie is het mogelijk om een Virtual Reality applicatie te maken die draait in een browser. Dit heeft voor zowel de gebruikers van de applicatie en ontwikkelaars voordelen. 

> Het doel van WebVR is om het voor zowel ontwikkelaars als gebruikers toegankelijker (drempelvrij) te maken om Virtual Reality te ervaren. Ongeacht de devices en input die ze tot hun beschikking hebben.

<iframe width="560" height="315" src="https://www.youtube.com/embed/Jzrqrji_2xk" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Gebruikers
Voor gebruikers is het, door de komst van VR op het web ten opzichte van specifieke native en/of software applicaties, een stuk toegankelijker om VR te ervaren ([Tony Parisi, Learning Virtual Reality](http://shop.oreilly.com/product/0636920038467.do)).

* **Korte opstart:** er hoeft geen aparte applicatie geïnstalleerd te worden. Het opstarten van een ervaring kan dus simpelweg door naar een link te gaan in de browser.
* **Cross-platform compabiliteit:** je bent niet afhankelijk van specifieke hardware of een bestaand platform.
* **Kosten hardware:** een gebruiker kan in veel gevallen met bestaande hardware (smartphone) VR ervaren en hoeft voor een basis ervaring geen duurdere hardware kit (oculus, htc) aan te schaffen.

## Ontwikkelaars
Voor ontwikkelaars is het ook een stuk toegankelijker geworden om een VR applicatie op het web te ontwikkelen ([Venturebeat, Amir Bozorgzadeh](https://venturebeat.com/2017/03/18/webvr-isnt-sexy-but-it-will-change-the-game-for-vr-this-year/)). 

* **Huidige infrastructuur:** we maken gebruik van bestaande Web Technieken waardoor we veel van [bestaande infrastructuur](https://aframe.io/docs/0.8.0/introduction/javascript-events-dom-apis.html) (die het web ons biedt) kunnnen gebruiken. Denk bijvoorbeeld aan het toevoegen van data uit andere webbronnen of gebruik maken van *[open-source tools en frameworks](https://github.com/wizztjh/awesome-WebVR)*.
* **Snellere livegang:** de applicatie kan constant worden geüpdatet met de bestaande links zonder dat dit via een App Store moet.
* **Cross-platform compabiliteit:** je hoeft niet te ontwikkelen voor een specifiek operating system of hardware device. De applicatie draait in een web browser.

### Technische obstakels
* **Browser vendors:** willen het onderling nog wel eens oneens zijn met [implementaties](https://webvr.rocks/) van een bepaalde techniek. Bij WebVR is dit niet anders, niet elke browser ondersteunt in dezelfde mate de WebVR techniek. Deze [scope](https://webvr.info/developers/) zal dus ook aangepast moeten worden naar de browsers die eindgebruikers zullen gebruiken.
* **Performance:** een applicatie is mede afhankelijk van omgevingsfactoren, bijvoorbeeld de snelheid van een internetverbinding op dat moment.
* **Progressive Enhancement:** vanwege de verschillende manieren van input die een gebruiker kan hebben is het verstandig eerst te detecteren welke input een gebruiker tot zijn beschikking heeft.

Elke front-end developer zou (met behulp van frameworks) een VR applicatie op het web kunnen ontwikkelen.

## Implementatie

Na de aankoop van [Oculus VR door Facebook](https://www.theguardian.com/technology/2014/mar/25/facebook-buys-virtual-reality-gaming-firm-oculus) begon [Mozilla](https://mixedreality.mozilla.org/) te werken aan een implementatie hiervan in Browsers, de [WebVR API](https://immersive-web.github.io/webvr/) was geboren. Hiermee was het mogelijk om verschillende VR devices te detecteren en 3D scene's te renderen.

Deze API biedt een ontwikkelaar alle functionaliteit die nodig is om een VR applicatie in de browser te programmeren. Op basis daarvan zijn er verschillende ['frameworks'](https://createwebvr.com/) gebouwd. Deze frameworks abstraheren de onderliggende techniek nog verder waardoor de drempel voor een ontwikkelaar extreem laag ligt.