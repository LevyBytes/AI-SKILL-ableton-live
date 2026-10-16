# Drift LFO Modulation And Global Controls

Open when you need guidance on Drift LFO Modulation And Global Controls in Ableton Live.

Context: [Drift](collision-and-drift-routes.md#303-drift).

<a id="source-3035-lfo-section"></a>
### 30.3.5 LFO Section

Drift’s LFO Section.

Just like the Cycling Envelope, Drift’s LFO offers one of four distinct time modes: Rate, Ratio, Time, or Sync. Which mode is chosen sets the LFO’s cycle rate in Hz, ratio, milliseconds, or tempo-synced beat divisions.

Within the LFO display, nine waveforms are pickable from the drop-down:

- Sine
- Triangle
- Saw Up
- Saw Down
- Square
- Sample & Hold
- Wander is a sample and hold carrying an S-shape that eases between a pair of values at the LFO’s rate.
- Linear Envelope is a single-shot decay envelope whose decay is linear.
- Exponential Envelope is a single-shot decay envelope whose decay is exponential.

Retrigger is toggled on or off with the R switch. When on, the LFO snaps back to the same point in its phase each time a note fires. When off, the LFO runs freely.

Overall LFO intensity is set by the LFO Amount knob. A source for the LFO is picked from the LFO Modulation Source drop-down, while how strongly that source acts on the LFO is fixed by the LFO Modulation Amount slider.

<a id="source-3036-mod-section"></a>
### 30.3.6 Mod Section

Drift’s Mod Section.

Nearly every parameter in Drift can be modulated; within the Mod section you may pick as many as three modulation sources and their destinations.

Available sources, picked through the Modulation Source choosers, are Env 1, Env 2 / Cyc, LFO, Key, Velocity, Modwheel, Pressure, or Slide.

The Modulation Destination choosers expose the following targets. Among the oscillator and noise options are Osc 1 Gain, Osc 1 Shape, Osc 2 Gain, Osc 2 Detune, and Noise Gain. On the filter and rate side you will find LP Frequency, LP Resonance, HP Frequency, LFO Rate, Cyc Env Rate, plus Main Volume.

How strongly the chosen destination responds to the source, anywhere from -100% to 100%, is fixed with the Modulation Amount sliders.

<a id="source-3037-global-section"></a>
### 30.3.7 Global Section

Drift’s Global Section.

How the instrument behaves and performs overall is governed by Drift’s global controls.

Drift’s four Voice Modes are selectable through the Mode chooser:

_Poly_ assigns a single voice to each note and supplies as many as 32 voices of polyphony.

<a id="source-live-instrument-reference-part-3"></a>

_Mono_ sounds a single note at any moment, yet that note draws on four voices to build a unison character governed by the Mono Thickness setting. With the Mono Thickness slider, you balance the relative loudness of the four voices tied to each individual note. Set Thickness to 0 and a note sounds through a lone voice. Push Mono Thickness upward and the remaining three voices grow louder until each note carries them audibly. Whenever a fresh note arrives, it cuts off the prior note that is still sounding, assuming you continue to hold it.

_Stereo_ assigns two voices to each note and spreads them toward the left and right channels. The Stereo Spread slider controls the degree of panning spread distributed among the separate voices. Raise the amount and the voices separate further, which yields a broadening result.

_Unison_ gently detunes each note's four voices, treating them as independent of one other. With the Unison Strength slider, you set the extent of pitch deviation spread among the separate voices. Crank it up and each voice receives a greater degree of variation.

To cap how many voices may sound at once, choose a value from the Voices drop-down menu. Some Voice Modes draw on a larger voice count than the notes you actually trigger, so the resulting polyphony shifts based on whichever Voice Mode is active. As an illustration, with the Voices amount set to 32 voices:

- Poly mode applies 1 voice per note, giving a ceiling of 32-note polyphony.
- Stereo mode applies 2 voices per note, giving a ceiling of 16-note polyphony.
- Unison mode applies 4 voices per note, giving a ceiling of 8-note polyphony.

The Drift slider introduces a touch of variation into every voice, touching assorted facets of how that voice sounds, including pitch and filter cutoff. In Drift, each voice gets its own randomization applied to the oscillators and to filter frequency; turning the Drift control up or down scales that individual randomization. Push the amount higher and the spread between the oscillators and the filter grows wider, pulling the sound further out of tune.

With the Voice Mode set to Mono, you may switch on the Legato toggle so that starting a new voice shifts its pitch while leaving its envelopes untouched. The Glide slider governs how long overlapping notes take to glide their pitch toward the next arriving pitch whenever notes play legato.

The Volume knob fixes the instrument's overall loudness, whereas the Vel > Vol slider controls the degree to which volume responds to incoming MIDI note velocity.

With the Transpose slider you shift the global pitch by semitones across a span of -48 to 48 st. Turn on the Note PB toggle to activate per-note pitch bend. Turning Note PB off allows an MPE controller to work without pitch shifting according to finger placement. The PB Range slider establishes the global pitch bend span measured in semitones.
