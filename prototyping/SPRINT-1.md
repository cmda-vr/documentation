# Sprint 1 - Boilerplates
**Week 8 - 10**

De eerste paar weken van het prototypen ben ik vooral gaan kijken wat de mogelijkheden zijn voor de technische uitwerking. Zoals bij de [werkwijze](https://productbiografie.dandevri.es/prototyping/WORKING.html) sectie staat beschreven heb ik een GitHub organization aangemaakt voor alle broncode.

## API

In eerste instantie is er de WebVR API die onderwater gebruik maakt van WebGL. De WebVR API exposed verschillende functionaliteit om het rendered in een head-mounted displays mogelijk te maken.

Sinds december 2017 is de specificatie van de WebVR API stopgezet omdat deze vervangen gaat worden door de WebXR API.

| Specificatie | Omschrijving |
|-|-|
| [WebVR Spec 1.1](https://immersive-web.github.io/webvr/spec/1.1/) | Deprecated |
| [WebXR API](https://immersive-web.github.io/webxr/) | Draft |

Voor de uitwerking heb ik besloten om niet met deze API's te werken.

| Reden |
|-|
| De WebVR API is redelijk stabiel maar als je daar nu mee zou werken ga je aan de slag met legacy techniek |
| De WebXR API is dan weer teveel toekomstmuziek en er wordt ten strengste afgeraden om deze in productie te gebruiken (te onstabiel) |
| Vanwege de beschikbare tijd is het leren van een nieuwe API een te hoge leercurve |

## Frameworks
Bovenop deze API's zijn er abstractielagen gemaakt in de vorm van frameworks.

| Framework | Omschrijving |
|-|-|
| [A-Frame](https://aframe.io/) | Populair, Simpel |
| [Babylon.js](https://www.babylonjs.com/) | Te Complex |
| [PrimroseVR](https://www.primrosevr.com/) | Legacy code |
| [ReactVR](https://facebook.github.io/react-360/) | Leercurve React|
| [Three.js](https://threejs.org/) | Te Complex |

Uiteindelijk heb ik de keuze gemaakt om voornamelijk gebruikt te maken van A-Frame.

| Reden |
|-|
| A-Frame is entiteit based waardoor je voornamelijk in HTML werkt|
| ReactVR zit je locked-in in het React ecosysteem |
| PrimroseVR voelt teveel als een legacy project en wordt niet meer regelmatig geupdatet |
| Three.js en Babylon.js hebben een te hoge leercurve, heeft een lange setup nodig om een basis scene op te zetten|

## Modulariteit

### Bundle
A-Frame bouwt hevig voort op een componenten systeem waarbij je nieuwe features kan toevoegen door externe scripts in te laden.
```
<script src="https://aframe.io/releases/0.8.0/aframe.min.js"></script>
```
Deze opzet zorgt er al snel voor dat het moeilijk wordt om versies bij te houden en daarbij komt dat het inladen van verschillende externe scripts invloed kan hebben op het renderen en dus performance.

Door gebruik te maken van Webpack en NPM modules is het beter om verschillende modules te bundlen.

```
require('aframe');
```
### Declarative HTML
Doordat je in A-Frame uitsluitend werkt in html (afgezien van custom events en de build tools eromheen) wordt de `index.html` al snel lang en onoverzichtelijk. Omdat ik toch al gebruik maakte van Webpack was het een logisch keuze om daarbij `html-loader` te gebruiken zodat ik HTML snippets en partials kan `includen`.

### A-assets
Daarnaast wordt het door A-Frame aangeraden om gebruik te maken van het assets systeem. Door externe files (afbeeldingen, modellen) te cachen in memory zijn er voor vervolgbezoeken aan de pagina minder requests nodig ([A-Frame, Best Practices](https://aframe.io/docs/0.8.0/introduction/best-practices.html)).

## Feedback volgende Iteratie
Doordat er bij de opdrachtgever geen technische mensen aanwezig zijn heb ik vanuit deze partij weinig feedback gekregen. Vandaar dat ik vooral op de opleiding en aan mede-studenten m'n broncode heb laten zien. Over het algemeen was deze duidelijk en begrijpbaar.