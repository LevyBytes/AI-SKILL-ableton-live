# Live Instrument Reference (part 4)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

You can drag samples onto any of Impulse’s sample slots straight from the browser or from the Session and Arrangement Views. As another option, every sample slot carries a Hot-Swap button for [hot-swapping samples](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#hot-swapping-samples). To remove a loaded sample, press the Backspace (Win) or Delete (Mac) key.

Once imported, samples map themselves automatically across your MIDI keyboard, so long as that keyboard is connected and recognized by Live. Pressing C3 fires the leftmost sample, with the remaining samples laid out in sequence across the octave spanning C3 to C4. With the Fold button on, Impulse’s eight slots show up labeled within the [MIDI Editor’s key tracks](https://www.ableton.com/en/live-manual/12/editing-midi/#editing-midi), regardless of whether a particular key track holds any MIDI notes. To shift this mapping away from its default, add a [Pitch](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#pitch) device; to reorder it instead, add a [Scale](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#scale) device.

Every one of the eight samples carries its own dedicated set of parameters, which sit in the region beneath the sample slots and become visible once you click a sample. Changes you make to a sample’s settings register only when the next note arrives — notes already sounding are left untouched. Keep in mind that this same logic governs how Impulse responds to parameter shifts coming from clip envelopes or automation, since those too take hold only as a fresh note begins. Should you instead need changes that evolve while a note sustains, the [Simpler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#simpler) instrument is the better choice.

Among Slot 8’s parameters is a Link button, sitting in the lower left corner, which ties slot 8 to slot 7. With these two slots linked, triggering slot 7 halts slot 8’s playback, and the reverse holds true as well. The intent behind this feature was a particular scenario (though naturally you can apply it elsewhere): emulating how a closed hi-hat cuts off an open one.

Hover the mouse over any slot and controls appear letting you play, solo, mute, or hot-swap it.

### 30.7.2 Start, Transpose and Stretch

The Start control sets the point at which Impulse starts playing a sample, and you can push it as far as 100 ms beyond where the sample truly begins. The Transp (Transpose) control shifts the sample’s transposition across a range of +/- 48 semitones, and you can drive it with the velocity of incoming notes or with a random value, both configured in the relevant fields.

The Stretch control runs from -100 to 100 percent. With negative values the sample contracts, and with positive ones it lengthens. You get a choice of two stretching algorithms here: Mode A suits low material such as toms or bass, whereas Mode B works better for high material like cymbals. MIDI note velocity can also drive the Stretch value.

### 30.7.3 Filter

The Filter section supplies a wide selection of filter types, and each one stamps a distinct sonic flavor onto the sample by stripping away particular frequencies. Where along the harmonic spectrum the filter takes effect is governed by the Frequency control, while the Resonance control lifts the frequencies sitting close to that point. A random value or MIDI note velocity can drive Filter Frequency.

### 30.7.4 Saturator and Envelope

The Saturator lends the sample a thicker, warmer, more analog quality, and you can toggle it on or off whenever you like. Boosting the signal and introducing distortion is the job of the Drive control. As a side effect, this tends to make most signals considerably louder, so you’ll generally want to offset it by pulling down the sample’s volume control. Pushing Drive to extremes on low-pitched material yields those classic, overdriven analog synth drum tones.

To shape the envelope, use the Decay control, whose ceiling is 10.0 seconds. Two decay modes ship with Impulse: Trigger Mode lets the sample decay alongside the note, whereas Gate Mode holds the envelope until a Note Off message arrives before it starts decaying. That latter mode comes in handy whenever you want decay lengths to vary, which is exactly what hi-hat cymbal sounds call for.

### 30.7.5 Pan and Volume

Every sample comes with Volume and Pan controls, governing amplitude and stereo placement respectively. You can modulate them both: Pan responds to velocity and a random value, while Volume responds to velocity alone.

### 30.7.6 Global Controls

Sitting to the right of the sample slots, these parameters act as global controls covering every sample under Impulse’s control. The instrument’s overall level is set by Volume, while Transp shifts the transposition across all samples. Time-stretching and decay for the whole set of samples fall under the Time control, which lets you morph between short and stretched drum sounds.

### 30.7.7 Individual Outputs

Drop a fresh instance of Impulse onto a track and its signal blends in with the other instruments and effects that feed that track’s audio chain. There are plenty of times when it’s preferable to pull the instrument, or just one of its drum samples, off on its own and route that signal to a track of its own. For instructions on doing this with Impulse’s combined signal or with its separate sample slots, consult the [Routing and I/O](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#tapping-individual-outs-from-an-instrument) chapter.

### 30.8 Meld

The Meld instrument device.

A flexible synthesizer, Meld brings two self-contained macro oscillator engines together inside a single device. Although it’s quick to call up familiar analog-flavored patches, where Meld really comes alive is in the wide range of synthesis and filtering approaches it invites you to stack and explore. Every engine in the device carries its own filter, envelopes, LFOs, and a Modulation Matrix that supports both MIDI and MPE, plus a pair of oscillator-specific macro knobs whose reach spans anything from straightforward overtone modulation to stranger territory such as noise loop fragmentation, chiptone pulsewidth, and raindrop generation density. The whole point of Meld is to deliver expressive, out-of-the-ordinary sounds steered by musical intent rather than by technical minutiae.

### 30.8.1 General Overview

Thanks to its dual-layer design, Meld can run as many as two polyphonic synth engines simultaneously. The layout breaks into four primary areas: the engines, the modulation section, the filters, and the global mix controls. That modular-style arrangement not only makes it simple to inject texture and motion into your sounds, it also helps you stumble onto and hold onto happy musical accidents. A good way to start exploring what Meld can do is to mix and match waveform types and tinker with each engine’s modulation macros. If you want tighter control, try routing an engine’s parameters into its Modulation Matrix, or use an LFO device to automate the device’s macro knobs. The further you push the interplay of Meld’s two layers, the more the device starts to feel like yours.

To open Meld up, press the Toggle Expanded View button found in the device header. While expanded, every available modulation target and source is displayed. Flip between the engines with the A and B toggles. To carry parameter modulation values across from one engine to the other, use the Copy to A and Copy to B buttons. Hitting the X button wipes out all the active modulation values.

Meld in Expanded View.

### 30.8.2 Oscillators

Meld’s Oscillators.

You can switch each of Meld’s two engines on or off on its own using the switches found in the Engines section. Shutting off one of Meld’s engines also shuts off the matching filter over in the device’s Filters section. A filter, by contrast, can be toggled on or off without disturbing whether the engine tied to it is active.

Three pitch controls (Octaves, Semitones, and Cents) accompany each of Meld’s engines. Flip on the Use Current Scale toggle and the semitone indicator (st) becomes scale degrees (sd). These pitch controls let you build harmonic richness into your sound — say, by lifting an engine a full octave or a fifth, or by detuning it gently in cents.

Both Engine A and Engine B give you twenty-four oscillator types to pick from, six of them being [scale aware oscillators](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#settings-tab) tagged with a (♭♯). The lineup spans everything from basic sine wave generation oscillators to stacked wave swarms, intricate frequency modulation, noise looping, and ambient sound generation algorithms. You can pick Oscillator Types from an engine’s drop-down menu or step through them with the arrows on the Oscillator Types displays.

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

### 30.8.4 Envelopes Tab

Engine A’s Amplitude Envelope.

Attack, Decay, Sustain, and Release controls come with each of Meld’s envelopes. You can set them by dragging the numeric readouts along the bottom of the Envelope section up or down, by typing a value on your computer keyboard, or by grabbing and moving the breakpoints on the envelope’s graphical display.

Shown in red, the Attack, Decay, and Release Slope controls can likewise be set by dragging the numeric readouts along the bottom of the section, by typing a value on your computer keyboard, or by grabbing and moving the diamonds positioned between the breakpoints on the Envelope section’s graphical displays.

The Amplitude and Modulation envelopes offer three Envelope Loop Modes. Under Trigger mode, every segment of the envelope runs through once a note arrives, and the chosen Sustain level is disregarded. Under Loop mode, the whole envelope cycles without ever holding the chosen Sustain level. Under AD Loop mode, only the Attack and Decay stages of the envelope cycle.

One extra group of parameters belongs to the Modulation envelope: the Initial, Peak, and Final levels. Together these fix where the envelope rests when it’s triggered and when it’s released, granting greater modulation flexibility.

Initial and Final Parameters in Engine B’s Modulation Envelope.

Switching on the Link Envelopes button ties together every engine’s Amplitude and Modulation envelopes. That’s handy when you want Meld’s two engines to behave as one instrument.

### 30.8.5 LFOs Tab

Engine A’s LFOs.

Two LFOs of its own come with each of Meld’s engines. You can dial in the rates of LFO 1 and LFO 2 in Hertz or lock them to tempo, and a Phase Offset slider nudges each LFO’s phase. With Retrigger switched on, the LFO begins again from the point fixed by the Phase Offset slider.

You choose LFO 1’s waveform from the LFO 1 Type drop-down menu, which offers six waveform types: Basic Shapes, Ramp, Wander, Alternate, Euclid, and Pulsate. You can sculpt these waveforms further with the LFO’s Rate knob and the two macro knobs beside it, whose behavior depends on the chosen waveform type.

There’s also the LFO 1 FX panel for modulating LFO 1. Each of the FX1 and FX2 drop-down menus holds eighteen effect types you can chain onto LFO 1 in series. You set how strongly an effect is applied through its matching macro knob. Be aware that LFO 1 and LFO1 FX can each serve as a standalone modulation source within Meld’s Modulation Matrix.

LFO 2 hands you six classic waveform types to pick from: Sine, Tri, Saw Up, Saw Down, Rectangle, Random S&H. Within Meld’s Modulation Matrix, LFO 2 can act as a third standalone modulation source.

### 30.8.6 Matrix Tab

Engine B’s Modulation Matrix.

Within the device, Meld’s Modulation Matrix is where you route modulation sources to modulation targets. You might, for instance, set Engine A’s LFO 1 to modulate its Volume, or have Engine B’s Modulation Envelope modulate its Filter Frequency.

The modulation sources run along the horizontal axis while the modulation targets run down the vertical one. To apply modulation between two parameters, click a cell and drag it up or down. Going negative speeds up envelopes and LFOs, while going positive slows them down. Keep in mind that certain parameters receive additive modulation, whereas others receive multiplicative modulation.

Clicking a parameter drops it into the Modulation Matrix. A parameter lands in the Modulation Matrix belonging to whichever engine is currently chosen via the Display Selector Tab. Any parameter that isn’t being modulated drops out of the Modulation Matrix the moment you click a different one.

### 30.8.7 MIDI and MPE Tabs

Engine A’s MIDI Tab.

Through Meld’s MIDI and MPE tabs you can press MIDI and MPE features into service as modulation sources, turning Meld into a responsive performance tool.

With Velocity chosen as a modulation source, Meld takes the velocity value of an incoming MIDI note and uses it to modulate its modulation target across the length of that note.

With Pitch chosen as a modulation source, Meld takes the pitch value of an incoming MIDI note and uses it to modulate its modulation target across the length of that note.

With Random chosen as a modulation source, Meld modulates its modulation target using a random value, freshly computed every time a note fires.

Many MIDI controller devices carry the Pitch Bend, Press, and Modulation Wheel hardware controls. Many MPE controller devices carry the Note Pitch Bend, Slide, and Press hardware controls. Lacking a MIDI or MPE controller, you can still drive these parameters through [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#midi-controller-clip-envelopes).

### 30.8.8 Settings Tab

Meld’s Engine Settings.

Three global settings live in Meld’s Settings tab, each adjustable on a per-engine basis: Osc Key Tracking, Scale Awareness, and Glide.

Oscillator key tracking is turned on or off by the Osc Key Tracking switch. With it on, an oscillator sounds the pitch of whichever incoming MIDI note it gets. With it off, an oscillator holds a fixed C3 pitch for every incoming MIDI note, or the scale’s root within the C3 octave should Scale Mode be on. This proves handy for, say, playing drones or percussive sounds.

Turning on the Phase Reset switch snaps the oscillator’s phase back to a fixed value at every new note. Enabling Phase Reset also unlocks the Phase Spread switch. With Phase Spread on, the oscillator’s starting phase gets spread according to the Spread modulation source in the Modulation Matrix. With Phase Spread off, the starting phase is pinned to zero.

The Scale Awareness section holds two switches you can turn on: Oscillator Scale Awareness and Filter Scale Awareness.

Turn on Oscillator Scale Awareness and the pitches driven by scale-aware oscillator types stay in scale as well. The (♭♯) tag flags the scale-aware oscillator types, namely Dual Basic Shapes along with all four swarm variants — Swarm Sine, Swarm Triangle, Swarm Saw, Swarm Square — plus Chip.

Switch on Filter Scale Awareness and the resonant frequencies of scale-aware filter types stay in scale too. These filter types, tagged with a (♭♯), are scale aware: Plate Resonator and Membrane Resonator.

Within the Glide section sit two glide modes — Portamento (Porta) and Glissando (Gliss) — together with a Glide Time control.

How long overlapping notes take to glide into the next incoming pitch is fixed by the Glide Time control. Glide works in both Mono and Poly modes.

With Portamento on, playing a note while another is still held causes the first note’s pitch to glide steadily into the pitch of the second. With Glissando on, playing a note while another is still held makes the first note’s pitch climb or fall into the second note’s pitch through discrete steps. If scale awareness is on, Glissando lays out those steps as scale degrees. Bear in mind that portamento and glissando are only heard once Glide Time sits at a value greater than zero.

### 30.8.9 Filters

Meld’s Filters Section.

A dedicated filter, A and B, belongs to each of Meld’s two engines, and you can flip each one on or off on its own with the switches in the Filters section.

Where the filter’s cutoff frequency is centered is set by the Filter Frequency knob.

Seventeen different filter types are on offer through the Filter Type drop-down menu. Every filter carries two macro knobs, and these adjust according to the filter type you pick.

Q and Drive are the macro knobs you’ll encounter most often across Meld’s filters. Q controls how strongly the frequencies surrounding a filter’s cutoff frequency are emphasized. Drive feeds saturation into the input signal ahead of the filter stage, which comes in handy for generating distortion.

State variable filters, the SVF 12dB and 24dB filters use an L-B-H-N macro control that sweeps through this filter type’s four available shapes: low-pass, band-pass, high-pass, and notch.

The MS2 filters take their cue from a Sallen-Key circuit found in a well-known semi-modular Japanese monosynth, using soft clipping to keep resonance in check. Meld offers them in low-pass and high-pass forms.

Based on a state variable filter from an obscure British monosynth, the OSR filter holds its resonance back with a distinctive hard-clipping diode. Meld offers it in a band-pass form.

LP Crunch 12dB is a dual-mode low-pass filter that routes the distortion it generates back into its own path.

The LP Switched Res filter draws on low-pass filters in which the resistors give way to fast switches, yielding downsampling artifacts. The Lofi macro knob shifts the frequency of those filter resistors. Crank it high and the filter turns out a more crushed tone; keep it low and the result is smoother.

Filther is built around a low-pass filter that distorts both a signal’s input and its output. A hard diode clipper handles the input signal while soft saturation handles the output signal.

Working as peak and notch filters, the Eq Peak and Eq Notch filters impose gain and width upon a signal fed into them. On the Eq Peak filter, the Boost macro knob lifts frequencies surrounding the filter’s cutoff point. On the Eq Notch filter, the Cut macro knob trims frequencies surrounding the filter’s cutoff point.

The Phaser filter is a six-stage delayless inverted feedback phaser offering variable feedback and notch spacing. On the Phaser filter, the Feedback macro knob governs how much output gets routed back into the filter’s input. The Spread macro knob tunes how the filter’s notches are spaced out across the frequency spectrum.

The Redux filter is a resampler and bitcrusher providing a variable sample rate, quantization, and a knob governing how many resampling artifacts it turns out. The Crush macro knob fixes the bit depth of the filter’s output. The Lofi macro knob balances a filtered, sample rate-reduced take on the signal against the unfiltered, downsampled artifacts that Redux has turned out.

The Vowel filter is a formant filter that imitates the qualities of spoken vowels, offering several shapes you can sweep through with the filter’s Morph macro knob.

Operating as feedforward and feedback filters are the Comb + and Comb - filters. The Feedback macro knob governs how much feedforward or feedback travels from the filter’s delayed output back to its input. The Damp knob places a low-pass filter on the filter’s output to tame high frequencies.
