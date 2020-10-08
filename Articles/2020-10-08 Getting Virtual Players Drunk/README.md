# First Experiments with Virtual Player States in [DQRDAP](../2020-07-06%20Post%20Music/README.md)

### _Getting virtual rock musicians drunk_

_Well, if There's one state of mind that most modern rock musicians share it's being drunk, since half the time we're playing, we're actually just working for someone else trying to sell more booze for them. One of the few industries that gets paid in liquor. It's not so much that alcohol is a depressant... it's the state of the world._

![Brent got wasted during the making of this module](media/drinky-crow.png)

* * *

## Tools for the job

There are three rack containers in Ableton

-   **Instrument Racks** - These group audio together. samples or tone generators
-   **Audio Effects Rack** - These group audio filter effects together
-   **MIDI Effects Rack** - these manipulate MIDI data

## Creating a very loose Person module for @BrentonHoliday

I've created:

-   **MIDI Effects** Rack for a Person Model that will represent Brenton
-   **MIDI effects** rack called drunk that interacts with the Brenton Holiday MIDI Rack
-   **Audio Effects Rack** for his standard electric guitar pedal board
-   **Instrument Rack** that will be is Fender Jaguar modeled and modified from the stock Ableton Electric Guitar.

### Types of MIDI Modules

##### There are two types of MIDI Modules in Post Music

-   **Pre / Performance** - Used while you're tracking or in some way directly interacting with Ableton.
    -   _example: a velocity module that you used to compensate for your controller while you're tracking MIDI_
-   **Post / Playback** - Used while your playing back already tracked MIDI
    -   _example: a velocity module that you used to add human feel after you've tracked the MIDI_

Audio and Effects racks can be used for either purpose.

## How the drunk rack interacts with the player modules

For more information please reference the [Quantum Russian Dolls Paper](../2020-07-06%20Post%20Music/README.md)

### Drunk modules

These are a set of variable MIDI effects that can be attached to player performance modules. A parallel Module to Person . They will influence the parameters of player modules. By Changing the player modules variables in relation to their normal (sober) values.

-   Virtual people are only used for playback, even though it's a type of performance or can be used while performing. You can't compose into people.

#### Drunk Brent Illustration

-   Drunk Module
-   Brent
    -   Brents Brain (controller)
    -   Brents Instrument
        -   Instrument Controller
        -   Instrument
            -   Instrument Basis or samples
        -   Instrument FX or amp

#### Can you get your instrument drunk?

Despite instruments being made of varying qualities of interaction and value. It doesn't contain the correct hookable receptors to get drunk. First off a guitar is an Instruments Rack not a MIDI rack and Spaces can be a huge array shitty qualities but they can't get drunk. Also because they are Effects racks. Drunk effects accuracy of velocity, note, length. The things that happen when instrument get played or are controlled by MIDI.

## WTF is the point of this?

Stay tuned for next week :)

## Downloads & Symlinked Media

### Audio Exports

-   [mp3 - Brent with his guitar and pedal board playing the MIDI file ](#)
-   [mp3 - Brent with his guitar and pedal board playing the MIDI file after 9 beers](#)
-   [mp3 - Brent with his guitar and pedal board playing the MIDI file after 9.5 beers, 5 whiskeys and a burrito](#)

### The MIDI File in Question

-   [MIDI File Download](#)

### Modules

-   [Drunk Module 1.0 - MIDI Rack Module](#)
-   [BrentonHoliday Module - MIDI Rack Module](#)
-   [Brent's Guitar Module - Instrument Rack Module](#)
-   [Brent's Pedalboard Module - Effects Rack Module](#)

* * *

![crow](media/crow2.jpg) ![oh sees](media/jd.jpg)