# Analog Oscillators Filters And Amplifiers

Open when you need guidance on Analog Oscillators Filters And Amplifiers in Ableton Live.

Context: [Analog](analog-and-collision-routes.md#301-analog).

<a id="source-3011-architecture-and-interface"></a>
### 30.1.1 Architecture and Interface

The figure that follows illustrates how signal moves through Analog:

Diagram of Analog’s Signal Flow.

At the heart of the synth, the main tone generators are a pair of oscillators plus a noise generator. Each of these can be sent on its own to a choice of two multi-mode filters, with each filter feeding into an amplifier. On top of that, you may route the signal path through the filters either in series or side by side in parallel.

Two low-frequency oscillators (LFOs) are also built into Analog and may apply modulation to the oscillators, filters and amplifiers. On top of this, every filter and every amplifier carries a dedicated envelope generator.

Analog's interface breaks down into two regions: a _display_ with a _shell_ wrapped around its entire perimeter. Whatever section you pick in the shell, that shell holds its key controls, and the display refreshes to present parameter visualizations along with extra controls for that chosen section. Beyond the synthesis modules, a Global section gathers broad performance settings — among them instrument volume, vibrato and polyphony — and an MPE section supplies controls for three MPE sources: pressure, slide and per-note pitch bend, letting you sculpt Analog's tone with an MPE-enabled controller.

<a id="source-3012-oscillators"></a>
### 30.1.2 Oscillators

Display and Shell Parameters for the two Oscillators.

The pair of oscillators in Analog rely on physical modelling to reproduce the flavor of old hardware oscillators. Since they depend on modelling rather than wavetables, aliasing does not occur.

In the shell, a switch marked Osc 1 or Osc 2 lets you activate or deactivate each oscillator on its own, and you set that oscillator's output level with the slider sitting just to the right of the activator.

How the oscillator's output divides between the two filters is governed by the F1/F2 slider. Place the slider at its midpoint and the signal splits evenly across both filters. Push it fully up or fully down and the signal goes solely to Filter 1 or Filter 2, in that order.

Which waveform the oscillator produces is picked with the Shape chooser, offering sine, sawtooth, rectangular and white noise. Selecting rectangular activates the Pulse Width parameter on the display, letting you alter the waveform's pulse width. Small Width settings yield an extremely narrow waveform that often comes across as thin or "pinched." Set it to 100% and the waveform becomes a flawless square, so only odd harmonics remain. An LFO can also modulate the pulse width through the slider beside Width, though that parameter becomes active only once the matching LFO is switched on.

Serving as coarse and fine tuning, the shell's Octave, Semi and Detune knobs each do their part. Octave shifts the oscillator in octave steps, whereas Semi moves it up or down by semitones. Detune works in single-cent steps (with a ceiling of three semitones (300 cents) in either direction).

The pitch of the oscillator responds to whatever you dial in for the Pitch Mod and Pitch Env parameters on the display. How strongly the LFO drives pitch is governed by the LFO slider — and once more, the parameter only works while the LFO is active. The Key slider sets how strongly incoming MIDI note pitch reshapes the oscillator's tuning. Leaving it at the default of 100% keeps the oscillator on a standard equal-tempered scale. Raising or lowering this figure widens or narrows the gaps between keyboard notes. Drop it to 0% and note pitch stops affecting the oscillator entirely. For a feel of the effect, hold one oscillator at 100% and nudge the other's Key scaling just a hair away. Now run some scales around middle C. Because C3 always fires the identical frequency no matter the Key setting, the two oscillators drift increasingly out of tune the further your playing strays from C3.

Over time, the Pitch Env controls impose a ramp that shifts the oscillator's pitch. Where the oscillator begins is set by Initial, and Time governs how long the pitch takes to slide to its destination value. Either parameter responds to its slider, or you can drag the breakpoints within the envelope display.

With the Sub/Sync controls on the display you can engage either a sub-oscillator or a hard sync mode. Setting the Mode chooser to Sub makes the Level slider govern the output of a supplementary oscillator pitched one octave under the main one. This sub-oscillator emits a square wave whenever the main oscillator's Shape is rectangle or sawtooth, and a sine wave when the main oscillator is on sine. Bear in mind that picking white noise for the main oscillator's Shape switches the sub-oscillator off.

Switch the Mode chooser to Sync and an internal oscillator — whose frequency the Ratio slider sets — keeps retriggering the oscillator's waveform. At 0% the internal and audible oscillators share a frequency, leaving sync inert. Pushing the Ratio higher speeds up the internal oscillator, which reshapes the harmonics of the audible oscillator. To squeeze out the gnarliest analog grit, assign a mod wheel or another MIDI controller to the Sync ratio.

<a id="source-3013-noise-generator"></a>
### 30.1.3 Noise Generator

Analog’s Noise Generator.

White noise is what the Noise generator outputs, and it carries a built-in -6db/octave low-pass filter of its own. You enable or disable the generator with the shell's Noise switch. The slider sitting to the right of that activator controls its output level.

Output from the noise generator is split between the two filters by the F1/F2 slider. Center the slider and an even share of signal reaches each filter. Drive it fully up or fully down and the signal arrives only at Filter 1 or Filter 2, respectively.

Frequency of the internal low-pass filter is set by the Color knob. Turning it up brings through more high-frequency content.

Keep in mind that Noise carries shell parameters only, so tweaking them leaves the display unchanged.

<a id="source-3014-filters"></a>
### 30.1.4 Filters

Display and Shell Parameters for the two Filters.

A versatile routing layout, several saturation choices and a wide range of modulation options come with Analog's pair of multi-mode filters. Just like the oscillators, every parameter is adjustable separately per filter.

Toggling each filter on and off is handled by the shell's Fil 1 and Fil 2 switches. Sitting beside the filter activator, the chooser sets the filter type, offering low-pass, band-pass, notch, high-pass and formant variants in both 2nd and 4th order forms.

You set the filter's resonance frequency using the shell's Freq knob, and the depth of resonance is dialed in with the Reso control. Pick a formant filter in the chooser and the Reso control sweeps through vowel sounds instead.

Sitting under each mode chooser is one more control, and it isn't the same on both filters. On Filter 1, the To F2 slider lets you set how much of Filter 1's output is passed along to Filter 2. The Follow switch underneath Filter 2's mode chooser ties this filter's cutoff frequency to that of Filter 1. Once enabled, Filter 2's cutoff knob then sets the offset separating the two cutoff values. Should any of Analog's modulation sources be driving Filter 1's cutoff, those sources reach Filter 2 as well while Follow stays on.

Beyond the [envelope](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#envelopes) controls, the filter displays house assorted modulation parameters together with the Drive chooser. Both cutoff frequency and resonance accept separate modulation from LFO, note pitch and filter envelope through the sliders found in the Freq Mod and Res Mod sections respectively. A positive modulation figure pushes the cutoff or resonance up, while a negative one pulls them down.

What flavor of saturation lands on the filter output is chosen with the display's Drive chooser. Its three Sym settings deliver symmetrical distortion, meaning saturation acts the same way for positive and negative values alike. The Asym settings yield asymmetrical saturation. Across both kinds, larger numbers mean heavier distortion. To bypass Drive completely, pick Off in the chooser. Try out the different settings to learn how each one colors an incoming signal.

<a id="source-3015-amplifiers"></a>
### 30.1.5 Amplifiers

Display and Shell Parameters for the two Amplifiers.

Once it leaves the filters, the signal heads to an amplifier that gives the sound further shape through an amplitude envelope and panning. Each amplifier's parameters can be dialed in separately.

The shell's Amp 1 and Amp 2 switches turn each amplifier on or off, and the Level knob handles output level. Where the amplifier's output sits across the stereo field is set by the Pan knob.

Alongside the envelope controls, the amplifier displays hold a range of modulation parameters. The Pan and Level values accept independent modulation from LFO, note pitch and amp envelope through the sliders within the Pan Mod and Level Mod sections respectively. Bear in mind that with note pitch driving Level, middle C stays the same no matter how much modulation you apply. A positive value boosts the level on higher notes.
