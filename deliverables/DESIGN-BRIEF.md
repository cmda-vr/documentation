# Design Brief

## Introductie

### Aanleiding project
Het was op CSSday dat ik voor het eerst in aanraking kwam met WebVR. Tijdens de Minor Web Development - ‘Everything Web’ kregen we een uitnodiging van Krijn Hoetmer om een dag, de conference die hij organiseerde, bij te wonen.

Een van de talks is me tot de dag van vandaag altijd bijgebleven, die van Ada Rose Edwards over VR toepassingen in een browser. Alsof ik voor het eerst water zag branden; kan dit NU in een Web Browser? Zo zonder fancy tooling, geavanceerde hardware en zonder ook maar een enkele euro te besteden. Heb je een smartphone met een touch screen? Dan is de kans groot dat je VR op elk moment kan ervaren.

> Nu ik het laatste halfjaar van de studie nog kan experimenteren wil ik die kans pakken en mezelf binnen VR / AR ruimte wat meer ontwikkelen, en dan voornamelijk op Technisch (WebVR) vlak. VR op het web is het laatste jaar erg toegankelijk en laagdrempelig geworden en het verbaasde mezelf hoe weinig ik eigenlijk afweet van de technologie en interactie methodes binnen dit vakgebied.

### De zoektocht naar een opdrachtgever

Met deze visie ben ik contact gaan zoeken met verschillende partijen. In eerste instantie binnen het research lectoraat van de Hogeschool van Amsterdam en vervolgens bij verschillende VR agencies in Noord-Holland.

Nu wil het zo zijn dat studiegenoot Bart Oude Elferink bezig was met zijn afstudeerstage bij &Samhoud media. Na wat berichten heen en weer kon hij me in contact brengen met Jip Samhoud (CEO) en na een aantal dagen stond er een afspraak in de agenda.

Bij &samhoud hadden ze wel interesse in een project met WebVR en er was ruimte om mij te ondersteunen tijdens het project.

### Over de opdrachtgever
&Samhoud media is een creatief bureau gespecialiseerd in augmented en virtual reality producties. Voor grote A-merken creëren ze innovatieve concepten binnen VR en AR vakgebied.

> “ We’re front runners in the field of augmented reality (AR) and virtual reality (VR). “

Zo hebben ze gewerkt aan de AH dino campagne met Freek Vonk, AH ruimtereis met André Kuijpers en recent nog samen met de Rabobank aan Rabo PinPin. Aan de Oosterdokskade (VR cinema) werken voornamelijk mensen die in het digitale tijdperk zijn opgegroeid. Oog voor digitaal, media en marketing trends. 

## Virtual Reality Overview

### Doel
> Virtual reality heeft één doel; jouw overtuigen dat je op een andere locatie bent. Het doet dit door je brein te 'tricken'. Het gevoel dat je volledige opgaat in de nieuwe omgeving is belangrijk voor de ervaring.

### Hardware
Een combinatie van verschillende hardware devices maakt het mogelijk om een VR ervaring te beleven;

* **Stereoscopic displays;** 3D schermen (head-mounted displays) produceren een stereo beeld dat onze ogen intepeteren als diepte.
* **Motion Tracking;** Sensoren die meten hoe ons hoofd en lichaam bewegen.
* **Input device;** dit zijn over het algemeen game of motion controllers.
* **Desktop and Mobile platforms;** Daadwerkelijke hardware en operating system om de applicatie te draaien. (bijv. een computer of een mobiele telefoon)

## De Context
> Het doel van WebVR is om het voor iedereen toegankelijker (drempelvrij) te maken om VR te ervaren, ongeacht de devices en input die ze tot hun beschikking hebben. 

### Toegankelijkheid consument
Alhoewel VR systemen steeds betaalbaarder beginnen te worden, het aanschaffen van hardware is nogsteeds een grote stap. De low-cost manier is om je huidige smartphone als Head-Mounted display te laten fungeren. Het is wellicht een minder meeslepende ervaring maar voor veel mensen is dit de eerste manier waarop ze in aanraking komen met Virtual Reality.

### Toegankelijkheid ontwikkelaars
Voor ontwikkelaars is het ook een stuk toegankelijker geworden om een VR applicaties op het web te ontwikkelen. 
* We maken gebruik van bestaande Web Technieken waardoor we veel van bestaande infrastructuur kunnnen gebruiken.
* Het is in principe sneller te coderen aangezien we kunnen voortborduren op de kennis van programmeertalen die we al hebben.
* De uiteindelijke applicatie draait in een browser waardoor hij veel meer cross-platform is. Je hoeft niets te ontwikkelen voor een specifiek operating system of hardware device.

