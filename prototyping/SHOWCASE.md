# ~~show~~case

Om de kandidaten in groepsverband een puzzel te laten oplossen is er gekozen voor een Escape Room achtig concept. Deze leent communicatieve element vanuit televisie spelshows en analytische patronen vanuit de game wereld.

## Escape Room

### Flow
Het scenario is relatief simpel. Tijdens de selectiedag betreden de kandidaten een ruimte zonder enige vorm van instructie. Voor hun ligt een houten kist met een cijferslot en een viertal drop-in viewers. Ze werken aan het gezamenlijke doel om de houten kist open te krijgen. 

Zodra ze de head-mounted display opzetten begeven alle vier de kandidaten zich in een virtuele ruimte. Dit lijken in eerste instantie dezelfde kamers maar iedere kandidaat ziet net andere details. Denk bijvoorbeeld aan een boekenkast waar, bij elke kandidaat, een aantal andere kleur boeken inzitten. Deze subtiele verschillen zijn gelijk hints naar de code voor het cijferslot.

> Je kijkt naar beneden en ziet dat jouw avatar rode schoenen heeft, bij een andere kandidaat staan er in  de boekenast vier rode boeken. Jouw persoonlijke cijfer is in dit geval 4.

De kandidaten kunnen niet in elkaars kamer kijken en mogen de VR bril niet afzetten tijdens hun sessie waardoor ze alleen met spraak met elkaar kunnen communiceren.

### Techniek
Zoals eerder benoemd maak ik bijna uitsluitend gebruik van [A-Frame](https://aframe.io/). Voor het registeren van componenten heb ik in eerste instantie een bolierplate opgezet die de applicatie met [Webpack](https://webpack.js.org/) bundled.

**Tech Stack**  
* [A-Frame](https://aframe.io/)
* [Webpack 4.0](https://www.npmjs.com/package/webpack)
* [Webpack Dev Server](https://github.com/webpack/webpack-dev-server)
* [Webpack HTML Plugin](https://github.com/webpack/webpack-dev-server)
* [ESLint](https://eslint.org/)
* [EditorConfig](http://editorconfig.org/)

## Toolkit
Het is voor de observant belangrijk dat de applicatie(s) snel en gemakkelijk zijn op te starten. Hiervoor heb ik een centrale toolkit (website) gemaakt vanwaar alle puzzels opgestart kunnen worden.

Hiervoor maak ik gebruik van [Node.js](), [Express]() en [Pug]() om de desbetreffende pagina's te renderen en door te linken naar de juiste puzzels.

[GitHub Repository](https://github.com/samhoudmedia/showcase/blob/master/README.md)

**Tech Stack**  
* [Node.JS](http://nodejs.org) w/
  * [Express](https://expressjs.com) webserver
  * [Pug](https://www.npmjs.com/package/pug) templating
* [Webpack](https://webpack.js.org/) bundle
* [ESLint](https://eslint.org/)
* [EditorConfig](http://editorconfig.org/)
