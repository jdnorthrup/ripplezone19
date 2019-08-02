# ripplezone19
Pure Data patch for AquaZone sonic installation

TODO:
x - get MIDI knobs working on Pi.
x - get audio input working on Pi.
x - make sure ELSE library works on Pi.
x - get more ambient audio clips, dice up into smaller chunks
x - spectral convolution
x - duck based on mic
x - pick from dir of files
x - have stereo background
x - have stereo convolution carriers
- clean up buffer experiment. may need abstraction / clones
- graphed sequencer(s) for delay fx...
	see tests/sequence.pd
- repeating the convolved thing so literally doesn't sound good IMO
	- rearrange to do live convolution of delayed parts?
- rotating bank of dry / wet (stereo) buffers
- ripple fx cascade pattern


Audio patch network:

- multiple patches
- trim more samples, don't have fades in audio

- vca network, vcs-style?
- solve last value thing on ctl_input_jdn macro
- jukebox mode
- modular frontend
- look into streaming disk playback
- modular fx setups
- vs distinct patches
- pitch shifting with feedback
- granulation / clouds mode
- mic autogain circuit
- pleasing sequencing?
	- according to jamie, just skip. no sequencing.
	- ambient noises only

System stuff:
- how to have the patch auto-start in PD?
- how to have system auto-sleep at certain time?
- how to have system power / on start playing at certain time?
- maybe a timer on a switch?
- how to "VNC" in on-playa? maybe set up on my work laptop?

Hardware:
- make the box
- paint / cover the box with fur
- which mic?
- how to mount mic?
- which switches / lights? (adafruit 30mm?)
- wire switches + lights into PI
- do i need anything i could get at lasher?

Audio system:
- get d-class amp (amazon)
- speaker wire
- outdoor speakers vs. car speakers vs. computer speakers?
- demo the best buy ones, audition.

...

NOTES:
- pvoc phase vocoder example is neat for drones
- else
	freeze~
	pvoc.freeze~
