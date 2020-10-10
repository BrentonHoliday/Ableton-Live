[Back to articles list](../README.md)

# Music Brentefesto

_Published: 2020-06-30_

My manifesto for logic, organization and creating jams to move asses

### _Brent's guide to working productively with music_

1.  Do not give a fuck
2.  Do not listen to a track more than once without making edits.
3.  Do not apply non-creative effects, compression or mix techniques before the arrangement is finished.
4.  Save each file as a version before making large corrections or changes.

## Creative Goals

### Working with drums

Start off the drums almost anyway.

For instance, loading them into a drum piece by piece to (drum rack of snares or kicks) and then play them out on the pads.

Once a compelling drum sound has been put together, Separate each of the drums midi files and

#### Goals

1.  Set up all drums on a massive piano roll for easy editing
2.  route each piano roll note to a separate channel with the drum rack loaded in it.

#### Workflow

1.  There are two approaches to experiment with:
    -   Put into one giant drum map and route to invididual channels. This is the prefered way since editing them will be a lot easier on a single piano roll
    -   Put each drum sound into it's own track. This is a simpler set up method.
2.  Send the MIDI signal from either the piano roll to individual channels with the units on them. This way we can swap out MIDI signals muting a track and still get the exact same effect except less destructively.
3.  Create a (drum type) \\  [snare] sum with all \[snares] fed into one bus
4.  Create a Drum kit bus (Likely using a group) that handles the whole drum mix that each drum type bus is sent to.

# How to make a Drum Rack

## Picking out sounds to use for a drum

### Layering drums for different lengths and velocities

1.  A main loud pop sound (for when you really smack it)
2.  A beefy base of the snare (present through all but the most quiet sounds)
3.  1 or 2 shorter snares that can be used as rolls and are more tinny (use at lower volumes)
4.  a light touch snare (can be adjusted manually)

Load  the samples that you're interested in into a sampler unit:

-   Use multiple different drums to layer at different velocities. For example for a snare.

### Layering them for a multi sample

Now that they are all loaded into sampler as a multi sample, go to the zones and make a midi piano roll to map out hit for the same drum.

## Setting up a testing channel

1.  In sessions view create an empty midi channel
2.  Set the output to go to the drums channel and select the pad you want
3.  Make sure to set all the midi notes on C3 or whatever your samples are tuned to

This way you don't have to move each midi signal around, you can just select a new pad when you're done with the prior.

#### Starting with all hits at the same volume

1.  Start with quarter notes. If you have 4 drums layered for each pad use 4 quarter notes and loop it put it in the sessions view.
2.  Make sure that in the global section "vol&lt; vel" is set at zero.
3.  if you have 4 sounds use 127, 96, 64, 32 as markers for each of the sounds
4.  use the fades to blend them together
5.  right click somewhere in sampler and normalize all the volumes
6.  Pick out the correct order for the hits (as you hit the drum from harder to lighter)
7.  use the fades to control the volume. Note that the drums do not have to perfectly match to a decrease in volume in velocity,  but as triggers for the sound to change. You can fine tune the volume later.

Aim to have the volume of the loudest hit be at -6db on the channel.

_Use the arrangement loop (or even better the session view) to create different regions and make loops to test each of these sounds, use the global tempo to make the beats run faster or slower 500-900 bpm can be useful..._

After you've found the velocity hot spots and made a loop next create two more midi loops

1.  different length notes same velocity (2, 4, 8, 16, 32, 64)
2.  Quarter Notes (even velocity decrease).

    -   use the pencil tool and size the grid to 1/4th notes and then just run the pencil across.
    -   Disable the pencil tool and then in the velocity section in the midi editor hold cmd (on mac) and draw a line from 127 on the first beat to 0 on the last

## Creating different sounds depending on note length

if you want to have the ability to control the drum hit in some way but altering the note and having the release do something....

## Creating a smooth level fade in velocity

First, work out a logical strategy for each drum type. Then work out a good sounding strategy. For example again with a snare:

1.  try layering all the drums for 127.
2.  fade the loud ring out evenly to 64
3.  fade the main body of the drum down to 24 evenly
4.  fade the secondary hit (roll or whatever) sound from 48 down to 0 at 16
5.  fade the last sound from 16 to zero

Now every velocity hit is unique. and the sound is getting more quiet without having to mess with the "vol > vel" knob in global.

Make note of the places where the sound is the most different and each drum sound is heard the clearest. for instance 127, 88, 48, 16.

# Make all the drums for a drum unit the same level

1.  leave a blank line in between drum types (4 notes)
2.  C-2 through G-2 will be used for the MIDI controllers 8 pads to jam with. (G#-2 through B-2 will be left blank)

## Engineering Goals

1.  Aim to keep channel faders at 0 to preserve maximum dynamics (db level is logarithmic and loses dynamics the lower the fader level is)
2.  Gain staging -  aim for recorded signals at -18 on each channel. Final mixes should never exceed -6
3.  Create fader adjustments on the sum busses.

### Properly gain staging

The correct order for creating sounds and arranging is:

1.  find the correct sound at maximum velocity. Set the instrument to have the desired dynamics, not just the largest.
2.  Use velocity plugin to pre gain stage dynamics
3.  Use utility plugin at end of each instrument chain to gain stage the channel
4.  send all alike channels to a summing bus
5.  Gain stage and smooth out 1st stage summing bus
6.  Send first stage summing bus to mix bus
7.  Send mix bus to master
8.  Group channels by song if composed of many songs or by summing bus and use summing group as the mix bus. Or just don't use groups and group by instrument and/ or bus.

### Common DAW arranging

If the set consists of more than one song

1.  Group instruments by song. When the song changes the same instruments get a new channel in a new group
    -   How to organize takes
        1.  Figure out the basic loop and record takes in loop format that can be pulled in and referenced at different points
        2.  Only have one take track for each instrumet and keep take loops as small and usable as possible
    -   Track group ordering
        -   drums (shades of Black)
            -   k, s, t, c, r, ho, hc
        -   bass (shades of purple)
        -   melody instrument (green- blue)
        -   order of appearance (yellow - orange)
        -   master channel is white
    -   Place the same order and color sheme in the summing bus and takes group
    -   multi song sets, use the summing bus group channel as a mix channel and set to the master
2.  Each part has 1-4 channels
    channel for each hand
    rhythm
    embelishment
    takes / unused
    	or
    drums
    	the different drums
3.  Sum each of these group types to it's own summing bus and place is sum group for song
4.  On the takes or backup muted track, stash all additional takes and then either leave the instrument and effects for a backup state and disabled or delete the instruments and effects all together depending on project needs.

#### When working with drums and bass

1.  Start with a drum click
2.  lay down the scratch take in as many as you like
3.  Get the kick drum dialed in

### Properly gain staging

1.  find the correct sound at maximum velocity. Set the instrument to have the desired dynamics, not just the largest.
2.  Use velocity plugin to pre gain stage dynamics
3.  Use utility plugin at end of each instrument chain to gain stage the channel
4.  send all alike channels to a summing bus
5.  Gain stage and smooth out 1st stage summing bus
6.  Send first stage summing bus to mix bus
7.  Send mix bus to master
8.  Group channels by song if composed of many songs or by summing bus and use summing group as the mix bus. Or just don't use groups and group by instrument and/ or bus.
