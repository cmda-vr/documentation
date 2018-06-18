# Sprint 1 - Boilerplates
**Week 8 - 10**

De eerste weken van het prototypen heb ik gekeken naar wat de mogelijkheden zijn voor de technische uitwerking. Zoals beschreven in [werkwijze](https://productbiografie.dandevri.es/prototyping/WORKING.html) sectie staat beschreven heb ik een GitHub organization aangemaakt voor alle broncode.

## API

Er is een [WebVR API](https://developer.mozilla.org/en-US/docs/Web/API/WebVR_API) die onderwater gebruik maakt van [WebGL](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API). De WebVR API exposed verschillende functionaliteit om het renderen in een head-mounted displays mogelijk te maken.

Sinds [december 2017](https://immersive-web.github.io/webvr/) is de ontwikkeling van de WebVR API stopgezet omdat deze vervangen gaat worden door de [WebXR API](https://immersive-web.github.io/webxr/).

| Specificatie | Omschrijving |
|-|-|
| [WebVR Spec 1.1](https://immersive-web.github.io/webvr/spec/1.1/) | Deprecated |
| [WebXR API](https://immersive-web.github.io/webxr/) | Draft |

Voor de uitwerking heb ik besloten om niet met deze API's te werken.

| Reden |
|-|
| De WebVR API is redelijk stabiel maar als je daar nu mee zou werken ga je aan de slag met legacy techniek |
| De WebXR API is dan weer te onstabel en wordt door de schrijvers van de specificatie ten strengste afgeraden om deze in productie te gebruiken |
| Vanwege de beschikbare tijd is het leren van deze nieuwe API's een te hoge leercurve |

## Frameworks
Bovenop deze API's zijn er abstractielagen gemaakt in de vorm van frameworks:

| Framework | Omschrijving |
|-|-|
| [A-Frame](https://aframe.io/) | Populair, Simpel |
| [Babylon.js](https://www.babylonjs.com/) | Te Complex |
| [PrimroseVR](https://www.primrosevr.com/) | Legacy code |
| [ReactVR](https://facebook.github.io/react-360/) | Leercurve React|
| [Three.js](https://threejs.org/) | Te Complex |

Uiteindelijk heb ik de keuze gemaakt om gebruikt te maken van [A-Frame]((https://aframe.io/).

| Reden |
|-|
| A-Frame is [entiteit gebasseerd](https://aframe.io/docs/0.8.0/introduction/entity-component-system.html) waardoor je voornamelijk in HTML werkt|
| ReactVR zit je locked-in in het gebruiken van [React](https://reactjs.org/) |
| PrimroseVR voelt teveel als een legacy project en wordt niet meer regelmatig geupdatet |
| Three.js en Babylon.js hebben een te hoge leercurve. Beide hebben een uitgebreide setup nodig om een VR scene op te zetten |

## Modulariteit

### Bundle
A-Frame bouwt voort op een componenten systeem waarbij nieuwe features kan toevoegen door externe scripts in te laden.
```
<script src="https://aframe.io/releases/0.8.0/aframe.min.js"></script>
```
Deze opzet zorgt er al snel voor dat het moeilijk is om versies van [externe componenten](https://aframe.io/aframe-registry/) bij te houden. Daarbij resulteerd het inladen van verschillende externe scripts tot [render-blocking](https://developers.google.com/speed/docs/insights/BlockingJS).

Door gebruik te maken van [Webpack](https://webpack.js.org/) en [npm modules](https://www.npmjs.com/) is het beter om verschillende modules te bundlen.

```
require('aframe');
```
### Declarative HTML
Doordat A-Frame uitsluitend werkt in html (afgezien van custom events en de build tools eromheen) wordt de `index.html` lang en onoverzichtelijk. Omdat ik toch al gebruik maakte van Webpack was het een logisch keuze om daarbij [`html-loader`](https://github.com/webpack-contrib/html-loader) te gebruiken zodat het mogelijk is om HTML snippets en partials te [`includen`](https://github.com/samhoudmedia/aframe-boilerplate/blob/master/src/index.html).

### A-assets
Daarnaast wordt het door A-Frame aangeraden om gebruik te maken van het [Asset Management System](https://www.google.com/search?q=a-frame+assets&ie=utf-8&oe=utf-8&client=firefox-b-ab). Door externe bestanden (afbeeldingen, modellen) te cachen in memory zijn er voor vervolgbezoeken aan de pagina minder requests nodig ([A-Frame, Best Practices](https://aframe.io/docs/0.8.0/introduction/best-practices.html)).

## Feedback volgende Iteratie
Doordat er bij de opdrachtgever geen technische mensen aanwezig zijn heb ik vanuit deze partij weinig feedback gekregen. Vandaar dat ik vooral op de opleiding en aan mede-studenten m'n broncode heb laten zien. De broncode was duidelijk leesbaar, de readme's gaven goede instructies voor het opstarten van het project en de mede-studenten vonden dat de keuze voor het gebruik van Webpack was onderbouwd.