When airplaying a video to a remote device, the sending device's controls don't reflect the remote device's playing state.

### Steps to reproduce

- Make sure you are not already airplaying to a remote device by opening control center and canceling any active airplay session

- Using an iOS device, head over to https://dev1an.github.io/HTML-Airplay-bug/
- Start playing the video on your local device
- While the video is still playing on your local iOS click the `show Airplay picker` button and select a remote device to cast the video to

### Expected behavior

The video is being cast on the remote device and the controls on your local device reflect the state of your remote device:

- When the video is playing on the remote device, the controls on your local device should indicate that de video is playing (Updating the progress bar, showing a pause button, etc.)
- When the video is paused on the remote device the controls on your local device should indicate that de video is paused (static progess bar, play button, etc.)

### Actual behaviour 

The video is playing on the remote device but the controls on the local device (= the sending device) are those of the paused state. So the progress bar is not updating and there is no pause button.
