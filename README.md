# ripplezone19
Pure Data patch for AquaZone sonic installation

TODO:
- have the carriers looping in memory and just pick which one dynamically - fix glitches!
- wet
- flow
- lattice
- rain
- more/better ambient tracks
- check levels on ambient tracks
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
x - rotating bank of fx
x - clearing buffers
- definitely do the carriers in ram
- why is ripples sketch so much louder than the others for mic input?
- set the light of the current sketch on startup
- trim more samples, don't have fades in audio
- recorders have some better persistence
- more banks?
- clear out buffers when switching back?
- mystery of the recorder_jdn buffers clearing, is it right?

CBB:
- add else/autofade for loops ?
- make the repeats smoother, better tail?
- phase vocode stretch the repeats?
- switch the carriers without glitching? maybe shared buffers?
- mic autogain circuit

dorien
- make it cool

regulator
- start from the soundhack granular thing?

rain
- tbd. little fragments raining down.

ice sketch
- good start. maybe animate it?


BUGS:
x - fix the sequenced players to work better and start at first step
- fix the recorder_jdn abstraction to clear buffers / resize?
- fix the else/rotate ... rotate 0 results in longer lists

Audio patch network:

- multiple patches

- vca network, vcs-style?
- solve last value thing on ctl_input_jdn macro
- jukebox mode
x - modular frontend
- look into streaming disk playback
x - modular fx setups
x - vs distinct patches
x - pitch shifting with feedback
x - granulation / clouds mode
x - pleasing sequencing?
	- according to jamie, just skip. no sequencing.
	- ambient noises only

System stuff:
x - how to have the patch auto-start in PD?
- how to have system auto-sleep at certain time?
x - how to have system power / on start playing at certain time?
x - maybe a timer on a switch?
- how to "VNC" in on-playa? maybe set up on my work laptop?

Hardware:
x - make the box
x - paint / cover the box with fur
x - which mic?
x - how to mount mic?
x - which switches / lights? (adafruit 30mm?)
NOPE - wire switches + lights into PI
NOPE - do i need anything i could get at lasher?

Audio system:
x - get d-class amp (amazon)
x - speaker wire
x - outdoor speakers vs. car speakers vs. computer speakers?
x - demo the best buy ones, audition.

...

NOTES:
x - pvoc phase vocoder example is neat for drones
x - else
	freeze~
	pvoc.freeze~
