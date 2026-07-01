<b>mirror0</b> is a simple motion-tracking interface for use with the JavaScript SunVox engine.<br>

To use the interface with projects created in SunVox, you will need to add a Ctl2Note module in the project and rename it "vctrl". Pitch and velocity values from that module can then be mapped to other module controls or be used trigger instruments or the MultiSynth module.<br>
<b>Note:</b> Pitch values are determined by motion along the x-axis, and velocity values are determined by the tracker's position along the y-axis.<br>

<b>How To Use</b><br>

There are three buttons which control the SunVox Javascript engine:<br>
<b>execute</b> - starts the SunVox engine and initiates tracker playback from the beginning of the project. It is important to note that the camera opens approximately two seconds after the <execute> button is clicked.<br>

<b>abort</b> - stops the project. You will need to click this button twice to completely stop the sound engine.<br>

<b>local file</b> - opens a file dialog to allow you to load SunVox project files from your local system.<br>

The motion tracking algorithm is controlled using six sliders:<br>
<b>threshold</b> - determines the amount of variation between points required to confirm motion.<br>

<b>step_size</b> - controls the "smoothness" of the motion tracking.<br>

<b>min_points</b> - controls the minimum number of delta points required to confirm motion.<br>

<b>hue_center</b> - controls the color to be tracked. The container background changes with the selected hue.<br>

<b>hue_range</b> - determines the range of color variation to be considered for tracking.<br>

<b>min_brightness</b> - controls the minimum amount of color brightness required to confirm motion.<br>

There are two utility project files included on the main page:
<b>tracking_test // no_audio</b> - this file is useful for "tuning" the algorithm prior to using it for controlling any sound. As the name suggests, it do not produce any audio.

<b>audio_test</b> - this file uses motion tracking to play a granular bell-like sound. It can be used to further adjust the motion tracking as well as the audio output of the system.

<b>Performance and Offline Access</b><br>
While the interface is designed to use minimal resources, performance will ultimately depend on internet connection speed and the complexity of the project. To help mitigate connection-related issues, <b>mirror0</b> can be run offline by downloading the repository files to a local directory and running <b>index.html</b>via localhost. Note that all files must be in the same directory.<br>

<b>Licensing</b><br>
You are free to use, modify and/or distribute the code provided in index.html; however, if any SunVox resources are utilized you must adhere to the requirements found in the LICENSE.txt file distributed with this release.
