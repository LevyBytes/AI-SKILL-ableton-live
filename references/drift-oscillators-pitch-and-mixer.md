# Drift Oscillators Pitch And Mixer

Open when you need guidance on Drift Oscillators Pitch And Mixer in Ableton Live.

Context: [Oscillator Section](collision-and-drift-routes.md#3032-oscillator-section).

<a id="source-30321-oscillator-1"></a>
#### 30.3.2.1 Oscillator 1

Several hand-picked waveforms are available from the Osc 1 drop-down: Sine, Triangle, Shark Tooth, Saturated, Saw, Pulse, and Rectangle. Drift alone carries the Shark Tooth and Saturated waveforms; Shark Tooth draws on a vintage Moog analog shape of that name, while Saturated suits bass tones nicely.

Oscillator 1 is shifted by octaves with the Oct knob. Reach for the Shape knob to nudge the waveform’s harmonic makeup into something subtly altered, giving an outcome akin to pulse-width modulation. Because each waveform’s timbre differs, every one reacts in its own way to the Shape control. While you adjust it, the outcome shows up in the Waveform Display down at the foot of the Oscillator section. The waveform visibly morphs as you alter the Shape value.

Just past the Shape knob, the Oscillator 1 Shape Mod Source drop-down picks a modulation source to act on the Shape control, letting you reshape the waveform further:

- Env 1
- Env 2/Cyc - Either Envelope 2 or the Cycling Envelope serves as the modulator, whichever happens to be switched on.
- LFO
- Key - With the Shape Mod Amount on the positive side, taller note pitches yield greater modulation and lower ones yield less, and the relationship reverses once the amount goes negative.
- Velocity - Arriving velocity feeds the modulation; stronger note velocities yield greater modulation and weaker velocities yield less.
- Modwheel
- Pressure
- Slide

Modulation depth anywhere from -100% to 100% is dialed in using the Oscillator 1 Shape Mod Amount slider. Keep in mind that Shape Mod is able to add waveform modulation on its own at settings of 1% - 100%, even while the Shape control itself stays at 0%.

<a id="source-30322-oscillator-2"></a>
#### 30.3.2.2 Oscillator 2

Through the Osc 2 drop-down, you pick a waveform for the second oscillator from Sine, Triangle, Saturated, Saw, and Rectangle.

Oscillator 2 is shifted by octaves with the Oct knob, whereas the Detune control shifts it in semitones.

<a id="source-30323-pitch-mod"></a>
#### 30.3.2.3 Pitch Mod

A pair of modulation source slots, both acting on the pitch of the two oscillators, make up the Pitch Mod section. For a source, the Oscillator Pitch Mod Source drop-downs let you reach for any of Env 1, Env 2 / Cyc, LFO, Key, Velocity, Modwheel, Pressure, or Slide. How strongly each source drives the pitch, anywhere from -100% to 100%, is fixed by the Oscillator Mod Amount sliders.

Drive pitch with an LFO running in the Ratio time mode and you can produce FM tones.

<a id="source-30324-waveform-display"></a>
#### 30.3.2.4 Waveform Display

Drift’s Waveform Display.

What the waveform display renders is the merged output of Osc 1, Osc 2, and, when switched on, the noise generator. Tweak the oscillators and you will watch the waveform shift in the display.

<a id="source-30325-oscillator-mixer"></a>
#### 30.3.2.5 Oscillator Mixer

Drift’s Oscillator Mixer.

Within Drift’s Oscillator Mixer, switches let you switch on Oscillator 1 and 2 along with a noise generator that mixes white noise into the combined waveform.

Each oscillator and the noise generator also gets its own gain, set with the Osc 1, Osc 2, and Noise controls. With filter processing engaged, pushing oscillator gain high can hit the filters’ ceiling, or “headroom,” where they cease behaving linearly and yield an intricate distortion reminiscent of analog gear.

Two saturation stages within the filter circuitry are responsible for that distortion — one ahead of the filter and one behind it. Raising oscillator gain past its -6.0 dB default kicks in the first saturation stage, and the second engages once gain climbs above 0.0 dB.

Flipping the arrow toggles beside the gain controls turns on filter processing for the oscillators and noise generator. Leave filter processing off and the oscillator and noise output skips the filter altogether.

Retrigger for the oscillators is toggled on or off by the R toggle. With Retrigger on, each oscillator’s phase snaps back to a shared starting point whenever a note sounds; leave it off and the oscillators run freely.
