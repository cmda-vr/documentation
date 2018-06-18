# Afbakening

Naar aanleiding van het onderzoek en gesprekken met de opdrachtgever (&samhoud consultancy)  en opdrachtnemer (&samhoud media) hebben we in overleg een duidelijke afbakening van het project gemaakt. Een afbakening van het uiteindelijke concept en product zorgt voor een specifiekere oplossing en meer focus met duidelijkere taken om actie op te ondernemen.

## Meerwaarde Virtual Reality

### User Engagement
Een Virtual Reality toepassing vergroot over het algemeen de **user engagement**. Doordat de cases interactiever en visueler zijn gaan mensen eerder op in de ervaring. In de wereld van Virtual Reality wordt dit onderscheden met twee termen ‘Immersie’ ([Frederick P. Brooks](https://www.cs.unc.edu/~brooks/WhatsReal.pdf)) en ‘presence’ ([Valve, Michael Abrash](http://media.steampowered.com/apps/abrashblog/Abrash%20Dev%20Days%202014.pdf)). 

Een digitale case kan de volgende vormen van immersie vergroten:
* tactische immersie (Ernest W. Adams): wanneer een speler tactische operaties uitvoert die een zekere vaardigheid vergen.
* ruimtelijke immersie (Staffan Bjork): spatiale of ruimtelijke immersie doet zich voor wanneer een speler de gesimuleerde ruimte als perceptueel overtuigend ervaart.

Daarnaast wordt onderzoek gedaan naar welke activiteiten er plaatsvinden in het brein. Uit recent onderzoek ([Zappar, Heather Andrew](https://www.zappar.com/blog/how-augmented-reality-affects-brain/)) bleek dat door een AR toepassing de ‘visual attention’ in het brein vergroot, want er wordt 70% meer opgeslagen in het geheugen ten opzichte van tekst op papier.

Het British Musem heeft in 2015 ([Museums and the Web, 2016](https://mw2016.museumsandtheweb.com/paper/virtual-reality-at-the-british-museum-what-is-the-value-of-virtual-reality-environments-for-learning-by-children-and-young-people-schools-and-families/)) geëxperimenteerd met het inzetten van Virtual Reality om de waarde van dit medium te meten. Wederom was de conclusie dat VR een positieve impact heeft op de reactie en participatie van gebruikers.

### Teamrollen en Competenties
Als kandidaten in groepsverband werken is het voor observanten interessant om te zien hoe kandidaten zich in een groep gedragen tijdens de ervaring. Door de head-mounted displays kunnen ze alleen via spraak met elkaar communiceren waardoor de teamrollen ([Belbin](http://www.belbin.com/about/belbin-team-roles/)) beter naar voren komen.

### Context
Daarnaast is een credo van &samhoud [‘usual unusual’](http://consultancy.samhoud.com/en/about), met recruitment wordt altijd geprobeerd anders te zijn dan de rest. Een VR toepassing tijdens een sollicitatie past bij deze visie en de strategie om altijd te innoveren in recruitment.

Tijdens de selectiedag is het van belang een bepaalde impressie achter te laten bij de kandidaten over de bedrijfsvoering van de consultancy tak. Kandidaten worden met een interactieve toepassing op een positieve manier verrast en maken kennis met de mogelijkheden van andere business lines binnen de &samhoud group.

### Data
Het zou mogelijk kunnen zijn om de sessie met videocamera's op te nemen, iets wat nu niet gebeurd. Ook zou het voor de observant een mogelijkheid kunnen zijn om live op een extern scherm mee te kijken met wat de kandidaten in de head-mounted display zien. Daarnaast is het nog mogelijk om een [reconstructie](https://github.com/dmarcos/aframe-motion-capture-components) (replay) van de sessie te maken door de positie en de input van controllers te [loggen](https://www.npmjs.com/package/aframe-log-component).

Deze data is inzetbaar om toekomstige selectiedagen te verbeteren. De observanten kunnen zelf zien hoe sessies verlopen zijn en in het vervolg aanpassingen maken of meer (gerichter) feedback te geven waarom een kandidaat door of afgewezen is. Bij de [terugkoppeling](https://productbiografie.dandevri.es/research/SCENARIO.html) kunnen ze tevens meer feedback geven.

## Low-cost hardware
Vanwege de verschillende opties met betrekking tot hardware zijn er keuzes gemaakt welke hardware componenten binnen de context van de selectiedag goed werken. De puzzels in de toolkit zijn geoptimaliseerd voor low-cost components, specifiek de zogeheten drop-in viewers (cardboards) waarbij een kandidaat de smartphone gebruikt als head-mounted display.

* Relatief lage opstartkosten: De drop-in viewers gemaakt van karton of plastic hebben lage inkoopkosten waardoor het goedkoop is om meerdere aan te schaffen voor gebruik in groepsverband tijdens de selectiedag.
* Portabiliteit: Vanwege het formaat en het gewicht zijn de drop-in viewers makkelijk na afloop mee te nemen.
* Opstelling: Duurdere hardware kits gaan vaak gepaard met kabels, al met al dus een langere opstarttijd. Drop-in viewers maken alleen gebruik van de smartphone van een kandidaat.

Na de selectieprocedure op locatie worden de drop-in viewers gebruikt voor een terugkoppeling, de kandidaten kunnen na afloop de drop-in viewer gemakkelijk meenemen.

Voor het project beperken we ons tot drop-in viewers zonder controllers en zonder magneet als trigger. Er is teveel fragmentatie binnen de soorten drop-in viewers, zoals te zien is aan het overvloed van drop-in viewers op de [Google Cardboard specificatie](https://vr.google.com/cardboard/get-cardboard/) site. Je kunt er niet standaard van uitgaan dat een drop-in viewer de functie van de magneet heeft. Daarnaast zijn de prijzen van cardboard viewers zonder magneet vaak goedkoper, zie bijvoorbeeld de [prijzen op Alibaba](https://www.alibaba.com/trade/search?fsb=y&IndexArea=product_en&CatId=&SearchText=cardboard+viewer&viewtype=G), waardoor het qua inkoopkosten aantrekkelijk is om ze massaal (whoelsale) aan te schaffen. Omdat de cardboards meegenomen worden door kandidaten, is het nodig om veel producten aan te schaffen. Daardoor is het belangrijk dat de prijs relatief laag is.

### Techniek
De voordelen van WebVR staan beschreven in de [techniek](https://productbiografie.dandevri.es/vr/TECH.html) sectie. In het kort:

* Korte opstart: er hoeft geen aparte applicatie geinstalleerd te worden. Het opstarten van een ervaring kan bestaat dus simpelweg uit het bezoeken van url in de browser.
* Cross-platform compabiliteit: de opdrachtgever zit niet verbonden aan specifieke hardware of bestaande platformen.
* Als developer kan ik gebruik maken van de bestaande kennis en infrastructuur die het web te bieden heeft.

## Ethiek
Het recruitment process is een gevoelig onderdeel, je kunt vraagtekens zetten bij het toepassen van een VR ervaring in deze context. &samhoud consultancy vind dit ethisch verantwoord: *‘kandidaten zien digitale ervaringen vaak als een positieve verassing en vinden het tevens interessant om te zien wat de mogelijkheden zijn binnen het vakgebied’. - Sascha Vloet* Uiteindelijk zal de beslissing van een selectie altijd door een medewerker genomen worden. 