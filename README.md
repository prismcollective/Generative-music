This contains small learning projects that use puredata for audio and MediaPipe (TouchDesigner) for webcam processing. The goal is to create generative music from movements. 

These projects are probably not the best way to do things, but they're intended as a learning resource for those who want to learn more operators/techniques by seeing them and playing around. Each project has a short description. This will be updated as I create new projects and tests.

# How this works

![Untitled Diagram drawio](https://github.com/user-attachments/assets/7a06aa97-6508-4cdb-9145-22fd70eb2c98)

Which software is used for what. Of course, this is just one way to do it-- many others use different softwares for the audio part, like VCV rack, Ableton, Max, etc. Any virtual midi device should work.

# Quick setup
* Install TouchDesigner (https://derivative.ca/)
* Install puredata (https://puredata.info/)
* Install the MediaPipe plugin for TouchDesigner (https://github.com/torinmb/mediapipe-touchdesigner)
* Install loopMIDI (or some other virtual midi progam; https://www.tobias-erichsen.de/software/loopmidi.html)

### For each project, you might have to:
* Open loopMIDI, and both the .pd and .toe files. In TouchDesigner, go to Dialogs -> MIDI device mapper -> Create new mapping, and set the out device to "loopMIDI port".
* In puredata, go to Media -> MIDI Settings and set the input device to loopMIDI port.
* In puredata, go to Media -> Audio Settings and set an output device.
* To start/stop audio in puredata, go to Media -> DSP On or DSP Off.
* You'll have to set the webcam by clicking on the MediaPipe node in TouchDesigner. There's a dropdown to select the webcam. Try resetting it also.
