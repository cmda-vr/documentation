## Toolkit
De puzzels, waaronder de eerste opzet van de Escape Room, zijn samengebracht tot een centrale toolkit (website) vanwaar alle 
puzzels gemakkelijk opgestart kunnen worden. De toepassingen worden zo op een centrale plek gehost en de puzzels kunnen op deze manier vanuit één website makkelijk opgestart kunnen worden.

![Prototype Toolkit](/resources/prototype-toolkit.jpg)

[Node.js](https://nodejs.org/en/), [Express](https://expressjs.com/) en [Pug](https://pugjs.org/api/getting-started.html) is de tech stack die de desbetreffende pagina's te renderen en doorlinken naar de juiste puzzels. De opzet met Node en Express is vooral gekozen voor de eventuele enhancement van een accountsysteem. De toolkit is alleen bedoelt voor intern gebruik. Een eventuele feature, die ik nog graag had willen toevoegen, is dat alleen observanten met een &samhoud mailadres kunnen inloggen.

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

## Cases

De toolkit bevat alle puzzels die ik gedurende het project heb uitgewerkt als proof of concept.

### Techniek
Zoals eerder benoemd maak ik voor de puzzels uitsluitend gebruik van [A-Frame](https://aframe.io/). Voor het registeren van componenten heb ik in eerste instantie een boilerplate opgezet die de applicatie met [Webpack](https://webpack.js.org/) bundled.

**Tech Stack**  
* [A-Frame](https://aframe.io/)
* [Webpack 4.0](https://www.npmjs.com/package/webpack)
* [Webpack Dev Server](https://github.com/webpack/webpack-dev-server)
* [Webpack HTML Plugin](https://github.com/webpack/webpack-dev-server)
* [ESLint](https://eslint.org/)
* [EditorConfig](http://editorconfig.org/)

### Escape Room

Om de kandidaten meer in groepsverband een case te laten oplossen is er in een later stadium gekozen om de sterke aspecten van alle puzzels samen te voegen tot een (virtuele) Escape Room. Vanwege tijdsgebrek heb ik hier alleen een eerste opzet van kunnen maken. De gebruikte techniek voor de Escape Room is nagenoeg hetzelfe als de voorgaande puzzels.

Het is belangrijk om te benoemen dat m'n Design Challenge NIET de Escape Room is. Het gaat om het inzetten van WebVR tijdens de selectiedag en of dat uberhaupt mogelijk is. De Escape Room is daar EEN VORM van (naast de andere puzzels), die ik verder had willen uitwerken mocht er tijdens het project meer tijd beschikbaar zijn geweest.

## Feedback
| Rol | Omschrijving |
|-|-|
| Sascha Vloet | De detail pagina's geven ook voor andere observanten en recruiters een impressie wat het doel is van een bepaalde case |
| Patrick Philippa | De stijl van de website sluit goed aan bij de styleguide maar hier en daar mis ik wel verfijning in animatie |
| Mitchell Hoogerheide | Door gebruik te maken van de kaarten en afbeeldingen is het makkelijk een impressie te krijgen naar welke case je kijkt, zonder de ondertitels te lezen of naar de detail pagina te gaan |