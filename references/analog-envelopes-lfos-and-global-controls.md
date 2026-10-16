# Analog Envelopes LFOs And Global Controls

Open when you need guidance on Analog Envelopes LFOs And Global Controls in Ableton Live.

Context: [Analog](analog-and-collision-routes.md#301-analog).

<a id="source-3016-envelopes"></a>
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

<a id="source-3017-lfos"></a>
### 30.1.7 LFOs

Display and Shell Parameters for the two LFOs.

Analog's pair of LFOs serve as modulation sources for the oscillators, filters and amplifiers. As in the other sections, every LFO carries its own separate parameters.

The shell's LFO 1 and LFO 2 switches turn each LFO on or off, while the Rate knob governs how fast the LFO runs. A switch beside this knob flips the Rate between a frequency in Hertz and tempo-synced beat divisions.

Which waveform the LFO uses is picked with the display's Wave chooser, offering sine, triangle, rectangle and two kinds of noise. The first noise variety jumps between random values, whereas the second glides along smooth ramps. With Tri or Rect chosen, the Width slider lets you reshape the waveform's pulse width. Under Tri, small Width values lean the waveform toward an ascending sawtooth, while bigger values produce a descending saw. Set it to 50% and you get a flawless triangle. Rect behaves comparably. At 50% the waveform is a perfect square wave, with lower and higher values producing negative or positive pulses respectively. Note that Width turns off whenever the LFO's waveform is sine or one of the noise modes.

How long the LFO waits to begin after the note starts is governed by the Delay slider, while Attack determines how long the LFO takes to climb to its full amplitude.

Turn on Retrig and the LFO resets to the same point in its phase with every note you trigger. The waveform's phase is shifted by the Offset slider.

<a id="source-3018-global-parameters"></a>
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
