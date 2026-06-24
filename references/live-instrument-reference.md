# Live Instrument Reference (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 30. Live Instrument Reference

A range of purpose-built native instruments ships with Live, spanning devices that rely on physical modeling, FM synthesis, wavetable synthesis, and several other approaches.

For a grounding in how instruments work inside Live, see the [Working with Instruments and Effects](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects) chapter.

Keep in mind that each Live edition ships with its own [feature sets](https://www.ableton.com/en/live/compare-editions/); as a result, certain instruments described here might be absent from particular editions.

### 30.1 Analog

The Analog Instrument.

Analog is a virtual analog synthesizer that we developed together with Applied Acoustics Systems. Rather than cloning one particular vintage analog synth, our aim with this device was to gather the standout traits of several iconic classic synths inside a contemporary instrument. The way Analog makes sound is by modeling the individual pieces of the synthesizer using physical modeling. Such a technique applies physical law to recreate the manner in which an object or system generates sound. With Analog specifically, the formulas that capture the behavior of analog circuitry get computed live. No samples or wavetables are involved in Analog; instead, the CPU derives the audio on the fly from the current setting of every parameter. The upshot of this synthesis approach is exceptional tone, authenticity, warmth and responsiveness when played.

### 30.1.1 Architecture and Interface

The figure that follows illustrates how signal moves through Analog:

Diagram of Analog’s Signal Flow.

At the heart of the synth, the main tone generators are a pair of oscillators plus a noise generator. Each of these can be sent on its own to a choice of two multi-mode filters, with each filter feeding into an amplifier. On top of that, you may route the signal path through the filters either in series or side by side in parallel.

Two low-frequency oscillators (LFOs) are also built into Analog and may apply modulation to the oscillators, filters and amplifiers. On top of this, every filter and every amplifier carries a dedicated envelope generator.

Analog's interface breaks down into two regions: a _display_ with a _shell_ wrapped around its entire perimeter. Whatever section you pick in the shell, that shell holds its key controls, and the display refreshes to present parameter visualizations along with extra controls for that chosen section. Beyond the synthesis modules, a Global section gathers broad performance settings — among them instrument volume, vibrato and polyphony — and an MPE section supplies controls for three MPE sources: pressure, slide and per-note pitch bend, letting you sculpt Analog's tone with an MPE-enabled controller.

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

### 30.1.3 Noise Generator

Analog’s Noise Generator.

White noise is what the Noise generator outputs, and it carries a built-in -6db/octave low-pass filter of its own. You enable or disable the generator with the shell's Noise switch. The slider sitting to the right of that activator controls its output level.

Output from the noise generator is split between the two filters by the F1/F2 slider. Center the slider and an even share of signal reaches each filter. Drive it fully up or fully down and the signal arrives only at Filter 1 or Filter 2, respectively.

Frequency of the internal low-pass filter is set by the Color knob. Turning it up brings through more high-frequency content.

Keep in mind that Noise carries shell parameters only, so tweaking them leaves the display unchanged.

### 30.1.4 Filters

Display and Shell Parameters for the two Filters.

A versatile routing layout, several saturation choices and a wide range of modulation options come with Analog's pair of multi-mode filters. Just like the oscillators, every parameter is adjustable separately per filter.

Toggling each filter on and off is handled by the shell's Fil 1 and Fil 2 switches. Sitting beside the filter activator, the chooser sets the filter type, offering low-pass, band-pass, notch, high-pass and formant variants in both 2nd and 4th order forms.

You set the filter's resonance frequency using the shell's Freq knob, and the depth of resonance is dialed in with the Reso control. Pick a formant filter in the chooser and the Reso control sweeps through vowel sounds instead.

Sitting under each mode chooser is one more control, and it isn't the same on both filters. On Filter 1, the To F2 slider lets you set how much of Filter 1's output is passed along to Filter 2. The Follow switch underneath Filter 2's mode chooser ties this filter's cutoff frequency to that of Filter 1. Once enabled, Filter 2's cutoff knob then sets the offset separating the two cutoff values. Should any of Analog's modulation sources be driving Filter 1's cutoff, those sources reach Filter 2 as well while Follow stays on.

Beyond the [envelope](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#envelopes) controls, the filter displays house assorted modulation parameters together with the Drive chooser. Both cutoff frequency and resonance accept separate modulation from LFO, note pitch and filter envelope through the sliders found in the Freq Mod and Res Mod sections respectively. A positive modulation figure pushes the cutoff or resonance up, while a negative one pulls them down.

What flavor of saturation lands on the filter output is chosen with the display's Drive chooser. Its three Sym settings deliver symmetrical distortion, meaning saturation acts the same way for positive and negative values alike. The Asym settings yield asymmetrical saturation. Across both kinds, larger numbers mean heavier distortion. To bypass Drive completely, pick Off in the chooser. Try out the different settings to learn how each one colors an incoming signal.

### 30.1.5 Amplifiers

Display and Shell Parameters for the two Amplifiers.

Once it leaves the filters, the signal heads to an amplifier that gives the sound further shape through an amplitude envelope and panning. Each amplifier's parameters can be dialed in separately.

The shell's Amp 1 and Amp 2 switches turn each amplifier on or off, and the Level knob handles output level. Where the amplifier's output sits across the stereo field is set by the Pan knob.

Alongside the envelope controls, the amplifier displays hold a range of modulation parameters. The Pan and Level values accept independent modulation from LFO, note pitch and amp envelope through the sliders within the Pan Mod and Level Mod sections respectively. Bear in mind that with note pitch driving Level, middle C stays the same no matter how much modulation you apply. A positive value boosts the level on higher notes.

### 30.1.6 Envelopes

Analog’s Envelope Parameters.

On top of the pitch envelopes found in the oscillator sections, Analog provides separate envelopes for every filter and amplifier. The four envelopes share one identical set of controls, all of which live inside the display. Every envelope follows a conventional ADSR (attack, decay, sustain, release) layout and offers velocity modulation along with looping.

You dial in attack time with the Attack slider. Velocity can also influence this time by way of the Att < Vel slider. Pushing the Att < Vel figure higher makes attack times progressively quicker as velocity rises.

How long the envelope needs to descend to its sustain level once attack ends is set by the Decay slider.

The Sustain slider fixes the level the envelope holds from the close of the decay phase until the key is let go. Rotate this knob fully left and the sustain phase vanishes. Rotate it fully right and the decay phase disappears.

On top of that, velocity can shape the overall envelope level through the Env < Vel slider.

Even while a key stays held, the S.Time slider can pull the Sustain level downward. The smaller the value, the faster that Sustain level falls.

Release time, lastly, is dialed in with the Release knob. This governs how long the envelope takes to fall to zero once the key is released.

Toggling between linear and exponential shapes for the envelope segments is done with the Slope switches. The envelope visualization mirrors this change as well.

By default, every fresh note fires its own envelope starting at the top of the attack phase. Turn on Legato and a note struck while another is still held picks up the first note's envelope wherever it currently sits.

Switching on the Free button makes the envelope skip its sustain phase, jumping straight from decay into release. People often call this "trigger" mode, since it yields notes of uniform length no matter how long you hold the key. Free mode suits percussive sounds well.

While a key is held, the Loop chooser provides a handful of ways to repeat particular envelope segments. Choose Off and the envelope runs through every segment a single time with no looping.

Pick AD-R and the envelope opens with the usual attack and decay phases, but instead of holding at sustain level, it keeps cycling the attack and decay phases until the note ends, whereupon the release phase fires. ADR-R mode works much the same, except it folds the release phase into the loop for as long as you hold the key.

Bear in mind that across both AD-R and ADR-R modes, turning on Free makes notes act as though they are held down forever.

ADS-R mode runs the envelope without looping, yet replays the attack and release phases one additional time once the key lifts. Given brief attack and release times, this mode can mimic instruments that have audible dampers.

### 30.1.7 LFOs

Display and Shell Parameters for the two LFOs.

Analog's pair of LFOs serve as modulation sources for the oscillators, filters and amplifiers. As in the other sections, every LFO carries its own separate parameters.

The shell's LFO 1 and LFO 2 switches turn each LFO on or off, while the Rate knob governs how fast the LFO runs. A switch beside this knob flips the Rate between a frequency in Hertz and tempo-synced beat divisions.

Which waveform the LFO uses is picked with the display's Wave chooser, offering sine, triangle, rectangle and two kinds of noise. The first noise variety jumps between random values, whereas the second glides along smooth ramps. With Tri or Rect chosen, the Width slider lets you reshape the waveform's pulse width. Under Tri, small Width values lean the waveform toward an ascending sawtooth, while bigger values produce a descending saw. Set it to 50% and you get a flawless triangle. Rect behaves comparably. At 50% the waveform is a perfect square wave, with lower and higher values producing negative or positive pulses respectively. Note that Width turns off whenever the LFO's waveform is sine or one of the noise modes.

How long the LFO waits to begin after the note starts is governed by the Delay slider, while Attack determines how long the LFO takes to climb to its full amplitude.

Turn on Retrig and the LFO resets to the same point in its phase with every note you trigger. The waveform's phase is shifted by the Offset slider.

### 30.1.8 Global Parameters

Display and Shell Parameters for the Global Options.

Through the Global shell and display parameters you can tailor how Analog reacts to MIDI data, plus controls covering performance settings like vibrato and glide.

The shell's Volume control governs the instrument's total output. Serving as the overall instrument level, it can lift or cut what the amplifier sections put out.

Vibrato is switched on or off with the Vib switch, and the percentage slider beside it sets how deep the vibrato runs. At its core, Analog's vibrato amounts to an extra LFO, but it is wired directly to the pitch of both oscillators. Vibrato speed is set by the Rate slider.

Switching the vibrato on brings up four more Vibrato parameters on the display. The Delay slider controls the gap before vibrato kicks in once the note starts, while Attack governs how long vibrato takes to climb to full intensity. The Error slider injects a degree of random spread into the Rate, Amount, Delay and Attack parameters of the vibrato that each polyphonic voice receives. How much the modulation wheel sways vibrato intensity is set by the Amt < MW slider. That control works relative to whatever you set on the shell's vibrato amount percentage slider.

The shell's Uni switch engages the unison effect, layering several voices on each note you play. The Detune slider beside the switch sets how much tuning variation lands on every stacked voice.

Switching on unison brings up two more Unison parameters on the display. The Voices chooser picks either two or four stacked voices, while the Delay slider lengthens the lag before each stacked voice fires.

Glide is switched on or off with the Gli switch. It makes the pitch slide from one note to the next rather than snapping over instantly. With Legato active, the slide happens only when you play the second note before letting the first go. Overall slide speed is set by the Time slider.

Switching the glide on brings up an extra Glide Mode chooser on the display. Pick Const and the glide time stays fixed no matter the interval. Pick Prop (proportional) and the glide time scales with the gap between notes. Wide intervals glide more slowly than narrow ones.

Sitting on the display's left side, the four Quick Routing buttons offer a fast way to dial in frequently used parameter routings. The top-left choice sets up a parallel structure, where each oscillator drives only its own filter and amplifier. The top-right button is comparable, except each oscillator splits its output equally across both filters. The bottom-left choice sends both oscillators into Filter 1 and Amp 1, skipping Filter 2 and Amp 2 altogether. Lastly, the bottom-right choice builds a serial structure, with both oscillators feeding Filter 1, whose output then goes solely to Filter 2 and Amp 2.

Keep in mind that the Quick Routing choices leave untouched any tweaks you have made to the oscillator level, tuning or waveform parameters — all they change is how the oscillators route into the filters and the amplifiers that follow.

Every one of Analog's tuning and polyphony parameters sits in the display's Keyboard section. Acting as coarse and fine tuning, the Octave, Semi and Detune controls each play their role. Octave shifts the whole instrument in octaves, whereas Semi moves it up or down by semitones. The Detune slider trims tuning in single-cent steps (with a ceiling of 50 cents in either direction).

PB Range sets how far, in semitones, pitch bend modulation reaches.

Stretch reproduces an approach called stretch tuning, a frequent tuning tweak applied to electric and acoustic pianos. Set to 0%, Analog performs in equal temperament, where two notes lie an octave apart once the upper note's fundamental is precisely double that of the lower note. Raising the Stretch figure pitches upper notes higher and lower notes lower. The outcome is a brighter tone. Negative settings mimic "negative" stretch tuning, where upper notes flatten and lower notes sharpen.

The Error slider raises how much random tuning error gets applied to each note.

The Voices chooser fixes the available polyphony, while Priority decides which notes drop out once you exceed the polyphony ceiling. Set Priority to High and incoming notes pitched above the ones currently held take precedence, with the lowest pitches being cut first. Low does the reverse. A Priority of Last favors your most recent notes, dropping the oldest ones whenever necessary.

### 30.1.9 MPE Sources

Display Parameters for the MPE Sources.

Flipping the MPE switch within the display's Global section uncovers three MPE sources: Pressure, Slide, and NotePB (per-note pitch bend), each available to reshape Analog's tone further.

Using the two Pressure Destination choosers, you can send MPE pressure data to as many as two separate destinations. The MPE Pressure Amount sliders on the right let you dial in how strongly that MPE pressure data modulates the chosen destinations.

Slide likewise offers two Destination choosers, and each carries its own MPE Slide Amount slider that sets how strongly the MPE slide data shapes the target.

Whenever Analog takes in MPE pressure and slide data, the Pressure and Slide Activity LEDs light up to show it.

The Note PB slider fixes the span, in semitones, of per-note pitch bend.

### 30.2 Collision

The Collision Instrument.

Collision is a synthesizer that recreates the qualities of mallet percussion instruments. Built in partnership with Applied Acoustics Systems, Collision applies physical modeling technology to recreate the assorted sound-producing and resonant parts of real (or imagined) objects.

### 30.2.1 Architecture and Interface

Two oscillators named _Mallet_ and _Noise_ generate Collision's sound, and they drive a pair of separate (or linked) stereo _resonators_. The oscillators supply the opening portion of the sound, yet it is the resonator settings that shape the sound's character the most.

Bear in mind that should both the Mallet and Noise sections be switched off, Collision yields no sound at all.

Collision's interface splits into sections and tabs. Controls for the matching Mallet and Noise oscillators live in the Mallet and Noise sections. Parameters for each individual resonator sit in the Resonator 1 and Resonator 2 tabs.

Two separate low-frequency oscillators (LFOs) reside in the LFO tab, and each one is able to modulate several parameters. In a similar way, the MIDI/MPE tab routes MIDI pitch bend, modulation wheel and aftertouch messages — plus their MPE (MIDI Polyphonic Expression) counterparts — to a number of destinations.

Sitting to the right of the MIDI/MPE tab, a block of global parameters covers voice polyphony, note retrigger, resonator structure, and total output volume.

Note: Switching off sections and tabs you aren't using can free up CPU resources.

### 30.2.2 Mallet Section

Collision’s Mallet Section.

The Mallet section models a mallet striking a surface. Its parameters tune the physical traits of the mallet itself.

Use the Mallet button to flip the section on or off.

Volume governs the mallet's total output level. Pitch and velocity can modulate the Volume parameter when you set the Key and Vel sliders found in the MIDI tab.

Stiffness sets how hard the mallet is. Kept low, the mallet stays soft, giving fewer high frequencies and a longer, less defined hit. Raise the stiffness and the impact grows shorter while high frequencies build. Pitch and velocity may also modulate this parameter through the Key and Vel sliders in the MIDI tab.

Noise determines how much impact noise rides along with every mallet hit. It comes in handy for recreating the "chiff" of a felt-covered mallet head. The Noise parameter responds to pitch and velocity modulation via the Key and Vel sliders in the MIDI tab.

Color sets the noise component's frequency. The higher you go, the fewer low frequencies remain in the noise. Setting Noise to 0 renders this parameter inert.

### 30.2.3 Noise Section

Collision’s Noise Section.

As with the Mallet, the Noise section creates the opening impulse of Collision's sound. White noise comes out of the Noise oscillator and then runs into a multimode filter that has its own envelope generator. You may employ this section in place of the Mallet section, or alongside it.

Use the Noise button to flip the section on or off.
