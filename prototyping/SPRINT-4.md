# Sprint 4 - Toolkit

**Week 15**

Na het uitwerken van de 360-video's ben ik verdergegaan met de grootste feedback vanuit de vorige iteratie: *de puzzels moeten vanaf een centrale plek worden opgestart.* Met verschillende telefoons handmatig URL’s invoeren kan maar is niet de meest efficiënte manier. Het was voor de observanten van &samhoud dus belangrijk dat de cases vanuit een centrale plek opgestart konden worden. De toolkit dient als website die doorlink naar de puzzels die gemaakt zijn bij de tweede sprint. De toolkit geeft op een makkelijke manier toegang tot de puzzels.

## Visuele stijl
Intern is er een styleguide maar als statische .pdf vorm. Om de huisstijl van &samhoud makkelijker digitaal te gebruik heb ik een digitale pattern library gemaakt zodat ik deze in de toolkit kon hergebruiken.

De `src` folder bevat alle algemene styling zoals typografie, kleur en animatie als `sass partials`. Deze importeer ik en build ik met NPM scripts. Dit zorgt uiteindelijk voor een `main.css` in de `build` folder die gemakkelijk in de head van een html pagina kan worden gezet. Je zou deze als statische file op een server kunnen zetten, voor de toolkit gebruik ik `rawgit` als cdn. 

De prototypes van de puzzel staan op GitHub, door een build branch aan te maken en als statische files te builden met Webpack kan ik deze gemakkelijk serveren via GH-pages.