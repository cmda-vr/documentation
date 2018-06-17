# Afbakening

Naar aanleiding van het gedane onderzoek en meerdere gesprekken met de opdrachtgever (&samhoud consultancy)  en opdrachtnemer (&samhoud media) hebben we in overleg een duidelijke afbakening van het project gemaakt. Een afbakening van het uiteindelijke concept en product zorgt voor een specifiekere oplossing en meer focus met duidelijkere taken om actie op te ondernemen.

## Meerwaarde Virtual Reality

### User Engagement
Een Virtual Reality toepassing vergroot over het algemeen de **user engagement**. Doordat de cases een stuk interactiever en visueler zijn gaan mensen eerder op in de ervaring. In de wereld van Virtual Reality wordt dit onderscheden met twee termen'Immersie' ([Frederick P. Brooks](https://www.cs.unc.edu/~brooks/WhatsReal.pdf)) en 'presence' ([Valve, Michael Abrash](http://media.steampowered.com/apps/abrashblog/Abrash%20Dev%20Days%202014.pdf)). 

Een digitale case kan de volgende vormen van immersie vergroten;
* tactische immersie (Ernest W. Adams); wanneer een speler tactische operaties uitvoert die een zekere vaardigheid vergen.
* ruimtelijke immersie (Staffan Bjork); spatiale of ruimtelijke immersie doet zich voor wanneer een speler de gesimuleerde ruimte als perceptueel overtuigend ervaart.

Daarnaast wordt er veel onderzoek gedaan naar welke activiteiten er plaatsvinden in het brein. Uit recent onderzoek ([Zappar, Heather Andrew](https://www.zappar.com/blog/how-augmented-reality-affects-brain/)) bleek nog dat door een AR toepassing de 'visual attention' in het brein vergroot wordt er 70% meer opgeslagen in het geheugen opgeslagen word ten opzichte van tekst op papier.

### Teamrollen en Competenties
Als de kandidaten in groepsverband gaan werken is het voor de observanten interessant om te zien hoe de kandidaten zich gedragen tijdens de ervaring. Door de head-mounted displays kunnen ze alleen door spraak met elkaar communiceren waardoor de teamrollen ([Belbin](http://www.belbin.com/about/belbin-team-roles/)) beter naar voren komen.

### Context
Daarnaast is een credo van &samhoud ['usual unusual'](http://consultancy.samhoud.com/en/about), met recruitment wordt altijd geprobeerd anders te zijn dan de rest. Een VR toepassing tijdens een sollicitatie past dus erg bij deze visie en de strategie om altijd te innoveren in recruitment.

Tijdens zo'n selectiedag is het natuurlijk ook van belang een bepaalde impressie / indruk achter te laten bij de kandidaten over de bedrijfsvoering van de consultancy tak. Kandidaten worden met een interactieve toepassing op een positieve manier verrast en maken kennis met de mogelijkheden van andere business lines binnen de &samhoud group.

### Data
Naast het feit dat de sessie met videocamera's opgenomen kan worden (iets wat nu niet gebeurd) zou het voor de observant een mogelijkheid kunnen zijn om live op een extern scherm mee te kijken met wat de kandidaten in de display zien. Daarnaast is het nog mogelijk om een [reconstructie](https://github.com/dmarcos/aframe-motion-capture-components) (replay) van de sessie te maken door de positie en de input van controllers te [loggen](https://www.npmjs.com/package/aframe-log-component).

Al deze data kan gebruikt worden om volgende selectiedagen te verbeteren, de observanten kunnen zelf zien hoe sessies verlopen zijn en in het vervolg aanpassingen maken, of meer feedback aan de kandidaten bij de [terugkoppeling](https://productbiografie.dandevri.es/research/SCENARIO.html) mee te geven om gerichter aan kandidaten te communiceren waarom ze eventueel door of afgewezen zijn.

## Low-cost hardware
Vanwege de overvloed aan hardware zijn er keuzes gemaakt welke componenten voor deze situatie goed werken. Er wordt gebruikt gemaakt van een klein spectrum aan hardware componenten. De toepassing is geoptimaliseerd voor low-cost components, specifiek de zogeheten drop-in viewers (google cardboards) waarbij een kandidaat de smartphone gebruikt als head-mounted display.

* Cardboards zijn relatief goedkoop, lage opstartkosten
* Lichtgewicht dus makkelijk op te zetten en af te breken tijdens een selectiedag
* Makkelijk om meerdere aan te schaffen voor gebruik in groepsverband
* Portabiliteit, na afloop kunnen kandidaten deze meenemen

Ook na de selectieprocedure op locatie worden de drop-in viewers gebruikt voor een terugkoppeling, de kandidaten kunnen na afloop de drop-in viewer gemakkelijk meenemen.

Voor het project beperken we ons tot drop-in viewers zonder controllers en de magneet als trigger. Er is teveel fragmentatie binnen de soorten drop-in viewers, zoals op de eigen [Google Cardboard specificatie](https://vr.google.com/cardboard/get-cardboard/) site te zien is kun je er niet standaard van uitgaan dat een drop-in viewer de functie van de magneet heeft. Daarnaast zijn de prijzen van cardboard viewers zonder magneet vaak [goedkoper](https://www.alibaba.com/trade/search?fsb=y&IndexArea=product_en&CatId=&SearchText=cardboard+viewer&viewtype=G) waardoor het qua inkoopkosten aantrekkelijk is om ze in wholesale aan te schaffen. De cardboards worden natuurlijk niet hergebruikt maar meegennomen door de kandidaten.

### Techniek
De voordelen van WebVR staan grotendeels beschreven in de [techiek](https://productbiografie.dandevri.es/vr/TECH.html) sectie. De grootste voordelen zijn; 

* Korte opstart: er hoeft geen aparte applicatie geinstalleerd te worden. Het opstarten van een ervaring kan bestaat dus simpelweg uit het bezoeken van url in de browser.
* Cross-platform compabiliteit: de opdrachtgever zit niet verbonden aan specifieke hardware of bestaande platformen.
* Als developer kan ik gebruik maken van de bestaande kennis en infrastructuur die het web te bieden heeft.

## Ethiek
Het recruitment process is vaak een gevoelige tak van sport, je kunt vraagtekens zetten bij het toepassen van een VR ervaring in deze context. &samhoud consultancy vind dit ethisch verantwoord; 'kandidaten zien digitale ervaringen vaak als een positieve verassing en vinden het tevens interessant om te zien wat de mogelijkheden zijn binnen het vakgebied.'

Uiteindelijk zal de beslissing van een selectie altijd door een medewerker (persoon) genomen worden. Het gaat natuurlijk ook om de impressie gedurende de hele dag, niet alleen de virtuele case.