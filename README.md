# Emotions
This repo covers some experiments to detect emotion. This was explored for the Comon Dag Van De Wetenschap installation.
The installation used 3 sensors to detect the emotional state of a person in a room:
* Stress levels ([emotibit](https://www.emotibit.com/))
* Emotion from facial expressions (webcam)
* Emotion from vocal expressions (microphone)

## Stress levels
Stress is a complicated thing to measure, but for this installation a rough indication is sufficient to experiment with. The emotibit is a HAT for an Arduino Feather that connects over http to a piece of software called the *Oscillator*. This oscillator connect to the hardware and streams the data in a dashboard also allows exports over OSC. [Read more on the set-up](https://github.com/EmotiBit/EmotiBit_Docs?_gl=1*1ved2u3*_gcl_au*MjAzMTUwMTI3MC4xNzU4MTc5MTEz*_ga*MTM2NDk1NzIxNi4xNzU4MTc5MTA5*_ga_9X5YR45643*czE3NTgzNTAxNzckbzQkZzAkdDE3NTgzNTAxNzckajYwJGwwJGgw).   
Things to remember:
* If you're unsure about the status of the emotibit: update the firmware
* Enter the WiFi credentials in the document on the SD card (i prefer using a smartphone hotspot for this). Make sure you connect the computer with in oscillatr to the same network
* Make sure the emotibit is not in hibernate mode (small swich on the board)

## P5 experiment
* Using https://p5js.org/
* P5 used an index.html and sketch.js structure to run processing-like code in a browser
* When working with pretrained models, these need to be downloaded first (weights), e.g. https://github.com/justadudewhohacks/face-api.js/tree/master/weights (put these in a models folder)

## Deepface experiment
```console
  pip install deepface opencv-python
```
