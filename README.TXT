I made some changes based on the author's source code to achieve different sound effects.

Beat Box - a simple sound example.
Author: Michael Kolling

Play with it, and you see what it does.

It is not very sophisticated as it is. To see what it can do, create a TestBeat 
object and call the testBeat methods.

To play some more, you can try the following:

 - Create a BeatBox object. Call the beat(int instrument) method to do a single
   sound. See the Instruments interface for constants for different intruments.
   
 - Create a BeatBox object. Then define a track. You can define a track by
   calling the foloowing objects in sequence:
   
        newTrack(length)
            addBeat(tick, instrument)
            addBeat(tick, instrument)
            ...
        endTrack
        
   The length of a new track is defined in ticks. The tick of every beat must be
   less than the length of the track (and >=0). After defining a track, you can
   call start() and stop() to play the track.
   
 - Instead of doing it interactively, you can program a track. See the 
   testBeat methods in class TestBeat for examples.

 
