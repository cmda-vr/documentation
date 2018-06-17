Doordat er veel versnippering is qua hardware en hoe (voornamelijk games) interactiepatronen inzetten heb ik een kort overzicht gemaakt van veelvoorkomende varianten.

## Input
Er is op het web niet één duidelijke manier van input. Door verschillende platforms en apparaten zijn er verschillende soorten input mogelijk ([Aframe, Interaction](https://aframe.io/docs/0.8.0/introduction/interactions-and-controllers.html#adding-3dof-controllers-daydream-controls-gearvr-controls)).

Al deze manier van input kunnen gebruikt worden op het web ([Google, Adding Input](https://developers.google.com/web/fundamentals/vr/adding-input-to-a-webvr-scene/)).

| Input | Voorbeelden |
|-|-|
| Muis | [Look Component](https://github.com/aframevr/aframe/blob/master/docs/components/look-controls.md) |
| Touch| [Look Component](https://github.com/aframevr/aframe/blob/master/docs/components/look-controls.md) |
| Accelerometer & Gyroscope. | [Google Cardboard](https://vr.google.com/cardboard/) |
| Controller (geen degrees of freedom) | [Google Cardboard](https://vr.google.com/cardboard/) |
| Controller (3dof) | [Oculus Go](https://www.oculus.com/go/) |
| Controller (6dof) | [Oculus Rift Touch Controller](https://developer.oculus.com/documentation/pcsdk/latest/concepts/dg-input-touch-overview/) |

### Magneet drop-in viewers
Bij de drop-in viewers is er, afgezien van het materiaal (karton of plastic), vaak onderscheid te maken tussen de manier van input. Drop-in viewers kunnen *wel* of *niet* input creeëren door de een magneet aan de zijkant van de viewer te plaatsen. Door het bewegen van de magneet pakt de telefoon het [signaal van de magnetometer](https://www.youtube.com/watch?v=-zpK4btcH84) op.

## Interactie

Deze manieren van interactie en selecteren zijn specifiek gericht op hardware die geen gebruik maakt van controllers (zowel 3dof als 6dof) of de magnetometer.

| Input | Voorbeelden |
|-|-|
| Gaze Tracking | [A-Frame Event](https://skezo.github.io/Reticulum/examples/basic.html) |
| Look and Lock | [VRhig](http://vrhig.com/) |
| Orbital Menu | [VRhig](http://vrhig.com/) |
| Fuse Tracking| [Reticulum](https://skezo.github.io/Reticulum/examples/fuse.html) |
| Moving Viewport | [Google](https://developers.google.com/web/showcase/2017/playcanvas) |

## Beweging
Beweging in de scene is zonder controllers relatief lastig. Met controllers wordt er vaak gebruikt gemaakt van [Lofting Movement](https://webvr.donmccurdy.com/checkpoints/) (ookwel teleportatie). Zonder controllers kunnen we een combinatie maken van Gaze Tracking en [Checkpoints](https://webvr.donmccurdy.com/checkpoints/).