### Technische obstakels
* **Performance:**
De technologie op het web is nog beperkt en compleet experimenteel. Het lijkt me interessant om de grens van deze technologie op te zoeken. 

* **Progressive Enhancement:**
Vanwege de toegankelijkheid van WebVR kan je van tevoren niet voorspellen welke input een gebruiker tot zijn beschikking heeft. Welk type input heeft de eindgebruiker? Maken ze gebruik van ‘Head Mounted Display (HMD)’ of van een ‘Cardboard’?

* **Browser Support:**
Niet elke browser is hetzelfde, van Firefox tot Samsung Internet elke vendor heeft eigen implementaties van de WebVR API of biedt ondersteuning voor een bepaald framework. Dezelfde ervaring bieden voor elke browser is zeker een punt om op te focussen, al zal dit een nobel streven zijn.

## Het probleem

De consultancy tak van &Samhoudmedia (&Samhoud) werkt vaak samen met grote corporates die elk een duidelijke missie en visie hebben. Eén ding hebben ze allemaal gemeen; ze vinden het moeilijk deze waardes naar bestaande of nieuwe medewerkers te communiceren. 

In plaats van een 'standaard' briefing op bijvoorbeeld het hoofdkantoor zoeken ze een meer interactive manier van storytelling die nieuwe medewerkers kunnen  ervaren.

**Probleemstelling**

Nieuwe klanten weten vaak niet wat de mogelijkheden binnen VR zijn en kunnen zich slecht een beeld vormen van een uiteindelijk product.

**Probleemstelling**

Het overbrengen van bedrijfswaardes naar nieuwe medewerkers op een speelse interactive manier.

**Mogelijke oplossing**
> Een shared interactieve WebVR ervaring die gemakkelijk en snel in een browser te bekijken is zonder dure hardware.

**Interne Stakeholders**
* &Samhoud Media
* &Samhoud Consultancy
* Bestaande medewerkers

**Externe Stakeholders**
* Nieuwe medewerkers
* Corporate bedrijven

## Design Challenge
> Hoe kan een WebVR applicatie &Samhoud helpen met het 'onboarden' van nieuwe en bestaande medewerkers om belangrijke waardes binnen het bedrijf over te brengen?

## Focus

De focus ligt bij uitstek op de technische uitwerking van het product / prototype. Op conceptueel niveau kan ik wat meer leunen op de opdrachtgever, dat is tenslotte hun core business. Samen met hun kan ik het project goed afbakenen en inspelen op trends die zij de afgelopen jaren hebben zien opkomen. Zij hebben zelf geen technische mensen in-house waardoor ik het daar vooral van mezelf moet hebben.

* **Vooral onderzoekend te werk gaan**; het VR vakgebied wordt vaak omschreven als een 'jungle' dus de eerste paar weken zullen vooral onderzoekend van aard zijn. 
* **Gemaakte werk is open-source:** ik wil graag dat al het werk zoveel mogelijk publiekelijk beschikbaar is en iedereen inzage kan krijgen in mijn werkwijze en voortgang.

### Onderzoeksvragen
* Welke Frameworks en API's zijn er beschikbaar om WebVR toepassingen te maken
* Welke Browsers en Hardware devices kan je ondersteunen in de browser?
* Hoe detecteer je input en hoe kan je met deze input detectie de ervaring enhancen?
* Hoe kan je zonder input devices (controllers) toch interactie en events triggeren.
* In hoeverre kan je de applicatie constant op 60 frames laten draaien om Motion Sickness te voorkomen?

## Product Visie

De voornaamste obstakels en voordelen van WebVR staan onder 'de context' sectie beschreven. Een Virtual Reality toepassing in de browser ten opzichte van een Native applicatie heeft een aantal voordelen:

* Als ontwikkelaar werken met bestaande web technieken 
* Het werkt over het algemeen cross-platform (niet voor een specifiek hardware apparaat)
* De ervaring is sneller op te starten (via een browser en een link) ten opzichte van een specifieke app die je eerst moet downloaden
* Je kunt Virtual Reality ervaren zonder dure hardware aan te schaffen

## Mogelijke impact product

Dit aspect van een product zal gedurende mijn project wellicht wat meer op de achtergrond treden. Vooral op lichamelijk vlak kunnen er mogelijk ongewenste consequenties naar voren komen. Een van de grootste is natuurlijk *motion sickness*. Vooral tijdens het user testen is dit een punt om de focus op te leggen; hoe zorg je ervoor dat mensen geen last krijgen van motion sickness en hoelang mag of kan een gemiddelde Virtual Reality ervaring duren?

