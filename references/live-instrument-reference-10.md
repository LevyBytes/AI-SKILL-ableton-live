# Live Instrument Reference (part 10)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Use the Finger Mass and Finger Stiff knobs to dial in the finger’s physical traits: the former governs how forcefully the finger presses against the string, while the latter controls how rigid the finger is. A separate Fret Stiff parameter handles the simulated rigidity of the fret.

#### 30.12.2.6 The Pickup Section

Tension’s Pickup Section.

This section emulates an electromagnetic pickup of the kind you’d encounter on an electric guitar or electric piano. Use the switch beside its label to enable or disable it. Its sole control is the Position slider, which behaves much like the equivalent parameter found in the Exciter and Damper sections. Setting it to 0% places the pickup right where the string ends; at 50% it sits beneath the string’s center. Smaller settings tend toward a thinner, brighter tone, whereas larger ones deliver greater body and depth.

The Body Section

Tension’s Body Section.

A string instrument’s body, or soundboard, exists to broadcast the vibrational energy coming off the strings. Depending on its dimensions and form, that body also shapes those vibrations like a filter. Certain instruments — the guitar being one — add an internal air cavity that lifts the low end.

Switching the Body section on or off is done with the toggle beside its label.

Through the Body Type chooser you pick among several body designs patterned on real-world instruments.

With the Body Size chooser you scale the resonating body anywhere from extra small (XS) up to extra large (XL). As a rule, larger body settings push the resonant frequency downward.

How long the body’s resonance rings out is governed by the Decay knob — turn it up for a longer tail.

The Str/Body knob balances the String section’s raw output against the version that has passed through the Body section’s filtering. Fully clockwise leaves nothing of the String section’s direct signal; fully counterclockwise essentially removes the Body section from the chain.

Two more knobs, Low Cut and High Cut, let you sculpt the body’s frequency response even further.

Tension’s Volume Knob.

Positioned to the right of the Body section, the Volume knob governs the instrument’s total output level. The same control is also reachable from the Filter/Global tab.

### 30.12.3 Filter/Global Tab

Tension’s Filter/Global Tab.

On Tension’s Filter/Global tab you’ll find a polyphonic filter complete with envelope, LFO, and MIDI modulation, alongside keyboard and portamento settings plus a built-in Unison audio effect.

Tension’s Filter Section.

The Filter section provides a deeply adjustable multi-mode filter positioned between the String and Body sections. On top of that, it can be driven by its own envelope generator and a low-frequency oscillator (LFO).

Keep in mind that a switch in the Filter subsection enables or disables the whole Filter section, whereas the Filter Envelope and Filter LFO sections come with separate toggles of their own.

Picking the filter type happens at the filter’s chooser. The available choices are low-pass, band-pass, notch, high-pass and formant filters, each offered in 2nd and 4th order.

Use the Freq slider to set the filter’s resonance frequency and the Res control to set how much resonance there is. With a formant filter active, the Res control steps through a series of vowel sounds. Both the Freq and Res controls accept modulation from LFO, envelope or note pitch by way of the sliders underneath. Bear in mind the LFO and Env sliders do nothing until the Envelope and LFO subsections have been switched on.

A switch beside its name turns the Filter Envelope subsection on or off. It follows the familiar ADSR (attack, decay, sustain, release) layout but adds a couple of wrinkles:

- The Attack knob defines the attack time, but the Vel slider sitting under it lets MIDI note velocity modulate that time too. Raising the Vel value makes harder-played notes attack progressively faster.
- After the attack stage, the Decay knob determines how quickly the envelope falls to the sustain level.
- Using the Sustain knob you set the level the envelope holds once decay finishes, lasting until the key lifts. All the way left removes the sustain stage entirely; all the way right removes the decay stage. Note velocity can also shape the sustain level through the Vel slider beneath the knob — larger settings raise the sustain level as velocity climbs.
- The Release knob defines release time, meaning how long the envelope takes to fall back to zero once the key is let go.

