# Wavetable Modulation MIDI And Unison

Open when you need guidance on Wavetable Modulation MIDI And Unison in Ableton Live.

#### 30.13.6.1 LFOs

Two LFOs are built into Wavetable, and each one is tuned separately using the controls covered below.

Wavetable’s LFOs.

Pick any of five LFO waveforms, then reshape whichever one you selected by dragging the Shape slider:

- Sine and Saw: Adds a rising or falling ramp to the curve.
- Triangle: Shifts the symmetry between Ramp and Saw, landing on Triangle at the midpoint.
- Square: Adjusts the pulse width.
- Random: Alters how the extreme values are distributed.

Use the Sync switch to choose whether the LFO Rate runs in Hertz or locks to the song tempo; the Rate slider then dials in the LFO frequency, expressed either in Hertz or as beat divisions. The LFO frequency can also be changed by dragging directly on the waveform display.

Amount controls how much LFO modulation reaches the signals coming in. Keep in mind that this acts as a multiplicative modulation destination.

Use the Offset slider to shift the LFO’s phase so it begins from a different point in the cycle. Bear in mind that Offset cannot be modulated.

The LFO Attack slider lets you set how long the LFO needs to fade in after a Note On triggers it.

Turning on the LFO Retrigger switch makes the LFO jump back to its origin, or initial phase, with every fresh MIDI note. Retriggering the LFO partway through a cycle can produce hybrid LFO shapes.

### 30.13.7 MIDI Tab

Routing MIDI to parameters can transform Wavetable into a lively performance instrument. Inside the MIDI Modulation Matrix, you can route MIDI modulation sources onto several of the instrument’s parameters at once (these are the “modulation targets”).

Wavetable’s MIDI Tab.

With Velocity assigned, Wavetable reads the velocity value of each arriving MIDI note and uses it to modulate the target parameters for as long as that note sounds.

With Note assigned, Wavetable takes the pitch of each arriving MIDI note and modulates the target parameters across the note’s lifetime. That pitch modulation is centered on C3. So if you route it to Filter Frequency at a modulation amount of 100%, the filter follows the played note exactly.

Pitch Bend, Aftertouch and Modulation Wheel: many MIDI controller devices carry these as physical controls. Lacking such hardware, you can still drive the parameters through [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#midi-controller-clip-envelopes).

With Random assigned, Wavetable modulates the target parameters using a fresh random value that is computed whenever a note fires.

Clicking a parameter on the instrument brings it into the matrix temporarily. Apply modulation to that parameter and it stays put in the matrix. Without any modulation applied, it drops out of the matrix the moment you click a different parameter. Remember that the Matrix tab and MIDI tab use the same set of rows.

### 30.13.8 Global and Unison Controls

The global controls in Wavetable govern how the whole instrument behaves and performs.

Wavetable’s Global Controls.

Transpose shifts the Wavetable instrument’s pitch up or down, measured in semitones.

Volume sets the instrument’s overall output level. Keep in mind that this is a multiplicative modulation destination.

Flipping the Poly/Mono toggle moves the instrument between a single legato-enveloped voice (Mono) and a polyphonic instrument (Poly).

Use the Poly Voices drop-down menu to cap how many notes may ring out at the same time. Note that Poly Voices only does anything while the Poly/Mono switch sits on Poly.

Glide governs how long overlapping notes take to glide their pitch toward the next note that arrives. Note that Glide only works while the Poly/Mono switch sits on Mono.

The Unison drop-down menu offers a choice among six unison modes, or none at all. These modes stack several oscillators carrying distinct phases, stereo placements, or wavetable positions to thicken the sound.

- Classic: Oscillators get detuned at even intervals and panned across alternating stereo channels.
- Shimmer: Oscillator pitches drift randomly over time for a shimmering, reverb-flavored result. A touch of wavetable offset is added on top for extra body.
- Noise: Like Shimmer, the pitches drift, but the jitter happens far quicker, producing noisy, breathy textures. A touch of wavetable offset is added for extra fullness.
- Phase Sync: Oscillators detune the way they do in Classic mode, yet their phases lock together at note start, yielding a bold sweeping phaser-style effect.
- Position spread: Each oscillator’s wavetable position fans out evenly by a set amount. A little detune is layered in as well for extra width.
- Random note: At each note start, the wavetable positions and detune amount for every oscillator are randomised.

The Voices slider controls how many oscillators run at once per wavetable oscillator. Adding voices thickens the tone, while fewer voices keep it cleaner.

The Amount slider scales how strong the unison effect is, behaving differently from one unison mode to the next. Keep in mind that this is a multiplicative modulation destination.

### 30.13.9 Hi-Quality Mode

Wavetable’s Hi-Quality Option.

Hi-Quality mode is switched on or off through Wavetable’s context menu.

With Hi-Quality off, Wavetable recomputes its modulation once every 32 samples. It also swaps in low-power variants of the Cytomic filters to trim CPU even further.

Running Wavetable with Hi-Quality off can reclaim as much as 25% CPU versus leaving it on, which suits large sets or sessions where low latencies matter.

Starting with Live 11.1, a freshly loaded Wavetable instance, along with any of its Core Library presets, defaults to Hi-Quality mode being off. That said, presets you made yourself or Live Sets saved earlier will keep loading Wavetable with Hi-Quality on, so their sound stays consistent with how earlier Live versions played them.

Note: With Hi-Quality mode turned on, you may notice slight differences in the sound.