## Roadmap

### Werkwijze

De eerste paar weken ligt de focus vooral op idee ontwikkeling en research om het concept nog verder af te bakenen. In onderstaande roadmap staan de belangrijkste deliverables beschreven.

Na deze fase ga ik werken met een versimpelde / aangepaste versie van The Design Sprint en werk ik 5-dagen iteratief aan een prototype.

### Sprint Overview
* **Maandag;** probleemstelling duidelijk maken en bepalen waar de rest van de week de focus op ga leggen.
* **Dinsdag;** uitwerken en op papier zetten van mogelijke oplossingen.
* **Woensdag;** keuzes maken uit de oplossing en beginnen met eerste prototypes.
* **Donderdag;** uitwerken prototype naar high fidelity.
* **Vrijdag;** testen en observeren van de voortgang.

### Schema
**Sprints**:
* Idee Ontwikkeling: Week 0/3
* Research: Week 4/5
* Ontwerp: Week 6
* Prototyping: Week 7/17
* Afronding: Week 17/20

#### Idee ontwikkeling
|Week | Deliverables | Methods |
|-|-|-|
| Week 0/3       | Concept Overview       | Ideation|
|                | Requirements List      | Focus Group|
|                | Design Brief           |
|                | Expert Interview       |

#### Research
|Week | Deliverables | Methods |
|-|-|-|
| Week 4/5       | Lecture Summary        | Literature Study|
|                | Trend Analysis         | Trend Analysis|
|                | Technical Research     | Competitive Research|
|                | Inspiration Gathering  | Benchmark creation|

#### Ontwerp
|Week | Deliverables | Methods |
|-|-|-|
| Week 6         | Brand Box              | Mood Board|
|                | Asset Export           | Design Pattern Search|
|                | OBJ Models             | Design Spec|

#### Prototyping
|Week | Deliverables | Methods |
|-|-|-|
| Week 7/17      | Prototyping            | Participant Observation|
|                | Feedback loops         | Think Aloud|
|                | User Testing           | A/B Testing|
|                |                        | Co-creation|
|                |                        | Field Trail|

#### Afronding
|Week | Deliverables
|-|-|
| Week 18/20     | Presentation           |
|                | Promovideo              | 
|                | Landingpage             |
|                | Copy Writing            | 


## Bibliografie
Parisi, T. ‘Learning Virtual Reality’. Developing Immersive Experiences and Applications for Desktop, Web, and Mobile. 1e druk. California: O'Reilly Media, 2015.

M. LaValle, S. ‘Virtual Reality’. Fundamentals of virtual reality systems (2016): Cambridge University Press. Online. Internet. 13 januari 2018. Beschikbaar: [http://vr.cs.uiuc.edu/](http://vr.cs.uiuc.edu/)

HVA | HAN. ‘CMD Methods pack’ Online. Internet. Beschikbaar:
[http://cmdmethods.nl/](http://cmdmethods.nl/)

Google Ventures. ‘The Design Sprint’ Online. Internet. Beschikbaar:
[http://www.gv.com/sprint/](http://www.gv.com/sprint/)

## Woordenlijst

* Virtual Reality (VR): Simuleert een omgeving via een computer om een gebruiker via diverse zintuigen onder te dompelen in een ervaring.
* Augmented Reality (AR): Direct of indirect, beeld van de werkelijkheid waaraan elementen worden toegevoegd door een computer.
* Mixed Reality (MR): Vermenging van de werkelijke wereld en een virtuele (schijnbare) wereld die met behulp van computers wordt gecreëerd.
* Head-Mounted display (HMD): Een beeldscherm dat op het hoofd gedragen wordt. Het kan de vorm hebben van een bril (men spreekt dan van een virtualrealitybril, kortweg VR-bril of VRil[bron?]), of in een helm ingebouwd zijn.
* Three / Six degrees of freedom (3DoF / 6DoF): de beweging van het hoofd in een driedimensionale ruimte en het registreren van de positie.
* Onboarding: Het reeds beginnen met inwerken van je medewerker in de tijd tussen het moment dat hij de baan bij het nieuwe bedrijf accepteert, maar er nog niet daadwerkelijk werkt.
* Native applicatie: Een Native-app wordt specifiek ontwikkeld voor een platform (Android, iOS, Windows Phone) in een eigen codeertaal.

 