# Learning Virtual Reality

> Cardboard can be first VR experience for many people.

> We can use web technologies to create applications. Faster to code and more cross-platform. Second; it affords us access to all of the existing infrastructure the Web has to offer. (hyperlinks, hosting etc.)

## Preface

This medium allows consumers to experience VR with affordable systems. Since the Oculus acquisition tech companies invested millions in the platform. The book is pretty broad, no too in-depth.

## Chapter 1 - Introduction
The ability to be transported to other places, to be fully immersed in the present. Consumer grade VR hardware is young, each offers a different experience with different price points.

The feeling of total immersion is what we are striving for with virtual reality.

### What is Virtual Reality?
Virtual reality has one goal; to convince you that you are somewhere else. It's doing this by tricking the brain. A variety of technologies achieve this;
* Stereoscopic displays; 3d displays (head-mounted displays). Produce stereo image that our eyes interpret as having three-dimensional depth.
* Motion tracking hardware; low cost components to sense when our bodies move and our heads turn, so we can update the view.
* Input devices; game controllers, body-tracking sensors etc.
* Desktop and mobile platforms; Computer hardware and operating systems.

You can achieve full immersion with most of these four components.

#### Stereoscopic Displays
This is the main ingredient in VR, 3D visual representation of the experience that conveys a sense of depth. One of the biggest inpediments to consumer-grade virtual reality was an affordable display.

Generate image for seperate eye, one slightly offset from the other to simulate parallex. From a softwware point of view, an hedset's job is to render an image a minimum of 60 and ideally 120 times per second.

#### Motion Tracking Hardware
Track the movement of the head. Inertial measurement unit (UMI), measure changes in rotation. Our perceptual systems are very sensitive to motion.

#### Input devices
Head-mounted displays enclose the user's eyes, they have to 'fly blind'. We don't use mouse and keyboard, we have alternative game controllers.

#### Computing platforms
Our existing computers and devices can be turned into virtual reality boxes simply by adding a few peripherals.

