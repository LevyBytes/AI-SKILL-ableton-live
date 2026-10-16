# Sampler Filter Volume Envelope And Globals

Open when you need guidance on Sampler Filter Volume Envelope And Globals in Ableton Live.

Context: [Sampler](operator-and-sampler-routes.md#3010-sampler).

<a id="source-30108-the-filterglobal-tab"></a>
### 30.10.8 The Filter/Global Tab

The Filter/Global Tab.

<a id="source-301081-the-filter"></a>
#### 30.10.8.1 The Filter

Sampler includes a polyphonic filter that can optionally route through a built-in waveshaper. Within the filter section you can pick from several filter shapes: low-pass, high-pass, band-pass, notch, and the distinctive Morph filter. Every filter toggles between 12 and 24 dB slopes, and you can also choose among various analog-modeled circuit characters, created together with Cytomic, that reproduce the hardware filters of certain vintage analog synthesizers.

Clean is a refined, light-on-CPU circuit identical to the filtering in [EQ Eight](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#eq-eight). Every filter type can use it.

OSR is a state-variable circuit whose resonance is reined in by a distinctive hard-clipping diode. Modeled after the filters in a fairly uncommon British monosynth, it works with all filter types.

MS2 employs a Sallen-Key topology together with soft clipping to keep resonance in check. Patterned after the filters in a well-known semi-modular Japanese monosynth, it is offered for the low-pass and high-pass filters.

SMP is a bespoke circuit that follows no specific piece of hardware. Blending traits drawn from the MS2 and PRD circuits, it is offered for the low-pass and high-pass filters.

PRD relies on a ladder topology and applies no dedicated resonance limiting. Modeled on the filters of a classic dual-oscillator monosynth from the United States, it is offered for the low-pass and high-pass filters.

Frequency and Resonance are the two controls that matter most and are familiar from any synth. Frequency picks the spot in the harmonic spectrum where the filter acts, and Resonance lifts the frequencies surrounding that spot.

Whenever the low-pass, high-pass, or band-pass filter runs through any circuit other than Clean, a supplementary Drive control appears, letting you push gain or distortion into the signal ahead of the filter.

A dedicated Morph control accompanies the Morph filter, smoothly cycling the response from low-pass through band-pass and high-pass to notch before returning to low-pass.

Through dedicated entries in the Morph slider’s context menu, the Morph control can be snapped at once onto whichever position you need — low-pass, band-pass, high-pass, or notch.

Over on the right, a dedicated filter envelope can modulate the filter’s cutoff frequency across time. It behaves much like the Pitch/Osc tab envelopes, providing Initial, Peak, Sustain and End levels along with ADSR, Loop mode and slope points. The F. Env button switches this section on and off. The Amount slider governs how strongly the filter envelope acts on the cutoff frequency and must hold a non-zero value before the envelope produces any result.

A waveshaper sits beneath the Filter and is engaged with the Shaper button. The Type selector offers four shaping curves: Soft, Hard, Sine and 4bit. You dial in Shaper’s strength with the Amount slider. The button positioned above the waveshaper area also lets you flip the order of processing: point the triangle upward and the signal travels from the shaper into the filter; point it downward and it travels from the filter into the shaper.

<a id="source-301082-the-volume-envelope-and-global-controls"></a>
#### 30.10.8.2 The Volume Envelope and Global Controls

Operating globally, the volume envelope shapes the articulation of Sampler’s tones through the usual ADSR (attack, decay, sustain, release) parameters. Refer to the [Sample Playback](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sample-playback) section for an explanation of those parameters.

You can loop this envelope as well, using the Loop chooser. Once a Loop mode is active, the Time/Repeat slider takes on significance. Under Loop and Trigger modes, a note held past the close of the Decay stage sends the envelope back to its starting value. How quickly it travels from the Sustain level down to that starting value is governed by the Time parameter. Under Beat and Sync modes, a note held longer than the span set on the Repeat slider sends the envelope back to its starting value.

Acting across every sample, the Pan slider is a global pan control, and Pan < Rnd injects some randomness into that global pan placement. Time (Global Time Envelope) stretches or compresses, in proportion, the duration of all of Sampler’s envelopes. Time < Key (Global Envelope Time < Key) stretches or compresses that duration in proportion to the pitch of arriving MIDI notes.

Lastly, the Voices selector grants as many as 32 concurrent voices to every Sampler instance. You can switch on voice retriggering with the Retrigger button (R) located beside the Voices chooser. With it on, a note that is already sounding gets retriggered instead of spawning an extra voice. Enabling Retrigger can conserve CPU, particularly when a note carrying a long release tail is retriggered repeatedly in rapid succession.
