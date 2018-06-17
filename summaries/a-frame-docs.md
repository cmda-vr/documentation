# A-Frame documentation

## What is A-Frame
> A-Frame is a web framework for building virtual reality (VR) experiences. 

It's based on top of HTML making it simple to get started. It is not just a 3D scene graph or a markup language. A-Frame aims to define fully immersive interactive VR experiences that go beyond basic 360° content, making full use of positional tracking and controllers.

* Uses a powerful entity component structure. HTML is just the tip of the iceberg; developers have unlimited access to JavaScript, DOM APIs, three.js, WebVR, and WebGL.
* While A-Frame uses the DOM, its elements don’t touch the browser layout engine. 

## Installation
A-frame can be developed from a plain `html` file.
* Code editors
* Include JS build
* As dependency (npm)

## VR Headsets

### What is Virtual Reality
Technology that uses head-mounted headsets with displays to put users into an immersive virtual environment.

### Differences between headsets
* Have positional tracking or only rotational (6DOF or 3DOF)
* Have controllers
* Are powered by PC or by mobile device

All headsets provide atleast rotational tracking. Positional tracking are becoming minimum viable experience.

### What is WebVR?
It's a JavaScript API creating VR experiences in the browser. A-Frame uses the WebVR API to gain access to VR headset data. *Note that WebVR, which provides data, should not be confused nor conflated with WebGL, which provides graphics and rendering.*

### Where does A-Frame want to take WebVR
VR content with native-like performance. *A-Frame believes the minimum viable bar will trend towards positionally-tracking headsets with positionally-tracked controllers.* A-Frame wants everyone to be able to get involved with VR content creation

### Support
* A-frame supports basically every capable headset out there.
* Supports VR for any browser that implements the WebVR specification
* Supports most modern browser that don't have WebVR support with the WebVR polyfill.

## HTML & Primitives
A-Frame is based on top of HTML and the DOM using a polyfill for Custom Elements. The HTML and the DOM are only the outermost abstraction layer. Underneath A-Frame is an entity component framework for three.js. Elements are called primitives.

Primitives act as syntactic sugar. They abstract the core-entity component. Primitives are `<a-entities>` under the hood.You can also register your own primitives.

## Entity-Component System
It's a three.js framework with ECS architecture. Composition over inheritance and hierarchy principle. Common pattern in 3D game design.
* Entities; container objects into which components can be attached.
* Components; reusable modules that can be attached to entities. Plug-and-play.
* Systems; provide global scope, are often optional.

Box > position > material > geometry

* Entities; `<a-entity>` element
* Components; attributes on entity
* Systems;  `<a-scene>`

We create `<a-entity>` and attach components as HTML attributes. A-Frame has HTML and the DOM which makes ECS ergonomic and resolves many of its weaknesses.

* Referencing other entities with Query Selector; something that the DOM provides.
* Communication with events; Listen and emit events. Components can listen to eachother without calling.
* DOM provides APIs to update elements
* DOM provides attribute selectors

Components have full access to JavaScript. (WebRTC, Speech Recognition)

### Component based development
Place all code within components. The codebase becomes very reusable. Components can set other components on the entity. You can plug into other components using the registry.

## JavaScript, Events, DOM APIs
A-Frame modifies the HTML element prototype to add some extra behavior for certain DOM APIs to tailor them to A-Frame. 

## Best Practices
Mixins and templating are useful to reuse and reduce repeated HTML.

### Performance
A high framerate must be maintained in order for people to feel comfortable and as if they were in another place
* Use stats component

### VR Design
Designing for VR is different than designing for flat experiences. As a new medium, there are new sets of best practices to follow, especially to maintain user comfort and presence.