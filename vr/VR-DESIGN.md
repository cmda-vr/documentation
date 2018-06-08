# Ontwerpen voor Virtual Reality

## 3D grafisch ontwerp
Ontwerpen voor VR is anders dan 'traditioneel' ontwerp. Je werkt nu vaak in een *'3D ruimte'* ten opzichte van traditioneel *'2D'* ontwerp. Het opvallende is dat alle grafische elementen zijn uitgedrukt in drie-dimensionale geometrische data maar deze worden uiteindelijk wel als 2D afbeeldingen op een monitor gerendered in de head-mounted display.

### Coordinate System
In 2D ontwerp maak je gebruik van twee assen; x (horizontaal) en y (verticaal) waarden. In 3D komt daar nog een derde as bij; z (diepte).

De z-as is in VR altijd op het scherm, de x-as en de y-as kunnen buiten de *'field of view'* van het scherm raken. Een positieve waarde op de z-as betekent dat element *dieper* in het scherm gaan. Dit noemen we een *'lefthanded coordinate system'*. 

> (I) Bij WebVR is dit juist andersom een positieve waarde op de z-as betekent dat element dichter in je gezichtsveld komen. Dit noemen we een *'righthanded coordinate system'*.

### Objecten
Naast 360 foto en video formaten zijn alle andere vormen van toepassingen gebasseerd op een virtuele omgeving die bestaat uit 3D modellen. Een 3D model bestaat vaak uit 3 componenten:

**Mesh**  
Een mesh is eigenlijk de **vorm** van het object. Zo'n object bestaat vaak uit allemaal losse lijnen (vertices) die de uiteindelijke vorm van het object maken.

**Materials**  
De **oppervlakte** (structuur) van een mesh staat vaak los van het model. Het is een apart formaat vaak een *'texture map'* (afbeelding van de textuur). Al deze oppervlakte eigenschappen van een model noemen we vaak *'materialen'*.

**Transforms**  
De **positie** van het object in de ruimte. Door te 'transformeren' pas je de lijnen van het originele object niet aan, je verplaatst het alleen in de ruimte op basis van coordinaten.