* Most VR developers build their apps using game middleware like Unity3D. (Middleware engines, IDE's)
* We can use web technologies to create applications. Faster to code and more cross-platform. Second; it affords us access to all of the existing infrastructure the Web has to offer. (hyperlinks, hosting etc.)
* Video players represent a whole class of virtual reality technology by itself, it is a copy of the real world.

### Virtual Reality Applications
* Video games are pretty obvious.
* Virtual worlds; socual user-generated persistent virtual worlds.
* Education; Interactive learning.
* Productivity; 360 workspace instead of computer
* Tourism; panoramas
* Architecture; Showing models and existing properties.
* Live events; VR video for concerts and live events.
* Web browsing; Navigate the web using VR.
* Enterprise; simulation, training etc.

## Chapter 2 - Virtual Reality Hardware
This is a rapidly evolving industry. New head-mounted displays are coming out all the time.

### Oculus Rift
It spaned an entire VR industry, first consumer market. 
* DK1; low resolution
* DK2; positional head tracking with camera

*CV1 is the difference between experiencing the promise of vr and actually experiencing it.*

### Samsung Gear VR
Gear VR is a partnetship with Oculus. The technology has been incorporated into the Gear VR. If you own a Samsung smartphone this is one of the best Mobile options. You develop with the Mobile SDK.

### Google Cardboard / Cardboard VR
Using and buying hardware is a major commitment. The most low-cost way is turning your existing smartphone into a VR box. It isn't as deep as immersive as expensive hardware but can be the first VR experience for many people. 

Cardboard simply refers to the technique of dropping a smartphone into a box with lenses. Head tracking for Cardboard is pretty straightforward, it uses the existing operatin system orientation events.

#### Input
Cardboard VR inut is wip, the phone is encased so you can't use touch.

## VR Input Devices
User input poses a new set of challenges in VR system design.
* Game controllers
* Hand tracking; motion input sensors. Low-cost motion devices. Leap motion e.g. Combination of cameras and infrared LEDs.
* Wireless hand and body trackers; 

Virtual reality is also pushing the envelope on user input. VR displays cut the user off completely from the outside world.

## Chapter 3
Information in this chapter is specific to the Rift and Oculus SDK, the same techniques will apply when developing for other headsets.

### 3D Graphics Basics
Graphics that use a three-dimensional representation of gemoetric data.
1. The data is represented in a D3 coordinate system
2. Drawn ('rendered') as a 2d image on monitor

The rendered image should be updates, it's billion dolar business. Real-time 3d rendering.

### 3D Coordinate System
2d; x and y values. Additional coordinate; z describes depth.
* x; horizontal
* y; vertical
* z; in and out

Most of the time the z-axis is always on screen. X and Y can move out of the field of view. z is in/out axis. Positive z is going *deeper* into the screen. This is known as a *lefthanded coordinate system. WebVR uses righthanded.

### Meshes
Object composed of one ore more polygonal shape, constructed out of vertices defining coordinate positions in 3D space. 3D meshes are often referred to as models. They only define the shape.

### Materials
The surface of a mesh is defined using additional attributes. Surface information can be represented using one or more bitmaps, known as texture maps. The surface properties a of a mesh are referred to collecitvely as materials.

### Transforms
3D meshes are defined by the positions of their vertices. It would get really tedious to change a mesh's vertex positions every time you wanted to move it. That's why most 3D systems support transforms, without changing any values in its vertices.

A 3D transform is represented by a transformation matrix, entity to compute the transformed positions of vertices.

### Cameras
Every rendered scene requires a point of view from which the user will be viewing it. 3D systems typically use a camera, an object that defines where (relative to the scne) the user is positioned and oriented.

Cameras are almost always represented using a couple of matrices.
* First matric; defines the position and orientation
* second matrix; translation from the 3D coodinates into the 2D drawing space of the viewport (projection matrix)

* View volume or view frustum; only objects within the view volume are actually rendere to the screen. (Field of view)

camera > viewport > projection

Cameras define the viewer's relationship to a 3D scene and provide a sense of realism.

### Stereoscopic Rendering
In VR we have to do the whole thing twice, each per eye.

* Define one main camera.
* Render from two cameras; Follow position and orientation of main camera but are slightly offset to the left and right.
* Render to two viewports; separate viewports for the left and right rendering camers.

## Unity3D
Professional game engines have become a tool of choice for developing virtual reality. Unity3D is defacto game engine. Engine contains native support for VR rendering and head tracking. Oculus has Utilities for Unity.

## Chapter 4

In partnership Oculus teamed up with Samsung to create GearVR. It uses the smartphone as a display but oculus lenses for the headset. Highest quality mobile VR experience.

They also have an Oculus Home, it fully immersive. You don't have to leave VR space to setup video's.

## Chapter 5 - WebVR

In previous chapters we worked with Native Platform SDK's to create applications, it's a single-user experience.

Many of us creating VR would prefer to build web applications;

* Instant access; No download and app install required.
* Easy integration of web data; pull in data from different API's and services.
* Cross-platform compatibility; HTML5 runs on all desktop and mobile devices.
* Fast, cheaper development; easiest cross-platform system for creating apps. Use open source development tools.
* Easier deployment; Deliver web applications and updates happen without having to go trough app stores.

Latest generation of web browsers include support for virtual reality using the WebVR api.

* Use the WebVR API
* 3D rendering in the browser with WebGL
* Or Three.js library

### The Story of WebVR
Roots can be traced to the spring of 2014. Acquisition of Oculus VR by Facebook, Mozilla began to work to add Oculus Rift support to Firefox. They used hacky ways to connect to the IMU hardware.

But then they see how far they could come with a native implemtnation, free of the performance issues. Since the WebGL meetup in 2014 there has been a flurry of activity to the API.

The collaboration between Mozilla and Google on WebVR is a testament to the power of web standards.

WebVR is not a standard. It is a set of extensions built into popular browsers. Someday we could see the WebVR API added as a W3C recommendation and becoming a true standard.

### The WebVR API
The browser already has the capability to do stunning real-time 3D rendering using WebGL. (The API standard for rendering 3D graphics using JavaScript) WebVR builds on top of that.
* Discovering / Connection displays; API for the developer to discover and connect to VR displays
* Presenting content; Presentation to the VR head-mounted display as a sseparate display device. Browser also performs any optial distortion.
* Refreshing the display; Application to refresh its graphics at the native refresh rate of the HDM.
* Head tracking; New JavaScript API that tracks head position and orientation.

With these four features, a application can use WebGL to render virtual reality scenes with high performance.

Desktop VR systems come with 6DOF, input controllers improve upon classis game controllers. WebVR API itself does not define support for 6DOF controllers. There is already the Gamepad API.

