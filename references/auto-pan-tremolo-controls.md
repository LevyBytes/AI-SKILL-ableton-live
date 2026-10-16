# Auto Pan Tremolo Controls

Open when you need guidance on Auto Pan Tremolo Controls in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-283-auto-pan-tremolo"></a>
### 28.3 Auto Pan-Tremolo

The Auto Pan-Tremolo Effect.

Auto Pan-Tremolo applies LFO modulation to the incoming signal’s stereo position or amplitude in order to build automatic panning, tremolo, and gating effects.

Two modes exist: _Panning_ and _Tremolo_. Under Panning mode, a pair of LFOs shift where the input signal sits across the stereo panorama by trading its amplitude back and forth between the left and right channels. Under Tremolo mode, one LFO varies the signal’s amplitude to produce changes in volume. Flip between the modes with their respective toggles. The LFO waveform along with the controls in the display refresh to match whichever mode is active and mirror its corresponding properties.

The Effect Can Be Used in Panning Mode or Tremolo Mode.

Below the LFO waveform, the live visualization displays the present stereo position under Panning mode or the present amplitude level under Tremolo mode. This lets you tell at a glance how the input signal travels across the left and right channels or how its amplitude rises and falls.

Through the Waveform drop-down, choose the LFO contour you want. On offer are Sine, then Triangle, Shark Tooth, Saw Up, plus Saw Down, the Square shape, Random, Wander, and finally S&H (Sample and Hold).

Choose one of the offered Time modes to fix the LFO’s rate: Rate, Time, Synced, Dotted, Triplet, or 16th. After you pick one, the matching modulation rate control beneath the drop-down refreshes to show the value linked to that mode. Under Time mode, for instance, the LFO’s period can be set anywhere between 100 milliseconds and 200 seconds, handy for building lengthy modulation cycles.

You can pick from two Stereo Offset modes: _Phase_ and _Spin_. Under Phase mode, each LFO waveform driving the left channel and the right one may be staggered by a chosen number of degrees. At 180° the LFOs sit fully out of phase, so that as one LFO arrives at its peak value the other rests at its minimum. Under Spin mode, the left and right channels drift apart steadily according to the chosen percentage. This introduces a gentle asymmetry across the two channels. Note that only Phase mode is on offer with the Random, Wander, and S&H waveforms.

With any of the beat-division-based Time modes active (Synced, Triplet, Dotted, or 16th), the Phase Offset control turns available and lets you slide where each LFO channel begins inside its cycle relative to the beat grid. This proves handy for nudging the modulation so it kicks in slightly ahead of or behind the beat.

With the Random, Wander, or S&H waveforms in use, Phase Offset behaves as a stereo width control and can be used to add variation across the channels.

The Invert toggle flips the LFO’s polarity. Switched on, the waveform’s positive and negative values are swapped, which in effect flips the waveform upside down. Under Panning mode, for example, inverting the Saw Up waveform yields a Saw Down waveform. Under Tremolo mode, the waveform’s peaks turn into valleys and the reverse. With ramp-shaped waveforms, switching Invert on yields a ducking effect, while leaving it off yields a gating effect.

Tremolo mode brings two extra options you can switch on to shape how the LFO modulation behaves: _Harmonic_ and _Vintage_.

The Harmonic and Vintage Tremolo Mode Toggles.

When Harmonic is on, the high and low frequencies get modulated in an alternating fashion instead of together. A set crossover at 600 Hz divides the signal into a pair of frequency bands.

When Vintage is on, the LFO varies the signal’s amplitude and a non-linear curve also shapes it, lending warmth and grit to the tremolo effect.

Beneath the display sit controls that adjust the LFO’s amount, rate, shape, attack, and reaction to the input signal’s level.

Use the Controls Below the Display to Adjust the LFO Modulation.

With the Amount control you set how strongly LFO modulation is applied to the arriving signal.

The control sitting to the right of the Amount control fixes the LFO rate. That control’s name and unit shift according to the chosen Time mode. As an example, it shows up as _Freq_ when Rate is picked and the value reads in hertz (Hz). Under Time mode it shows up as _Time_ with the value in milliseconds (ms). Under the Synced, Triplet, Dotted, and 16th modes it shows up as _Rate_ with the value in beat divisions.

Note that the Amount control’s value and the LFO rate are shared across the Panning and Tremolo modes and can’t be set on their own.

The Shape control molds the LFO waveform in a different way for each mode. Under Panning mode, positive Shape values drive each waveform toward its upper and lower extremes. This trims the overlap between the LFOs, so the handoff from one channel to the next grows more abrupt. Under Tremolo mode, positive values steadily round out the waveform into rounded peaks, while negative values steadily squeeze the peaks into an angular form. Pushed to its highest or lowest setting, the Shape control can form ramps that yield gating effects (when Invert is off) along with pumping effects (when Invert is on).

Use the Shape Control to Create Ramps for Gating and Ducking Effects.

<a id="source-live-audio-effect-reference-part-2"></a>

Once a transient is registered, the Attack Time slider governs the number of milliseconds required before modulation climbs to its peak depth. Setting a lengthy attack lets you confine the processing to the held tail of a sound while sparing the opening spikes. With Panning mode active, this keeps those spikes anchored at the center of the stereo image; under Tremolo mode, it protects their punch instead.

How strongly the incoming level steers the LFO rate is governed by the Dynamic Frequency Modulation slider. Push it positive and louder material speeds the LFO rate up; pull it negative and the rate slows down instead.
