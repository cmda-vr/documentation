# Methods

## Benchmark Creation

**Why?**:  
*Existing products in your niche can be a valuable reference and source of inspiration.*

**How**:  
> Scout for products that are somehow related to your design goal. Create a structured overview of these products.

## Audio Visualization
Creating visualizations based on audio.

## Education
Enhancing the lecture experience. You can give students a quick link to demonstrate or show models. For example during a history lesson, showing the model of architecture or the inside of a museum (exploring 360 images / models or something).

## Physical Location / Multi Location
Being at different physical locations but come together in VR to experience something, Can be pretty interesting using sockets or something.

(Networked A-Frame)

## Accessibility / disabled
Creating a new environment for people who can't go outside to experience something.

## Best, good and Bad Practices

## WebVR guidelines

* **Present VR on page load:** Many VR sites are focused on the traditional 2D Web. Someone navigates to a page, waits for a loading spinner, clicks several buttons, and only then it enters VR mode. We need less 2D loading screens.
* **Handle link traversel:** Link traversal allows for us to remain in VR as we navigate from site to site.
* **Add audio:** Add any form of audio, anything is better then complete silence.

[http://supermedium.strikingly.com/blog/webvr-guidelines](http://supermedium.strikingly.com/blog/webvr-guidelines)

## Design Pattern Search

**Why?**:  
*Find common solutions for recurring problems and a description of the context in which these solutions work best.*

**How**:  
> Pattern collections are found in online repositories and books focusing on certain topics.

## Standards

> One of my favorite things about #VR development with @aframevr is the blank slate for user interface design. There are no  standards or expectations in a brand new medium.

## Terminology
Most VR experiences involve another crucial component: inter- action. Does the sensory stimulation depend on actions taken by the organism? If the answer is “no”, then the VR system is called open-loop: otherwise, it is closed-loop. In the case of closed-loop VR, the organism has partial control over the stimulation, which could vary as a result of body motions, including eyes, head, hands, or legs. Other possibilities include voice commands, heart rate, body temperature, and skin conductance (are you sweating?).

* [Field of View vs Point of View](https://medium.com/facebook-design/becoming-a-virtual-reality-designer-9dcf6ddea4c3)

## Hardware
* **Drop-in viewers:** turn your smartphone into a VR box (cardboard etc.). Drop the smartphone into a viewer with lenses.


## Interaction

### Patterns
List and overview of common patterns and interaction methods inside virtual Reality.

Red, Brett. ’Virtual Reality Human Interface Guidelines’. Online. Internet. Beschikbaar: [http://vrhig.com/](http://vrhig.com/)


### Actions
When possible, we designed more than one way to accomplish something. This redundant interaction approach aimed to give people the option to use what is most comfortable for them to accomplish the most common tasks.

[Article](https://medium.com/inborn-experience/designing-facebook-for-mobile-vr-df4823282d02)

### Events
* **Progessive enhancement:** what if a person doesn't have a hdm. What's the enhancement? They can look around with mouse and keyboard. Then gradually improve to input.
* **Gaze tracking:** looking with an arrow in the middle for a timeout to select items on the screen without input.
* **Fuse buttons:** Virtual buttons that leverage a timer, or fuse, which trigger after the user has focused on them for a certain amount of time. When creating fuse buttons, always give the user the option to directly and immediately click on the target. Avoid placing fuse buttons in close proximity to each other. Fuse buttons work best if they are large targets that are sufficiently far apart from each other. 

### Menus
However, Immersive Design poses an interesting question: where does the line between content and UI start and end?

As they envision a world to be inhabited by players, the interface to navigate it can often be abstracted into menus that live outside the world’s logic.

Although some games rely on the traditional 2D menu systems, others place cues in the environment to educate the user.

[Article](https://uxdesign.cc/immersive-design-the-next-10-years-of-interfaces-16122cb6eae6?token=aFtjGoqA_pn1Pe15)


## Fly on the Wall
Belangrijk om op een scherm mee te kunnen kijken naar wat de gebruiker ziet maar het is ook niet geheel onhandig om de persoon zelf te filmen. VR is natuurlijk ook voor een groot deel eenn fysieke ervaring.

> When a scientist designs an experiment for an organism, as shown in Figure 1.2, then the separation is clear: The laboratory subject (organism) has a first-person experience, while the scientist is a third-person observer.

> The Display is not the window. If you are testing on a desktop VR headset then it is pretty easy to see that the VR content is being displayed on a completely separate device.

A phrase we often say on the Facebook VR team is “put it on your face.” This emphasizes the fact that you shouldn’t design for VR without building a prototype that can be tried on a headset itself.

**Passive Immersive UX**  
Through user testing, we learned that most Gear VR owners don’t use VR standing up, instead, they use it while sitting on a couch or in bed and find constant interaction with the headset’s touchpad to be tiring.

## Guidelines

## Developing for Google Cardboard

Google. ‘Developing voor Google Cardboard’ Online. Internet. Beschikbaar:
[https://vr.google.com/cardboard/developers/](https://vr.google.com/cardboard/developers/)

### Design

* Understanding the physiological effects of virtual reality design, and following these guidelines, is critical to making your app a success and ensuring that users avoid simulator sickness.
* Establishing familiarity: As a new medium, users may not be familiar with virtual reality interactions yet.

#### Physiological considerations
Motion sickness is caused by the disparity between what one feels and what one expects to feel.

#### Head Tracking
Head tracking enables objects in virtual space to maintain fixed positions regardless of how you move your head, creating the perception of a virtual world surrounding you. 

* Never stop tracking the user’s head position inside of the application. Even a short pause in head tracking will cause some users to feel ill.
* If your app consistently drops head tracking at a particular time, fade the screen to black prior to losing tracking.

#### Control of movement
It is important that users are not “passengers” in the app as much as active drivers. Users should remain in control of their movement inside the app, so that they will be able to actively anticipate what they are about to see.

#### Velocity
When the user virtually accelerates or decelerates inside of your application, they will not feel the change in real life. The disparity between what they are seeing and what they are feeling may cause discomfort. You can reduce this discomfort by trying to keep the user at a constant velocity when they are moving inside of your app.

#### Fixed objects
If the user is sitting while using a virtual reality device, placing the user in a stationary virtual environment.

#### Brightness
Be mindful of sudden changes in brightness. Given the proximity of the screen to the user’s eyes, transitioning the user from a dark scene to a bright scene may cause discomfort as they acclimate to the new level of brightness

### Setup
To avoid the user feeling rushed, make sure the experience only begins when the user indicates readiness. Do not start your app automatically or based on a timer. Allow the user to click through an initial screen, signalling they are ready for the experience to start.

### Controls
When your app launches, place the UI controls in the user’s current field of view. Gaze tracking, fuse buttons.

### Feedback
Text instructions don’t perform well in virtual reality. Consider including short audio summaries instead to provide users with instructions.

### Reticle
If you are concerned that displaying a reticle may reduce immersion or create unnecessary visual clutter. Display the reticle only when the user approaches a target that they can activate.

## WebVR fundamentals

Google. ‘WebVR fundamentals’. Online. Internet. Beschikbaar:
[https://developers.google.com/web/fundamentals/vr/](https://developers.google.com/web/fundamentals/vr/)

### Performance

Keep track of performance, consistent high framerate is typically 60Hz (or 16ms per frame including the per-frame browser’s overhead).

You need to make sure that you aren't just hitting your frame timing most of the time, but that you have enough headroom on every frame that you can handle any variance that the device throws at you.

### Progressive enhancement

What are you to do if your users don’t have a Head Mounted Display (‘HMD’) or VR-capable device? Detect changes in the VR environment for us to discover and adapt to changes in the inputs and viewing options in the user’s device.

### Considerations
* Users must click a VR controller button before it's available to your code.
* The Display is not the window. If you are testing on a desktop VR headset then it is pretty easy to see that the VR content is being displayed on a completely separate device.
* We move the world not the camera. If I move 10 metres forward did I move 10 metres forward or did the world move 10 metres backward?

## Facebook VR

Facebook. ‘Designing for VR resources’. Online. Internet. Beschikbaar:
http://facebook.design/vr

**Use Depth to Reinforce Hierarchy**
Traditionally, we’ve been trained to design information hierarchy from top to bottom, left to right. However, in VR, the center point takes precedence over anything else and objects placed closer to you will take priority over objects that are farther away.