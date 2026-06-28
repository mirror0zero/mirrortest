To use the interface with your own projects created in SunVox, you will need to add a Ctl2Note module in your project and rename it "vctrl". Pitch and velocity values from that module can then be mapped to other module controls in your or be used trigger instruments or the MultiSynth module.
<b>Note:</b> Pitch values are determined by motion along the x-axis, and velocity values are determined by the tracker's position along the y-axis.

Alternatively, using the module group from the <b>vctrl</b> file will also allows for adjustment of the trigger time in the "vctrl" module by changing the "Attack" and "Release" times of the ADSR module.


There are three buttons which control the SunVox Javascript engine:

<b>execute</b> - starts the SunVox engine and initiates tracker playback from the beginning of the project. It is important to note that the camera opens approximately five seconds after the <execute> button is clicked.

<b>abort</b> - stops the project. You will need to click this button twice to completely stop the sound engine.

<b>local file</b> - opens a file dialog to allow you to load SunVox project files from your local system.


The motion tracking algorithm is controlled using six sliders:
<b>threshold</b> - determines the amount of variation between points required to confirm motion.

<b>step_size</b> - controls the "smoothness" of the motion tracking.

<b>min_points</b> - controls the minimum number of delta points required to confirm motion.

<b>hue_center</b> - controls the color to be tracked. The container background changes with the selected hue.

<b>hue_range</b> - determines the range of color variation to be considered for tracking.

<b>min_brightness</b> - controls the minimum amount of color brightness required to confirm motion.


There are two utility project files included on the main page:
<b>tracking_test // no_audio</b> - this file is useful for "tuning" the algorithm prior to using it for controlling any sound. As the name suggests, it do not produce any audio.

<b>audio_test</b> - this file uses motion tracking to play a granular bell-like sound. It can be used to further adjust the motion tracking as well as the audio output of the system.
