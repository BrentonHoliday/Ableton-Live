# Working with Samples in Ableton and  Organizational Strategy

Since each line only has to be written once, just write it when you make the change. Then just keep appending.

## Logic in making names

-   Only name something if it's going to have a lineage through destructive edits
-   a channel name in a live project should fit heirarchy and nothing more. drums > cymbals > rides > big ride
-   The only exception is to automate naming conventions like when creating files when tracking.
-   I tried so hard not to have to do this, but it's necessary when working with modular components, not just files recorded into a daw that stay there and don't move. These files will move all over the place.

## Preset names

name of preset - specification - up the heirarchy

## Naming Clips and Files

## Midi Clips

### Even MIDI clips...

Since MIDI is not really sound but tiny instruction informtion, include the tiny information with it. Audio is much more nuanced and special information so this is easier.

Only unused MIDI is destroyed when consilidating save old and unused MIDI takes to an unused takes group and hide it.

Just name clips after the channel names. Make sure each sucessive take is named. Ableton will do this with a hash mark in front of the name.

take/variation # - patch - key - time signiture -  part - song

```bash
13 - Vibraphone - CM - 4.4 - intro - Lawrenece of Arabia Main Theme
```

Just name the takes channel as such and each created clip will be named as such

If it's just info to trigger drums or something more abstract than notes and time.

## Audio Clips

Audio clips have lineage. We want to be able to track that. Each time a clip is consolidated, it goes into the user library of ableton and will clog it up with bullshit over time. Instead harness the clutter and reuse it.

### For audio the basic format is:

```txt
Song/name - artist - album (if it came from one) - encoding format - source - any information about the source
```

### Examples

#### Ripping a sample off youtube:

It's Clean - Lawrence of Arabia - Mp3 48K 220vbr - Youtube <https://www.youtube.com/watch?v=jdFwhhH2x7I>

or at the least the video ID instead of the whole URL

#### Tracking some bullshit:

When you're tracking just name the channel that. and each recording will be auto named.

```txt
Brent noodling on guitar - Date and time - place - any notes
take 13 - Brent noodling on guitar - Date and time - place - any notes
```

#### tracking with more structure:

```txt
13 - guitar - 1 bridge - FX through deville and strat 1 - Date and time - place - any notes
```

_take # and bridge number_

#### Ripping a song off a record

```txt
Stuff - Miles Davis - Miles in the Sky - FLAC L7 24bit 88k Vinyl G+ Condition - Worn Ortifon Carts on a 1200 - Motu interface
```

You don't need to label non destructive but lossless changes. Like converting FLAC to AIFF.

#### Ripping a CD

```txt
Miles Davis - Miles in the Sky - Japan Mastersound - 24bit 88.2k FLAC
```

#### Using that FLAC File from the ripped record as a sample:

but first...

##### Grabbing the left channel from that FLAC in audacity:

```txt
Stuff L Mono - Miles Davis - Miles in the Sky - Japan Mastersound - Mono L FLAC 24bit 44.1k
Stuff - Miles Davis - Miles in the Sky - mp3 32kb 48k - Youtube C9rDt8SuH7k
```

_Stereo is implied with audio, even though we want to be using mostly mono. DO notice that mono is denoted 2x, once for the track name which is more accessible to us, and once for linage. We don't want to have to look past the CD edition to figure out that's it's only the _

##### Sampling a closed hi hat from that file:

```txt
Hi Hat Closed Light 1b - 8:33 Stuff L - Miles Davis - Miles in the Sky - Mono L FLAC L5 24bit 88k from FLAC L7 24bit 88k Vinyl G+ Condition - Worn Ortifon Carts on a 1200 - Motu interface
```

Then when you have just a tiny little single hi hat hit 3kb AIFF, you'll know exactly where it came from.

_More on naming drum samples below_

## Never be destructive

If making a destructive change like creating a clip for a drum machine or create a different channel and freeze the old one. Then Label the channel with "Working - whatever the old name was". You can freeze, mute and hide that channel and still get all your work back at from any point if you need and it takes up almost no overhead.

When making a cut to a clip add just wtf the cut is about to the front that way if you consolidate it it's just ready to go.

## Types of sample naming conventions

### Clips

sample name variations - sample data (how it fits) pattern - song data (key and tempo) - file lineage

name variations - beats (b) bars (B) pattern - key bpm - lineage

#### Examples

Hi Hat Closed Light EQed and Delayed - 1b - 8:33 Stuff - 8:33 Stuff - Miles Davis - lineage

##### A variation on a triplet drum fill that winds up from the 2 to climax to the next 1.

Drum fill triplets var - 3b oxxx - 119bpm - 8:33 Stuff - Miles Davis - lineage

##### A bass solo that last 4 bars

Bass solo var 2 4M - 4/4 CM 119bpm - 8:33 - Stuff - Miles Davis - lineage

_var just means variation if you can more than one. Try to use expressive words instead of var or just a number. Words like: tinny, wham, chocolate, shimmer. whatever the impression it gives you is. var would be good if you're trying to decide which of two samples to include in a pack and decide to throw in both ;)_

#### What's the logic here?

-   b - beat
-   M - Measure/ Bar

