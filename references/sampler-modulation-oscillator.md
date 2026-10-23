# Sampler Modulation Oscillator

Open when you need guidance on Sampler Modulation Oscillator in Ableton Live.

Context: [The Pitch/Osc Tab](sampler-zones-and-playback-routes.md#30107-the-pitchosc-tab).

<a id="source-301071-the-modulation-oscillator-osc"></a>
#### 30.10.7.1 The Modulation Oscillator (Osc)

Each voice in Sampler comes with its own modulation oscillator capable of applying frequency or amplitude modulation (_FM_ or _AM_) to the multisample. This oscillator is fully equipped: 21 waveforms (picked from the Type chooser) plus a loopable amplitude envelope all its own for dynamic waveshaping. Keep in mind it does nothing but modulate — you never hear its output on its own. What reaches your ears is how that output acts upon the multisample.

_FM_: Under this mode, the modulation oscillator alters the frequency of samples, yielding richer waveforms that sound noticeably different.

_AM_: Under this mode, the modulation oscillator alters the amplitude of samples. Modulator frequencies below hearing range produce gentle or fast swings in volume level, whereas modulator frequencies within hearing range generate composite waveforms.

You steer the modulation oscillator through its Initial, Peak, Sustain, End, Loop, Attack and Time < Velocities parameters. The [Sample Playback](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sample-playback) section covers in depth how these operate. On top of that, the right-hand portion of the modulation oscillator section holds these controls:

_Type_: Pick the waveform for the modulation oscillator here.

_Volume_: Governs how strongly the modulation oscillator modulates the sample.

_Vol < Vel_: Incoming MIDI note velocity can drive the modulation oscillator’s Volume parameter. That sets the modulation's depth.

<a id="source-live-instrument-reference-part-8"></a>

_Fixed_: Switch this on and the modulation oscillator holds a constant frequency, set by the Freq and Multi parameters; played MIDI notes no longer shift that rate.

_Freq_: When Fixed is On, the Multi parameter scales this value to arrive at the modulation oscillator’s constant frequency.

_Multi_: When Fixed is On, this factor multiplies the Freq parameter to arrive at the modulation oscillator’s constant frequency.

_Coarse_: Broad tuning for the modulation oscillator’s frequency (0.125-48). It is accessible only while Fixed is Off.

_Fine_: Detailed tuning for the modulation oscillator’s frequency (0-1000). It is accessible only while Fixed is Off.
