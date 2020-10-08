[Back](../README.md)

# Audio Synthesis with Ableton

## Precursor

### Science Facts

-   For a vibrating guitar string the first harmonic is 2x the length of the string. The "Negative" portion of the wave is absent on the vibrating string
-   Fundimentals are do not contain lower levels of vibration. Harmonics exist only as multiples.

### Terminalogy

-   **Fundemental** - The lowest frequency produced by any instrument
-   **Harmonic** - A multiple of the fundimental frequency.
-   **Node** - the transient of each vibration. a 2nd level harmonic has 3 nodes. start, middle, end. On a guitar string, this would be the bridge and the nut. 2 nodes are required to produce a Fundemental.
-   **Antinode** the widest part of the wave. There is always 1 few antinode to each node.
-   **Complete wave** - The complete cycle of the wave. With a first level harmonic this does not exist on the vibrating string as only the "positive" portion of the wave usually exists.
-   **Transient** - A resting point at 0db where the wave goes from positive to negative.

#### Notations

-   **λ** - Anonymous Lambda Calculus Abstraction (Function) - A function that binds one variable to another through equivalence.
-   **->** - Forward implication. For example "A -> B" means A implies B (ie if A is true then so must B be true) The double sided arrows pointing both ways means both ways Implication.
-   **ϕ** Defines the phase relationship between 2 waves. `ϕ` 180° means that the waves have opposite phase.

In calculus, unlike programming, functions are always anonymous, meaning they aren't given names.

So the following pseudo code function:

```javascript
square_sum(x,y) = x2 + y2
```

Can be rewritten as:

```bash
(x,y) -> x2 + y2
```

#### Length to wave length relationships

**(nodes/ antinodes)**

-   Wavelength = (2/1) x L - Harmonic 1
-   Wavelength = (2/2) x L - Harmonic 2
-   Wavelength = (2/3) x L - Harmonic 3

#### How to determine harmonic frequency

```txt
speed = frequency x wavelength

speed = 400 Hz x 1.6 m

speed = 640 m/s
```

### The Harmonic series

The harmonic series is the basis for synth work. It's also the reason that music sounds good to us.

-   1 (1)
-   1, 5 (2-3) [ root & fifth]
-   1, 3M, 5, 7m (dominant 7th) (4-7, major 3rd + dom dom 4th)
-   Major scale (Major scale notes 1,2,3,4,5,6,7) (8-15)
-   all 12 diatonic notes [All 12 diatonic notes] \(16-31)
-   48 note Scale (4x subdivisions between each of the 12 diatonic notes)

### Frequency Cancelling & Reenforcement

-   two waves of the same frequency operating at 180° phase will cancel each other out.
-   200hz and 100hz with only second harmonic on the 100hz ocilator willcancel each other out
-   For each additional overtone the phase amount in operator needs to be divided by two.

## FFT (Fast Fourier Transform)

-   Amplitude will yield Volume
-   FFT is the Amplitude at different levels.

## Operator

A digital synth clone using 4 oscilators, 1 LFO, Filter and pitch bend

**Coarse Knobs** - Multiplies the played frequency by the number selected. Works as the series of overtones in the following order:

after each tone is introduced it is used in every octive after.

### Subtractive Synthesis

Taking away parts of the sound by cancelling or filtering them out.

0.5, 1, 2, 4, 8, 16, 32, 64 are the intervals

### Types of filters

1.  Low pass
2.  High pass
3.  Band pass
4.  Notch
5.  Morph Filter - Can change between the previous 4 types (holing option)

**12/ 24** - is the slope of the filters. 12 or 24 db per octive

### Low Frequency oscilator

Usually produces low frequencies below our hearing range. Sending the LFO only to the filter we can modulate the filter.

-   Rate - is the amplitude of the produced sinewave.
-   Rate - the frequency of the sinewave

### Where to start

Begin By choosing a complex wave form (Like a Saw D 64 or a Square 64)

Use the 4 independent oscilators for subtractive. (tetris line)

### Frequency Modulation (FM) Synthesis

**Using the triple (pyramid tetris piece)** - Set all oscillators to sine waves and tune the three carriers to 1, 2, and 4

## Physical Modeling

there are 3 physial modeling synths in Ableton

1.  **Electric** - Electric piano style
2.  **Tension** - String instruments
3.  **Collision** - Mallets

### Collision

Mallet style physical modeling

-   **2 resonators** - with things like beams, marimba, string
-   **excitator / mallet** - what you're going to "hit" the resonators with.

Start by picking a resonator and then adjusting the excitator.

### A better aproach

Corpus is a resonater very similar to the resonators in collison.

Pairing **Operator** with **Corpus**.

## References

-   <https://www.physicsclassroom.com/class/sound/Lesson-4/Fundamental-Frequency-and-Harmonics>
-   <http://synthesizeracademy.com/harmonics/>