An extra modulation source for the filter comes from the Filter LFO subsection, which you enable or disable with the switch beside its name.

The waveform driving the LFO is chosen at the LFO waveform chooser, offering sine, triangle, rectangular and a pair of random waveforms. One random option jumps between random levels, while the other transitions with gentler ramps.

You set how fast the LFO runs with the Rate knob, and the switches under it flip the Rate between a frequency in Hertz and tempo-synced beat divisions.

Finally, the Attack knob governs how long the oscillator needs to climb to full amplitude, and the Delay knob governs how much time passes before the LFO kicks in after a note starts.

Tension’s MPE Section.

Within the MPE section you can route MPE pressure and slide data to destinations and define Tension’s global and per-note pitch bend ranges. Each of the three MPE sources carries an Activity LED that illuminates whenever Tension picks up an incoming MPE signal.

Both the Pressure and Slide sources let you pick two destinations to send their MPE data to, with the Amount sliders setting how much modulation is applied.

Through the Pitch Bend controls you set the modulation range for the global pitch bend together with the MPE per-note pitch bend (Note PB), expressed in semitones.

Tension’s Keyboard Section.

Everything to do with Tension’s polyphony, tuning, and MIDI parameters lives in the Keyboard section.

Coarse and fine tuning duties fall to the Octave, Semi and Detune controls. Octave shifts the whole instrument in octave steps, Semi moves it up or down by semitones, and the Detune slider nudges things one cent at a time (out to a ceiling of 50 cents in either direction).

How many voices are available is set by the Voices chooser.

Stretch reproduces a method called stretch tuning, a tuning tweak frequently applied to both electric and acoustic pianos. Leave it at 0% and Tension performs in equal temperament — meaning two notes form an octave when the higher note’s fundamental is precisely double that of the lower one. Because a real vibrating tine or string doesn’t resonate exactly as the theory predicts, equal temperament can sound “wrong“ on pianos. Dialing Stretch upward sharpens the upper notes while flattening the lower ones, producing a brighter character. Going negative mimics “negative“ stretch tuning, in which the upper notes flatten and the lower notes sharpen.

Pushing the Error slider up introduces more random tuning error on every note. Crank it high if you’re feeling nostalgic for your junior high school orchestra days.

Finally, Priority decides which notes get dropped once you exceed the maximum polyphony. With Priority set to High, incoming notes pitched above the notes already sounding take precedence, and the cull begins from the lowest pitch. The Low setting reverses this. Choosing Last favors whatever was played most recently, dropping the oldest notes when room is needed.

Tension’s Portamento Section.

Rather than letting pitch jump straight from one note to the next, the Portamento section makes it glide between them. Flip the switch beside its name to engage or disengage the effect.

The slide’s overall pace is governed by the Time slider.

Turn on Legato and the glide happens only when you strike the second note before letting go of the first.

Enabling Prop. (Proportional) ties the glide duration to the size of the interval between notes, so wider intervals glide more slowly than narrow ones. Switch it off and the glide time stays fixed no matter the interval.

Tension’s Unison Section.

With the Unison section you can layer several voices onto each note you play. The Unison toggle switches the whole section on or off.

Use the Voices switch to pick either two or four layered voices, and Detune to set how much tuning spread is applied across those layers. Modest amounts yield a gentle chorus, whereas large amounts offer yet another route to that youth-orchestra feel.

Raising the Delay amount introduces a lag before each layered voice comes in.

Tension’s Volume Knob.

Sitting in the corner, the Volume knob controls the instrument’s total output level. You can also get to this same control from the String tab.

### 30.12.4 Sound Design Tips

On the surface, Tension’s modular layout might look fairly familiar compared with other synths — a set of functional blocks passing a signal down a path and reshaping it along the way. The crucial thing to keep in mind, though, is that these blocks aren’t walled off from each other; adjusting a single parameter can ripple out and strongly affect another one elsewhere. As a result, certain parameter combinations will yield silence, and others will generate punishingly loud output — so take care when you set your levels!