-   1b - 1 beat - Every 1 beat sample can work with all the others (1b - these don't need a time signiture)
-   2b - 2 beat
    -   samples can work with any even time signiture (2b - don't need a time signiture either)
-   say 3 beats of a 4/4
    -   3b oxxx 4/4 - these can't work with any 2/2 time but can if we can visually see where it naturally falls, it would save a million years later when looking for samples. (like guitar tab - open, on, on, on) make notation with as many subdivisions as needed. if we can see the time signiture next to it we can count it and place it without even hearing it.

The key should be labeled if there is any disernable pitch. Not people talking, but a bass drum is debatable. A snare drum is not, a tom would be helpful.

Meter should be labeled if there is more than one or two beats. Ableton shows this in the clip section for each transient.

### Midi

### Presets

Name any long term or inate configuration with all heirarchy details or what the variation of configuration is at save point.

## Maintainence

I've got a lot of these to clean up :(

Stuff L (Drums & Bass) - Miles Davis - Miles in the Sky (Japan Mastersound) - Mono Left FLAC 24bit 44.1k
Stuff R (Keys) - Miles Davis - Miles in the Sky (Japan Mastersound) - Mono Left FLAC 24bit 44.1k

### make sure to collect all and save anytime you import audio

Periodically check the file manager for your sets and make sure everything is filled away. Any poory name files can be renamed swapped out. Check all presets, modules, Library folder

### The real point

Also any lower quality files can be swapped out with higher quality ones. You can match up the wave forms and just switch them right out of any reference in a set.

## Workflow when sampling a track

1.  Load the track into a group called "Unwarped source samples" with a descriptive file name
2.  Duplicate the audio track outdie of the group and create a new group called "Warped source Samples" and duplicate the unwarped sample track into it.
3.  Click warp on the track and set it to complex
4.  Create a channel below it for your cuts called "cuts warped" or something. If you're cutting drum hits, set up a different channel for each kind.
5.  Go through the track and set warp markers. It's generally easiest to go 1 bar at a time and warp the 1 count of each bar. Go through a second time and dial it in when you're searching for hits.
6.  Don't throw this away after you're done as it has all the warp markers you created
7.  Cut samples to the cuts track
8.  When you are done with the source file back it up into the session view and remove it from the arrangement. Do this for each level of creating tracks.

### For Drum samples

### Method for tony williams loop chops

Cut loops into 1 bar slices. Make sure each slices cut to the grid.

Use the following naming convention for drum slices:

-   Loop Number and part (if loop goes for more than 1 bar)
-   Where the hit starts and ends (this will make placement easy)
-   A good patch name

### Beat placement (comes before duration)

-   1 = beat 1
-   2 = beat 2
-   2.5 = beat 2 and a half

...etc

### Note durations are notated as

1 - whole note
2 - half note
4 - quarter note
8 - eigth note
16 - sixteenth note
32 - thirty second note

### Examples

-   2/2 - 2nd beat/half note. would end on beat 4
-   4/4 - 4th beat/quarter note. would end on  0 (0 is the first beat of the next bar)
-   1/4 - 1st beat/quarter note on the . would end on beat 2

#### L1 2/2 roll (to snare)

-   Loop 1
-   half note
-   It's a Snare and a clear hit, has a roll in the prior hit

### Workflow

1.  Select the total length of the loops you want. This could be 1 loop at 1 bar or 7 loops over a sequential 12 bars some loops being 2 bars or more.

crop the sample at the total length you plan on using and have warped.

2.  find a loop and set the loop marker perfect
3.  Create a "loops" track below it and clip each 1 bar loop segment to it naming each one . **when sending to drum rack, use a default 1 shot preset. when cropping clips from the 16 minute track, use crop and  preserve warp timing to off**. This track will preserve each of the loops in the context of the original song. Name each loop something like "L1 Snare to Roll - 4/4 CM 128.74bpm". This means Loop 1, it's a snare to roll - 4/4 time in c major and the bpm. Name and color each of the loops. Same color if the loop is more than 1 bar.
4.  Do not crop the loops instead go through and slice them into 1 bar segments. Name and color each of the loops. Same color if the loop is more than 1 bar. Use L2.2 for loop 2 part 2.
5.  For each of the loops, right click on it "slice to midi" and use your custom preset for 1 shot hits. make sure that preserve warp time is off. This will produce a midi piano roll for each loop. Set your quantize settings and then quantize all the midi notes (start and end) to fall on the grid perfectly.
6.  Name each slice on the simpler instrument (this will name simpler, chain and the pad the same name)
7.  Set up loops based on each of your samples and begin selecting the best hits. Duration should play a large part in choosing the samples. load each of these samples into their own sampler (convert from simpler) and begin adding in beats and creating richer sounds for these hits over 2-3 loops at a time.


7.  build around a 10-15 piece drum kit. each drum hit treated as it's own instrument through sampler that can play scales.
8.  do strange, subtle things with routing/zoning where different notes get routed to different chains. say a d# tom tom gets routed to delay or reverb or has a synth sound behind it.
9.  Listen through headphones and laptop speakers. get deep bass on headphones and octive higher frequencies only on laptop speakers for the same sound.
10. try not to perfect each hit but make it variable and expressive
11. build the whole kit together so that the sounds match
12. put together a few loops from altered versions of bar length samples
13. start out with a straight loop chopped up in midi. use the filler slices in their default places as scaffolding to begin making beats.
14. Add in other elements of the kit and begin removing scaffoling sounds
15. create several variations for each of the loops and beats and fills and layer into a group
16. set up an arpegiator to begin choosing these layers at random and randomizing different components such as take selection for variation, velocity.
17. try to figure out a way to create builds and waves in the playing over 16-32 bars. do this by a sense of intensity. find some global midi parameter that can be referenced

#### Slicing

1.  Select the passage of music you want from the warped source sample
2.  copy it to it's own cuts track
3.  Back up the samples to the session view
4.  Crop not consolidate existing samples in arragement view
