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
x - clean up buffer experiment. may need abstraction / clones
x- graphed sequencer(s) for delay fx...
	see tests/sequence.pd
x - repeating the convolved thing so literally doesn't sound good IMO
x	- rearrange to do live convolution of delayed parts?
x - rotating bank of dry / wet (stereo) buffers
x - ripple fx cascade pattern
x need to have the graphs remembered in the parent patch somehow?
- rotating bank of fx
- add else/autofade for loops
x - clearing buffers
- make the repeats smoother, better tail?
- phase vocode stretch the repeats?
- switch the carriers without glitching? maybe shared buffers?
- do we need three vocodes? what about having different sample selects on playback instead, and only the two primary vocode banks?
- recorders have some better persistence
- playback indexes separate from recorders?
- more banks?
- clear out buffers when switching back?

dorien
- make it cool

regulator
- start from the soundhack granular thing?

rain
- tbd. little fragments raining down.

ice sketch
- good start. maybe animate it?




BUGS:
- fix the else/rotate ... rotate 0 results in longer lists
x - fix the sequenced players to work better and start at first step
- fix the recorder_jdn abstraction to clear buffers / resize?

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