It often helps, while working with Tension, to picture the sections as genuine parts of one physical object. Imagine a bow drawn slowly across a string with no damping — it may set that string in motion. Clamp the same string with a massive damper, however, and the bow has to move much faster to produce any result.

A good way to appreciate the range on offer is to dig into how the factory presets were built. It won’t take long to discover that Tension reaches well beyond plain string sounds.

### 30.13 Wavetable

The Wavetable Instrument.

Wavetable is a synth built around a pair of wavetable oscillators, a pair of analog-modelled filters, and a modulation system that’s capable yet easy to grasp. The aim is for it to suit players and sound designers no matter their level of synthesis know-how — straightforward enough to produce strong results quickly, while opening up an almost endless field of options the further you explore.

The Wavetable interface breaks down into three principal areas: the oscillators, each on its own tab; the two filters; and the modulation area, which is spread across three tabs. Clicking the button in Wavetable’s title bar reveals additional parameters in one view. Which parameters appear in the main Device View versus the expanded view depends on how your screen layout is dimensioned.

### 30.13.1 Wavetable Synthesis

Sound from Wavetable’s oscillators is generated through a method known as wavetable synthesis. At its core, a wavetable is just a freeform set of short, looping samples laid out side by side. Lock the oscillator onto a single one of those samples and a held note rings out with one fixed timbre. The technique’s real strength, though, emerges when you sweep across the samples in the table while the note sounds, giving a timbre that morphs as it plays. That makes wavetable synthesis an excellent fit for evolving, time-varying sounds.

### 30.13.2 Oscillators

The oscillators in Wavetable are tuned for the highest possible sound quality. Provided you apply no modulation, their unprocessed output is fully band-limited, so no aliasing artifacts appear regardless of the pitch you play.

Wavetable’s Oscillators.

A switch on each oscillator’s tab lets you enable or disable that oscillator on its own. Clicking the tab brings the oscillator into focus and exposes its parameters for editing.

Each oscillator’s total output level rides on its Gain slider, and its placement across the stereo image is handled by the Pan control. Coarse and fine tuning are dialed in with the Semi and Detune controls, with that tuning measured relative to the global Transposition slider.

Pick a wavetable by way of the choosers or the arrow buttons. The first chooser narrows you to a wavetable category, and the second drills down to a particular wavetable inside it. Once you hit the last entry in a category, the arrow buttons roll over to the next one automatically, letting you scroll straight through every wavetable using only the arrows.

You can broaden the oscillator section’s palette by importing any WAV or AIFF file to serve as a wavetable. Just drag a sample out of the browser and drop it onto the wavetable visualization. From then on the choosers and arrow buttons point at the folder that holds your imported sample, so you can swiftly preview the other samples sitting alongside it.

Imported samples are processed automatically by Wavetable to cut down on unwanted artefacts. You can skip that processing, though, by turning on the Raw mode switch. Raw mode comes in handy above all when you load files already crafted specifically to act as wavetables. That said, it can equally be “misused” to conjure unpredictable, noisy or glitchy textures.

Wavetable’s Raw Mode Switch.

A display in the middle of the oscillator tab visualizes that oscillator’s wavetable. Drag inside this display to jump to another spot within the wavetable, or alternatively move there with the Wave Position slider.

The wavetable visualization switch flips between two available visualization styles. Each conveys identical information, just rendered differently. In the linear view the waveforms stack from bottom to top with time advancing left to right, whereas the polar view draws them as loops running from the inside outward with time advancing clockwise.

Plentiful as the wavetable selection is, you can also reshape any wavetable’s sound itself using oscillator effects. Choose one of three effects in the chooser, then tune their parameters with the sliders on the right. These oscillator effects are:

