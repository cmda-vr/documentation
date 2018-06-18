# Sprint 4 - Toolkit

**Week 15**

Na het uitwerken van de 360-video's ben ik verder gegaan met de voornaamste feedback vanuit de vorige iteratie: *de puzzels moeten vanaf een centrale plek worden opgestart.* Met verschillende telefoons handmatig URL’s invoeren kan maar is niet de meest efficiënte manier. Het was voor de observanten belangrijk dat de cases vanuit een centrale plek opgestart konden worden. De toolkit dient als website die doorlinkt naar de puzzels die gemaakt zijn bij de tweede sprint.

## Visuele stijl
Intern is er een styleguide maar als statische PDF vorm. Om de huisstijl van &samhoud makkelijker digitaal te gebruiken heb ik een digitale [pattern library](https://github.com/samhoudmedia/system-sam) gemaakt zodat ik deze in de toolkit kon hergebruiken.

De `src` folder bevat alle algemene styling zoals typografie, kleur en animatie als `sass partials`. Deze importeer ik en build ik met npm scripts. Elk component word in een apart bestand geschreven maar samengevoegd door een `build tool`. Dit werken in componeten zorgt ervoor dat het toevoegen van componenten in de toekomst makkelijk gaat, de opzet is op deze manier schaalbaar. Dit zorgt uiteindelijk voor een `main.css` in de `build` folder die gemakkelijk in de head van een html pagina kan worden gezet. Developers bij &samhoud kan deze vervolgens als statische file op een server kunnen zetten, voor de toolkit gebruik ik `rawgit` als cdn. 

De prototypes van alle puzzels staan op GitHub, door een [build branch](https://github.com/samhoudmedia/puzzle-room-prototypes/tree/gh-pages) aan te maken en als statische files te builden met Webpack kan ik deze gemakkelijk serveren via GH-pages.

## Feedback volgende Iteratie

| Feedback opdrachtgever | 
|-|
| ‘Er mist een detailscherm zodat andere observanten van &consultancy weten waar de cases over gaan.‘ | 