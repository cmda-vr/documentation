## Toolkit
De puzzels, waaronder de eerste opzet van de Escape Room, zijn samengebracht tot een centrale toolkit (website) vanwaar alle 
alle puzzels gemakkelijk opgestart kunnen worden. Dit is een belangrijke requirement vanuit de opdrachtgever. De toepassingen moeten op een centrale plek gehost worden en vanuit één website makkelijk opgestart kunnen worden.

![Prototype Toolkit](/resources/prototype-toolkit.jpg)

Hiervoor maak ik gebruik van [Node.js](https://nodejs.org/en/), [Express](https://expressjs.com/) en [Pug](https://pugjs.org/api/getting-started.html) om de desbetreffende pagina's te renderen en door te linken naar de juiste puzzels. De opzet met Node en Express is vooral gekozen voor de eventuele enhancement van een accountsysteem. De toolkit is alleen bedoelt voor intern gebruik. Een eventuele feature die ik nog graag had willen toevoegen is dat alleen observant met een &samhoud mailadres kunnen inloggen.

[GitHub Repository](https://github.com/samhoudmedia/showcase/blob/master/README.md)

**Tech Stack**  
* [Node.JS](http://nodejs.org) w/
  * [Express](https://expressjs.com) webserver
  * [Pug](https://www.npmjs.com/package/pug) templating
* [Webpack](https://webpack.js.org/) bundle
* [ESLint](https://eslint.org/)
* [EditorConfig](http://editorconfig.org/)

Voor basic styling heb ik op basis van de &samhoud brand styleguide een pattern library gemaakt die de statische .pdf omzet in web componenten. 

[GitHub Repository](https://github.com/samhoudmedia/system-sam)

### Videoregistratie
<iframe width="560" height="315" src="https://www.youtube.com/embed/tyo6ARajhEE" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

## Puzzels

Met de teamrollen van Belbin in het achterhoofd ben ik in eerste instantie aan de slag gegaan met het prototypen van verschillende puzzels.

### Techniek
Zoals eerder benoemd maak ik bijna uitsluitend gebruik van [A-Frame](https://aframe.io/). Voor het registeren van componenten heb ik in eerste instantie een bolierplate opgezet die de applicatie met [Webpack](https://webpack.js.org/) bundled.

**Input**  
Doordat er gebruikt gemaakt gaat worden van drop-in viewers zijn de mogelijkheden qua input beperkt. Bij drop-in viewers zijn er vaak geen game controllers of motion tracking hardware aanwezig. Door deze limitatie is het belangrijk om tijdens het technisch uitwerken rekening te houden met bepaalde interactie patronen (gaze tracking bijvoorbeeld) en vormen van input.

Dit is in lijn met de requirement list, de applicatie optimaliseren voor deze specifieke low-cost hardware componenten en rekening houden met input en motion sickness.

**Tech Stack**  
* [A-Frame](https://aframe.io/)
* [Webpack 4.0](https://www.npmjs.com/package/webpack)
* [Webpack Dev Server](https://github.com/webpack/webpack-dev-server)
* [Webpack HTML Plugin](https://github.com/webpack/webpack-dev-server)
* [ESLint](https://eslint.org/)
* [EditorConfig](http://editorconfig.org/)

## Escape Room

Om de kandidaten meer in groepsverband een case te laten oplossen is er in een later stadium gekozen om de sterke aspecten van alle puzzels samen te voegen tot een (virtuele) Escape Room. Vanwege tijdsgebrek heb ik hier alleen een eerste opzet van kunnen maken. De gebruikte techniek voor de Escape Room is nagenoeg hetzelfe als de voorgaande puzzels.

Het is belangrijk om te benoemen dat m'n Design Challenge NIET de Escape Room is. Het gaat om het inzetten van WebVR tijdens de selectiedag en of dat uberhaupt mogelijk is. De Escape Room is daar EEN VORM van, die ik verder had kunnen en willen uitwerken als er meer tijd was geweest.

## Validatie en Feedback
| Rol | Omschrijving |
|-|-|
| Opdrachtgever | De detail pagina's geven ook voor andere observanten en recruiters een impressie wat het doel is van een bepaalde case |
| Designer | De stijl van de website sluit goed aan bij de styleguide maar hier en daar mis ik wel verfijning in animatie |
| Designer | Door gebruik te maken van de kaarten en afbeeldingen is het makkelijk een impressie te krijgen naar welke case je kijkt, zonder de ondertitels te lezen of naar de detail pagina te gaan |