- FM — Imposes frequency modulation on the oscillator. The Amt slider scales how strong that frequency modulation is, while the Tune slider sets the pitch of the modulating oscillator. At a tuning of 50% (and -50%) the modulating oscillator lands an octave above (or below) the main one. At 100% (and -100%) it sits two octaves above (or below). Anywhere in between leaves the modulating oscillator at inharmonic ratios, perfect for spawning gritty overtones.
- Classic — Offers two modulation flavors familiar from vintage analog synths. PW changes the waveform’s pulse width. Bear in mind that hardware synths usually only let you vary pulse width on square waves, whereas Wavetable allows it across every wavetable. Sync brings in a “hidden” oscillator that resets the phase of the one you hear, reshaping its timbre.
- Modern — Supplies two more ways to warp the waveform’s shape. Warp behaves much like pulse width, and Fold introduces wavefolding distortion.

Keep in mind that switching the effect type leaves the two effect parameter values where they are. That lets you hop between effects and audition how each process colors the timbre using identical settings.

### 30.13.3 Sub Oscillator

Wavetable’s Sub Oscillator.

Beyond its two primary oscillators, Wavetable also carries a sub oscillator. The Sub toggle switches it on or off, and the Gain knob sets its output level.

Reaching for the Tone control reshapes the sub oscillator’s timbre. Held at 0% it puts out a clean sine wave, and raising Tone adds harmonic content to the waveform.

The sub’s pitch follows the note you play together with the global Transpose value, though the Octave switches let you drop the sub one or two octaves lower.

### 30.13.4 Filters

The filters in Wavetable are a great tool for carving up the harmonically dense timbres the oscillators and their effects throw off. And because those oscillators also hand you the classic analog-synth waveforms, putting together a subtractive-style synth is a breeze.

Wavetable’s Filters.

You get an assortment of filter types in Wavetable — low-pass, high-pass, band-pass, notch, plus a distinctive Morph filter. Every filter can be set to either a 12 or 24 dB slope, and you can pick from a range of analog-modeled circuit behaviors, built together with Cytomic, that recreate the hardware filters of certain classic analog synths.

The Clean circuit is a top-quality, CPU-light design — the very same filtering found in EQ Eight — and it works with every filter type.

The OSR circuit is a state-variable design whose resonance is reined in by a distinctive hard-clipping diode. It’s patterned on the filters of a fairly uncommon British monosynth and is offered for all filter types.

The MS2 circuit relies on a Sallen-Key topology with soft clipping to cap resonance. Modeled on the filters of a celebrated semi-modular Japanese monosynth, it’s offered for the low-pass and high-pass filters.

The SMP circuit is a bespoke design tied to no specific hardware. Blending traits of both the MS2 and PRD circuits, it’s offered for the low-pass and high-pass filters.

The PRD circuit employs a ladder design and applies no deliberate resonance limiting. It’s modeled on the filters of a vintage dual-oscillator monosynth from the United States and is offered for the low-pass and high-pass filters.

Frequency and Resonance are the two filter parameters that matter most, the usual synth staples. Frequency picks the spot in the harmonic spectrum where the filter acts, and Resonance lifts the frequencies right around that spot. You can also set both Frequency and Resonance by dragging either of the filter dots within the filter display.

Engaging the low-pass, high-pass, or band-pass filter with any circuit other than Clean exposes an extra Drive control, which you can use to push gain or distortion into the signal ahead of the filter.

For the Morph filter there’s an added Morph control that continuously glides the filter type from low-pass through band-pass and high-pass to notch, then loops back to low-pass.

Filter routing lets you wire the filters together in different layouts for wildly varied sculpting approaches. Three routings are on offer:

- Serial — Sends every oscillator into Filter 1, then feeds Filter 1 into Filter 2. Sub goes to both filters.
- Parallel — Feeds the two main oscillators separately into Filter 1 and Filter 2. Sub goes to both filters.
- Split — Routes Oscillator 1 into Filter 1, while Oscillator 2 heads into Filter 2. Sub gets divided in two and supplied to both filters. Should either filter be switched off, you’ll still hear the matching oscillator’s signal. Split lets you process each filter on its own, which is handy when you’re after layered synth tones. And with the main oscillators turned off while both filters stay active, Split doubles as a way to lavish extra processing on the Sub oscillator.

