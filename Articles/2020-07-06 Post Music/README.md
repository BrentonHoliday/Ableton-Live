[Back to articles list](../README.md)

# Post Music Production Concept

## _aka Detangled Quantum Russian Doll Audio Production_

_Published: 2020-07-06_

Ok, ok, the title is a bit much but bear with me here. I've nearly got a prototype of this complete.

This is basically just a philosophy and workflow for creating music of any type  with a "human feel" that is comprised of remixable and reusable components on each level. It's always intentional, but never exactly the same.

1.  The **detangled** bit is how people can work together on whatever aspect of a composition they want in a non-destructive way while not screwing up the mix later and not being tangled up and bottle necked by each other.
2.  The **quantum** part comes from applied subtle randomness in the lowest levels to create in variations that can be encapsulated into a larger structure.
3.  The **russian doll** thing is how each component is added up to a larger whole and swappable with other components to create new structures.
4.  And um, we're going to apply it to **audio production**

_I've probably misused at least one of these words_

![omg salvia](https://images.fnewsmagazine.com/2019/04/Russian-Dolls.jpg)

_omg salvia_

## Abstract

Decouple sound design, playing, composing, arranging, mixing to all be approached in parallel throughout the creative process. Whatever inspiration fancies and whomever is fancy at the time.

Then, sprinkle in a variable dash of randomness in the lowest levels of each step.

### In a nutshell

I'll be using Ableton and [Max](https://cycling74.com/) as it's veritably LSD in software form.

1.  Have groups of takes layered in place and sent to virtual instrument channels. This keeps overhead low as only midi notes are stored.
2.  Sound design, arrangements and mixes can be done in parallel as they are completely separate.
3.  Create instruments, virtual players, bands as well as performance spaces to be packaged up reused (see: reusable, component based hierarchy below). _Mixing is basically creating a sterile laboratory performance space and then coloring it anyway, right?_.
4.  Create predictable and packageable variations of randomness algorithms on each level so no expression is identical (see: Quantum Musician Dynamics and Sound Design below). Again bear with me here.

## Basic Workflow for Playing, Engineering, Mixing

1.  Ideas would be tried out as usual on the scratch channels and fleshed out as much as needed. Instruments loaded in the channel its self with effects the simplest way with no immediate barrier. Just start screwing around or getting ideas out.
2.  If the idea is to be pursued, the instruments would be copied to their own channel in the instruments group in an instrument rack and a group set up in the instruments group for the instrument takes.
3.  For each take, a new channel is set up and routed into the instrument channel. _note: Digital performer had a sweet comping feature. This would model that, but not quite as elegantly, but better visually as well as creatively (more on that later)_. If variations are required for the instruments timbre or tonality, create a variation by copying the instrument in the rack and routing to the new one. This way there is a copy of both incase you need to go or want a change. Before each take the channel is copied and for the next take or a future one, **always leaving a blank take track for easy access in case inspiration strikes later**. These can be used for punch ins as well.
4.  After one or several successful takes, each take can be auditioned while still using only 1 actual Virtual Instrument that it's routed to, or multiple if you have set up several different versions in the rack. This will be highly efficient on the CPU, since [MIDI files are tiny antiquated things](https://en.wikipedia.org/wiki/Open_Sound_Control).
5.  One or a combination of several are selected for the current rendition of the arrangement, will be placed into a midi arrange track for that instrument in the arrangement group and the audio routed accordingly.
6.  Player variations can be added pre instrument rack by simply by adding subtle randomizer modules in the instrument chain like pitch, rhythm and attack. _See, This is not quite rocket science and a pretty common production technique._
7.  Then potentially cycling at light/ varying degrees from the chosen take to other takes with a variably yet lightly randomized arpeggiator module.
8.  Each of these takes, instruments, players etc can be exported as a whole or on their own for later use or [recombination](https://en.wikipedia.org/wiki/Genetic_recombination). _More on this below_.

_All non VIs tracks (audio tracks), would be triggered in arrangement group via MIDI. The same as all other instruments._

## Reusable, component based hierarchy

A lot of this is possible due to Ableton's open ended structure and their drum, instrument and effects racks. Racks are essentially folders for different serial or parallel chains that can be packaged and exported for later use.

### An example of a ride cymbal to a concert hall

![basic drum bussing right to left](https://i.imgur.com/UVCeYcv.png)

_example of kick drum bussing groups, but with in a rack context_

**Starting from smallest detail and moving up the acoustic reality chain**:

1.  A **ride cymbal** may be comprised of 4 or more different ride cymbals or synthesized sounds mapped out in velocities and triggered by a single hit to produce a complex and unique sound each hit. A ride sounds slightly or a lot different where you hit it and how hard.
2.  There may be a 2 or more rides on a kit. Each comprised of multiple sounds. These together make up the **ride group** (aka ride bus in studio nerd mix parlance).
3.  The two rides are part of a larger group called the **cymbals group** that include the crash or china/hi hats or splash, maybe even a gong.
4.  The Cymbals group is part of the **drum kit group** that have the rest of the components of the kit.
5.  The Drum kit is played by a **player**. This player may drag their fills (random setting on arpeggiator to get slightly out of time rhythm) or not have a very consistent attack on their hits (velocity module with higher variable randomization), or fretless instruments randomizing pitch by a reasonable and well tuned +20/-20 cents, or a slightly different delay of when when a strings player would apply vibrato. Different players would have different feels through predictable randomized settings to create their "style" of play. It wouldn't actually take that long to set that up. Just a few modules and knobs.
6.  The player can belongs to a group of musicians they are interacting with in the **band group**. Different bands have different dynamics through their role and relationship. The Bass player is likely is more tied to drummer than guitar player. The vocalist likely pays more attention to the guitar, less to the drummer and least to the bassist. Most importantly though, bands tend to have very peculiar but predictable dynamics that is magical and unique to the listener. These come in the form of errors as they are not generally intentional with non-academically trained career musicians. When there are peaks in the music often the band's metronome speeds up, musicians have harder attack and likely play less accurately. When there is a quiet passage, the opposite, things tend to be more quiet and delicate. _(More on the importance of imperfection below)_.
7.  The band of musicians performs in a space. **Space groups** like a hall can be modeled with different reverb modules and packaged in the same hierarchy.

It would be very easy to swap any of these steps with other components. Say step 6, to take the player away and swap them out with a different player on the same drum kit in the same room since the headlining bands drummer didn't bother bring his own drums.

We can even package up all of a bands instruments without the players attached and just let the other band keep them, since that's the [2033 punk spirit](https://wundergroundmusic.com/david-guetta-world-tour-cancelled-after-losing-usb-containing-his-entire-set-2/). Punk is no patches.

### Quantum Musician Dynamics

If you factor in player variations, sound variations due to play style, velocity of attack, room variations, dynamics between players (and even something as wild as random arpeggiation through different improvisational takes (!) by simply telling midi to select a variable degree of randomness of certain takes and shift MIDI tracks via legato) it would be possible to export 1000 copies of the same song and none would be exactly the same. Some would be very different. Yet each would be played, engineered and mixed exactly as intended.

This comes with even one other **potential** (_I haven't tested this part yet_) and gross hidden benefit. We can quantize individual tracks to a disgusting degree and sail through takes. If the velocities and rhythms, and even notes of takes, player dynamics or the global metronome are set to be slightly randomized **within a greater structure**, there would be a human feel.

### Quantum Sound design

This approach could be used as well in modeling sounds and instruments on the lowest level. For example, when modeling a sound with reverb, all acoustic instruments are in fact their own room. A viola or guitar contains a hollow space with in it, that causes the vibrations to resonate and creates a different timbre in the outer room, just as a rave club sounds different on the outside due to low frequency dampening and acoustic resonance on the inside. Da club is essentially a big acoustic resonance chamber from the outside.

![shove it up your f hole](https://upload.wikimedia.org/wikipedia/commons/3/30/Doublebass_fhole.jpg)

_Shove it up your f hole_

#### Example of a kick drum

Let's use a kick drum as a simple example. It has the space on the inside, with resonance and all, however dissecting what creates the sound is composed of many different sounds.

1.  The initial almost static noise of the felt of the pedal hitting the drum that is only a few milliseconds.
2.  The attack thud of the vibrations inside the drum pushing the air from the back head through the body and hitting the front head.
3.  The sound moving out of the drum and maturing in different directions (this is what we call a kick drum sound) and into the room. (how about that snare rattle...)
4.  The sound reverberating off the the surfaces in the room even after the "kick drum sound" itself is gone. (the snare is still rattling...)

I'm not saying all drum kits should have snare rattle, but it's a pretty consistent thing with a trap kit and should be recoginzed.

Also, a 4 part sound is a great simplification of a kick drum as there's a lot more going on.

But... if all of these sounds are mapped to MIDI velocity and no two hits on the 0-127 scale are exactly identical and velocities are triggered within pseudo random margins... See where this is going?

We can nest it further with as many sounds as we want, perhaps to account for pedal action or where on a cymbal or head a drum is hit, not just how hard.

![Acoustic 808](https://i.ytimg.com/vi/MpuNOAUjFcc/hqdefault.jpg)

_The legendary acoustic 808 bass drum sound_

## How people and wolves turn into robots

Cutting instrument noise and silence out of recordings (like editing studio drum tracks) [to me anyway] is a bit of a disservice to the instruments themselves as we've taken away 3 of the 4 fundamental parts of the sound and replaced the last artificially with a plugin. Cutting the intake of a breath of a singer (unless it's an annoying singer who needs editing) takes away a small but meaningful and important characteristic that reduces them just a little bit closer to a more sterile and robotic artificial instrument. The timbre of their voice may remain, but we'll EQ that and apply a generous amount of reverb in mixdown.

**This is the important part**, that when creating new textures, sounds and instruments that do not yet exist, that these subtle nuances will lead to a higher level of expression of an instrument. Currently, the most beautiful and expressive existing instruments, you simply can't take the [wolf note](https://en.m.wikipedia.org/wiki/Wolf_tone) out of a cello. You can try to reduce it artificially with an eliminator. However, the wolf is an imperfect and inherent part of the beauty. As is the breath of a human before they squirt the air back out through their [meat tube](https://www.mit.edu/people/dpolicar/writing/prose/text/thinkingMeat.html). _That looks like a risky click but it's not and it's worth it ;)_

## Philosophical Conclusion

The creative process, technical workflow and design can be approached as a Russian doll. With dolls of similar size or structure, each doll can be placed inside a different doll and experimented with non-destructively, taken apart, put back together with ease to create completely new dolls. Some dolls will still never quite fit together, however many unexpected combinations will.

**The ultimate goal should not be to model musical traditions of the past of harpsichords and rock bands or even humans in a modern digital enviorment, but to apply the values of past traditions to the new sounds of the future.**

A lot of these come in the form of imperfections and are a hidden yet cumulatively large part of the magic of music, collaboration, nature and in turn what makes things unique and special. We should stop seeking to polish them out, but within reason to embrace them creatively. I speculate that a lot of engineers and producers have been [polishing gems into turds](https://en.m.wikipedia.org/wiki/Nevermind) this whole time.

### _By the way..._

We can take these sets and work with them live (hence the name), improvisationally ourselves as we can be the players in a real room as well.

Also, Ableton is all about forward compatibility and you can [Arduino or OSC it](https://www.ableton.com/en/packs/connection-kit/) (there's a link about OSC above somewhere), or just hook apps into it in fruity ways if we wanted to get extra nerdy in parallel.

* * *

I will be presenting the _Dances with Wolf Tones Sonata_ this Friday at Rays Bar & Grill. Wear your nicest mask, like us on facebook and don't forget to smash subscribe.
