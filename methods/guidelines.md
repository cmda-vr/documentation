# Guidelines

## Developing for Google Cardboard

Google. ‘Developing voor Google Cardboard’ Online. Internet. Beschikbaar:
[https://vr.google.com/cardboard/developers/](https://vr.google.com/cardboard/developers/)

### Design

* Understanding the physiological effects of virtual reality design, and following these guidelines, is critical to making your app a success and ensuring that users avoid simulator sickness.
* Establishing familiarity; As a new medium, users may not be familiar with virtual reality interactions yet.

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

Keep track of performance, consistent high framerate is typically 60Hz. (or 16ms per frame including the per-frame browser’s overhead)

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