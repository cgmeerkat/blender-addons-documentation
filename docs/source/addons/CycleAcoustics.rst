CycleAcoustics
**************

For the calculations to work as intended, the Cycles sample count must be set to 1. Don’t raise the sample count to increase quality; to get more lush reverb, enlarge the render resolution (make sure it’s square).

Larger resolutions “catch” more reflections and thus allow for more lush-sounding reverb, but there always comes a point where more pixels is overkill because it basically sounds the same. Smaller resolutions can still produce good-sounding reverbs, depending on the size of your scene (bigger rooms generally need higher resolutions for more reflections to fill out their longer reverb tails).

To save a CycleAcoustics render for later IR generation, you can save the render result as an EXR file. The format should be 32-bit RGBA (not RGB).

Controls
========

Exclude Direct (Wet Only)
-------------------------
(Full Edition Only) Makes the impulse response output include only indirect rays and none of the rays that reach the listener (camera) directly. Enable this if you intend to add reverb to a dry signal (e.g. use the reverb in a music production with dry/wet mix).

Speed of Sound
--------------
The simulated speed of sound in Blender units per second. Default: 343 (meters per second).

Audio Sample Rate
-----------------
The sample rate of the impulse response output (stereo WAV file). 44.1 KHz and 48 KHz are supported.

Max IR Length (s)
-----------------
This setting limits the length of the impulse response output in seconds.

Psychoacoustic Mode
-------------------
(Full Edition Only) Delays reverb reflections in the left and right channels based on the direction they hit the listener, affecting both timing and frequency response. This simulates how the head, body, and ears influence sound perception.

If psychoacoustics is disabled, the add-on just does simple panning (with a -6 dB pan law).

Output Folder Path and Output File Name
---------------------------------------
Output Folder Path: Folder in which the impulse response WAV file will be saved to.

Output File Name: The name that the file will be saved as. The add-on will not replace existing files (to prevent accidental overwrites); you receive a warning message if the output file name already exists.

IR Player (Online)
------------------
Pressing the button opens the `impulse response player <https://cgmeerkat.github.io/impulse-response-player/>`_ in your browser.
