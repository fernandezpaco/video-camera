# video-camera
Polymer component for video camera access and for image capture

It can take a snapshot (screenshot/selfie...) of the image when you click on the video or when you invoke the takePicture method. Takepicture method has a boolean parameter so you can bind it or not to any kind of switch.

```html

<video-camera screenshot="{{screen}}"></video-camera>
<img src="{{screen}}"></img>

```

Additionally you can use it to bind it to a webrtc stream. In case you want if for this porpouse, you need to activate the waitforinput flag.

```html
<video-camera waitforinput="true" stream="[[peerstream]]"></video-camera>
<webrtc-peer peerid_tocall="the-peer-id" peerstream="{{peerstream}}"></webrtc-peer>
```

You can see it working here: https://fernandezpaco.github.io/video-camera/index.html
