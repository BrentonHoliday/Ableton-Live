[Back to articles list](../README.md)

# Ableton Live Naming Conventions

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