### 30.13.5 Matrix Tab

By way of the Modulation Matrix you route modulation coming from Envelopes and LFOs — collectively the “internal modulation sources” — onto the instrument’s parameters, otherwise called the “modulation targets.”

Wavetable’s Matrix Tab.

Across the grid, modulation sources lie along the horizontal axis and modulation targets along the vertical one. Drag inside the grid to set how much modulation the chosen source sends to the chosen parameter.

Be aware that some parameters act as additive modulation targets while others act as multiplicative ones.

A parameter receives additive modulation according to this formula:

1. The outputs of a parameter’s modulation sources are summed together.
2. The summed modulation value is added to the current parameter value.

With additive modulation the values revolve around 0, where 0 is the “neutral” point. These values may run negative or positive. A source putting out both negative and positive values is a “bipolar” source, whereas one limited to positive values only is a “unipolar” source.

A parameter receives multiplicative modulation according to this formula:

1. The outputs of a parameter’s modulation sources are multiplied together.
2. The multiplied modulation value is multiplied with the current parameter value.

Here the neutral point is 1 and the floor is 0. The Wavetable manual flags multiplicative-modulation parameters wherever they occur.

Clicking a parameter on the instrument drops it into the matrix temporarily. Apply any modulation to it and it sticks around; leave it unmodulated and it vanishes again the moment you click a different parameter. Note as well that the Matrix tab and the MIDI tab draw on the same set of rows.

Clicking any of the modulation source headers sitting above the matrix whisks you straight to that source’s panel over in the Mod Sources tab.

The Time slider rescales the timing of every modulator at once. Negative settings speed up the envelopes and LFOs, positive ones slow them down. Modulating this value with an envelope or LFO won’t touch the modulator doing the assigning, yet that modulator continues to scale toward its other destinations.

Every source feeding the modulation matrix has its combined depth governed by the Amount slider, which itself behaves as a multiplicative modulation destination.

### 30.13.6 Mod Sources Tab

On the Mod Sources tab you tweak the Envelope and LFO settings, each covered in greater depth below.

Wavetable’s Mod Sources Tab.

Envelopes

The three Wavetable envelopes (Amp, Env 2 and Env 3) respond to Time and Slope parameters, and Env 2 and Env 3 add their own Value controls on top. You can also set the Time, Slope and Value parameters directly by dragging on the envelope display.

Attack is the time taken to climb from the initial value up to the Peak value, and the contour of that segment follows the Attack Slope value.

Decay is the time taken to fall from the Peak value down to the Sustain level, with the segment’s contour set by the Decay Slope value.

Sustain fixes the level held once the Decay stage finishes. The envelope lingers there until a Note Off comes in — unless you’ve chosen Trigger or Loop for the Loop mode, whereupon it presses on to the Release stage the moment that level is reached. Note that this is a multiplicative modulation destination.

Release is the time taken to reach the Final value once a Note Off occurs, the contour of that segment being set by the Release Slope value.

As noted earlier, Wavetable’s envelopes additionally give you parameters for adjusting the slope of each segment. A positive slope makes the envelope race ahead early on and ease off later; a negative slope holds it flat longer before accelerating toward the end. Set the slope to zero for a linear shape, where the envelope advances at a steady rate across the whole segment.

The Initial slider fixes the value the envelope departs from at the moment of triggering. Bear in mind it serves as a multiplicative modulation destination. You won’t find this control on the amp envelope.

The Peak slider fixes the value that caps off the Attack stage and kicks off the Decay stage. The amp envelope omits this control.

The Final slider fixes the value reached when the Release stage ends. Again, the amp envelope has no such control.

Three options await you in the Loop Modes drop-down:
