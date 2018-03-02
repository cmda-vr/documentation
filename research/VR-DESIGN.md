# Ontwerpen voor Virtual Reality

## 3D grafisch ontwerp
Ontwerpen voor VR is anders dan 'traditioneel' ontwerp. Je werkt nu vaak in een *'3D ruimte'* ten opzichte van traditioneel *'2D'* ontwerp.

> (I) Alle grafische elementen zijn uitgedrukt in drie-dimensionale geometrische data maar worden uiteindelijk wel als 2D afbeeldingen om een monitor gerendered.

### Coordinate System
In 2D ontwerp maak je gebruik van twee assen; x (horizontaal) en y (verticaal) waardes. In 3D komt daar nog een derde as bij; z (diepte).

De z-as is in VR altijd op het scherm, de x-as en de y-as kan buiten de *'field of view'* van het scherm raken.

Een positieve waarde op de z-as betekent dat element *dieper* in het scherm gaan. Dit noemen we een *'lefthanded coordinate system'*. 

> (I) Bij WebVR is dit juist andersom een positieve waarde op de z-as betekent dat element dichter in je gezichtsveld komen. Dit noemen we een *'righthanded coordinate system'*.

### Objecten
Naast 360 foto en video formaten werken we in VR vaak met 3D object modellen.

#### Mesh
Een mesh is eigenlijk de **vorm** van het object. Zo'n object staat vaak uit allemaal losse lijnen (vertices) die de uiteindelijke vorm van het object maken.

#### Materials
De **oppervlakte** (structuur) van een mesh staat vaak los van het model. Het is een apart formaat vaak een *'texture map'* (afbeelding van de textuur). Al deze oppervlakte eigenschappen van een model noemen we vaak *'materialen'*.

#### Transforms
De **positie** van het object in de ruimte. Door te 'transformeren' pas je de lijnen van het originele object niet aan, je verplaats het alleen in de ruimte op basis van coordinaten.