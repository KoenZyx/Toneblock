# Toneblock
Waveform Synth made with PureData and turned into a VST3 using Camomile. 

TONEBLOCK STILL NEEDS WORK, EXPECT BUGS! and please report any bugs you find.
(See the issue list at the bottom of this file)

## Install notes
- Place the Toneblock folder* in your VST3 folder and (if needed) tell your DAW to scan for new plugins. 
  *the folder name needs to be exactly the same as the name of the vst3 file
- If you need/want to use the help files (outside the DAW) move them into the Toneblock folder, that way puredata should be able to find them when you right click the relevant object. 
  
## Usage notes
- The VST loads in a minimized state, button for expanding the UI is in the top right corner.

## Small UI preview
![Toneblock_Small_Screenshot](/Resources/Toneblock_UI_2_Small.PNG?raw=true "Toneblock UI small")

## Full UI preview
![Toneblock_Screenshot](/Resources/Toneblock_UI_2.PNG?raw=true "Toneblock UI")

## Work in progress
- Even smaller array sizes to emulate cheap/old hardware. (should also be easier on the CPU)
- Program support. (and making some factory programs)
- Auto-generating named sends from the parameters text file, so we no longer need to know the index of a parameter to save/load it. 
- UI overhaul.
- Trying to improve the waveshaper performance. (I need to study some more maths and program some c)
- More/better filters.
- More/better envelopes on filters and effects.
- Linking settings across multiple instances. (not sure how feasible this is)
- Cross-platform distribution.
- More complete documentation (help files).

## Known issues
- Bus activation fails, this can be traced back to an old bug in Juce.
- It's (too) loud, will be fixed soon.
- Automating the waveshaper settings while the UI is visible breaks the waveform processing. Still looking for a workaround.
- There are some issues with the phase inverting when it's not at 1 (default). I recommend not using this setting for now, same for phase-offset and the "reverse" toggle.
- Automating large waveform arrays use a lot of CPU, that's just the way it is. (An option for turning off waveform automation will be added for this reason)

...
