# Meld Oscillators Macros And Envelopes

Open when you need guidance on Meld Oscillators Macros And Envelopes in Ableton Live.

Context: [Meld](impulse-and-meld-routes.md#308-meld).

<a id="source-3081-general-overview"></a>
### 30.8.1 General Overview

Thanks to its dual-layer design, Meld can run as many as two polyphonic synth engines simultaneously. The layout breaks into four primary areas: the engines, the modulation section, the filters, and the global mix controls. That modular-style arrangement not only makes it simple to inject texture and motion into your sounds, it also helps you stumble onto and hold onto happy musical accidents. A good way to start exploring what Meld can do is to mix and match waveform types and tinker with each engine’s modulation macros. If you want tighter control, try routing an engine’s parameters into its Modulation Matrix, or use an LFO device to automate the device’s macro knobs. The further you push the interplay of Meld’s two layers, the more the device starts to feel like yours.

To open Meld up, press the Toggle Expanded View button found in the device header. While expanded, every available modulation target and source is displayed. Flip between the engines with the A and B toggles. To carry parameter modulation values across from one engine to the other, use the Copy to A and Copy to B buttons. Hitting the X button wipes out all the active modulation values.

Meld in Expanded View.

<a id="source-3082-oscillators"></a>
### 30.8.2 Oscillators

Meld’s Oscillators.

You can switch each of Meld’s two engines on or off on its own using the switches found in the Engines section. Shutting off one of Meld’s engines also shuts off the matching filter over in the device’s Filters section. A filter, by contrast, can be toggled on or off without disturbing whether the engine tied to it is active.

Three pitch controls (Octaves, Semitones, and Cents) accompany each of Meld’s engines. Flip on the Use Current Scale toggle and the semitone indicator (st) becomes scale degrees (sd). These pitch controls let you build harmonic richness into your sound — say, by lifting an engine a full octave or a fifth, or by detuning it gently in cents.

Both Engine A and Engine B give you twenty-four oscillator types to pick from, six of them being [scale aware oscillators](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#settings-tab) tagged with a (♭♯). The lineup spans everything from basic sine wave generation oscillators to stacked wave swarms, intricate frequency modulation, noise looping, and ambient sound generation algorithms. You can pick Oscillator Types from an engine’s drop-down menu or step through them with the arrows on the Oscillator Types displays.

<a id="source-3083-oscillator-macros"></a>
### 30.8.3 Oscillator Macros

Meld’s Oscillator Macros.

Each of Engine A and Engine B carries two macro knobs of its own, and these shift in function based on whichever oscillator type is in play. Every one of the four oscillator macro knobs can be mapped to a MIDI controller for live use or to the LFO device for hands-free modulation. Internally, the Modulation Matrix can drive them too.

Two macro knobs, Shape and Tone, belong to the Basic Shapes oscillator. Shape sweeps the oscillator’s waveform across sine, triangle, saw, and square wave forms. Tone alters the pulse width of the source wave.

The Dual Basic Shapes oscillator carries two macro knobs, Shape and Detune. Shape sweeps the oscillator’s waveform across sine, triangle, saw, and square wave shapes. Detune lays a duplicate of that original wave on top and detunes it.

Two macro knobs, Shape and Rough, sit on the Noisy Shapes oscillator. Shape sweeps the oscillator’s waveform across sine, triangle, saw, and square wave shapes. Rough layers noise distortion over that source wave.

On the Square Sync oscillator you’ll find two macro knobs, Freq 1 and Freq 2. This pair of controls retunes the frequencies of the oscillator’s two synced square waves.

Two macro knobs sit on the Square 5th oscillator: 5th Amt and P Width. 5th Amt blends the oscillator’s starting square wave toward a second square wave pitched a perfect fifth higher. P Width alters the pulse width of the square wave that’s produced.

Two macro knobs, Tone and Aux, accompany the Sub oscillator. Tone reshapes the oscillator’s starting sine wave into a square wave. Aux layers a lower subharmonic sine wave beneath the original sine wave that’s produced.

The Swarm Sine, Swarm Triangle, Swarm Saw, and Swarm Square oscillators each offer two macro knobs, Motion and Spacing. Motion introduces modulation into the wave swarm that’s generated. As you raise the amount, Spacing crossfades through ever more elaborate chords.

The Harmonic Fm oscillator has two macro knobs, Amount and Ratio, which adjust the modulation amount and ratio within the frequency modulation algorithm.

Two macro knobs, Amount and Shape, sit on the Fold Fm oscillator. Amount alters the modulation amount within the frequency modulation algorithm, and Shape alters the shape of its carrier wave.

The Squelch oscillator carries two macro knobs, Amount and Feedback. Amount alters the modulation depth of the frequency modulation algorithm, while Feedback alters how much signal gets routed back into the device.

The Simple Fm oscillator has two macro knobs, Amount and Ratio, which respectively adjust the modulation amount and the depth within the frequency modulation algorithm.

Two macro knobs, Tone and Rate, belong to the Chip oscillator. Tone alters the oscillator’s pitch and pulse width. Rate alters how fast the chip interval in use runs.

Two macro knobs sit on the Shepard’s Pi oscillator: Rate and Width. Rate alters the speed and direction of the oscillator. From 0.0 up to 49.9 the movement falls, while from 50.1 up to 100.0 it rises. At 50.0 there’s no movement at all. Width alters how many octaves the oscillator spans.

The Tarp oscillator has two macro knobs, Decay and Tone, which adjust the algorithm’s decay amount and tonality.

The Extratone oscillator has two macro knobs, Pitch and Env Amount, which adjust the oscillator’s pitch and envelope behavior.

Two macro knobs, Rate and Fade, belong to the Noise Loop oscillator. Rate fixes how frequently fragments of differing noise loops appear. Push it higher and the oscillator turns to noise. Fade dials in the grain or roughness of the noise.

The Filtered Noise oscillator has two macro knobs, Freq and Width, which adjust the oscillator’s filter frequency and width.

The Bitgrunge oscillator carries two macro knobs, Freq and Mult. Freq tunes the frequency of the square wave that’s produced. Mult sets how many sub-octaves are generated relative to that original square wave. Turned all the way up, it produces no sub-octaves; turned all the way down, it produces a great many.

Two macro knobs, Density and Intensity, sit on the Crackle oscillator. Density fixes the average rate of crackles that are produced. Intensity tunes how loudness and brightness are spread across the crackles.

The Rain oscillator has two macro knobs, Tone and Rate. Tone fixes the resonance of the raindrop and wind sounds that are produced, which renders the oscillator tonal and responsive to the notes you play. Rate fixes how dense the generated raindrop sounds become.

Two macro knobs, Density and Spread, belong to the Bubble oscillator. Density fixes the rate at which bubbles are generated, and Spread fixes how random the size of the produced bubbles is.

The Chord oscillator stacks four sawtooth oscillators to build an assortment of chords. Its two macro knobs are Shape and Inversion. Shape sets the intervals separating the chord’s notes, whereas Inversion shuffles the order in which those notes sit. With the Use Current Scale toggle switched on in the device title bar, the chords that are produced draw from the notes of the chosen scale. With no scale chosen, a major scale applies, taking the incoming MIDI note as its root.

<a id="source-3084-envelopes-tab"></a>
### 30.8.4 Envelopes Tab

Engine A’s Amplitude Envelope.

Attack, Decay, Sustain, and Release controls come with each of Meld’s envelopes. You can set them by dragging the numeric readouts along the bottom of the Envelope section up or down, by typing a value on your computer keyboard, or by grabbing and moving the breakpoints on the envelope’s graphical display.

Shown in red, the Attack, Decay, and Release Slope controls can likewise be set by dragging the numeric readouts along the bottom of the section, by typing a value on your computer keyboard, or by grabbing and moving the diamonds positioned between the breakpoints on the Envelope section’s graphical displays.

The Amplitude and Modulation envelopes offer three Envelope Loop Modes. Under Trigger mode, every segment of the envelope runs through once a note arrives, and the chosen Sustain level is disregarded. Under Loop mode, the whole envelope cycles without ever holding the chosen Sustain level. Under AD Loop mode, only the Attack and Decay stages of the envelope cycle.

One extra group of parameters belongs to the Modulation envelope: the Initial, Peak, and Final levels. Together these fix where the envelope rests when it’s triggered and when it’s released, granting greater modulation flexibility.

Initial and Final Parameters in Engine B’s Modulation Envelope.

Switching on the Link Envelopes button ties together every engine’s Amplitude and Modulation envelopes. That’s handy when you want Meld’s two engines to behave as one instrument.
