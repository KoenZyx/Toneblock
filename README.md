# Toneblock
Waveform Synth made with Pure Data and turned into a VST3 using Camomile. 

TONEBLOCK STILL NEEDS WORK, EXPECT BUGS! 
And please read the following:

## Install notes
- Place the Toneblock folder* in your VST3 folder and (if needed) tell your DAW to scan for new plugins. 
  *the folder name needs to be exactly the same as the name of the vst3 file
  
## Usage notes
- Midi notes are too high, setting the course to -64 is more correct.
- Waveshaper presets aren't tied into the persistence yet, this may/will affect preset saving/loading.
- Automating the waveshaper settings is possible but seems to freeze when the UI is visible. 
- Label messages don't work when the code is loaded as a vst, that's why some of the UI labels seem strange. 

## Screenshot of UI
![Toneblock_Screenshot](/Resources/Toneblock_UI.PNG?raw=true "Toneblock UI")

...
