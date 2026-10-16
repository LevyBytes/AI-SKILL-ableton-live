# Resonators And Reverb

Open when you need guidance on Resonators And Reverb in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2831-resonators"></a>
### 28.31 Resonators

The Resonators Effect.

Built from five resonators operating in parallel, the Resonators effect imparts a tonal quality to whatever signal feeds it, with tuning possible in either semitones or scale degrees. Outcomes span everything from plucked-string colors to tones reminiscent of a vocoder. Support for [tuning systems](https://www.ableton.com/en/live-manual/12/using-tuning-systems/#using-tuning-systems) is included as well.

Before reaching the resonators, the signal is routed through a filter. You can pick from four filter shapes: low-pass, band-pass, high-pass, and notch. To set the chosen filter’s frequency, turn to the Frequency parameter.

Two distinct resonation modes are on offer. The realism of Mode A makes its resonation sound more natural, whereas Mode B yields a result that becomes particularly compelling once Resonator I’s Note parameter is dropped to lower pitches.

With the Decay parameter you control how long it takes for the resonators to fall silent once a signal arrives. Longer decay settings produce a more tonal, sustained result, much like an undamped piano string behaves. Just as a genuine string does, the decay length tracks pitch, so lower notes ring on longer than higher ones. Activating the Const switch holds the decay time fixed no matter the pitch.

Reach for the Color control to shift how bright the resulting tone sounds.

Both left and right input channels feed the first resonator; the left channel alone is handled by the second and fourth resonators, and the right channel by the third and fifth.

How the resonators are tuned hinges on whether [scale awareness](https://www.ableton.com/en/live-manual/12/live-concepts/#scale-awareness) has been switched on in the effect, or whether a tuning system happens to be active. Out of the box, the first resonator establishes the root pitch while the remaining four are tuned to it across musical intervals. With scale awareness on, the first resonator follows the active clip scale in octave 2 and the others are tuned relative to that pitch. With a tuning system engaged, the first resonator locks to an absolute pitch from the tuning, and the rest are tuned relative to it.

Use the Note parameter to fix the root pitch shared by every resonator. By default this pitch is expressed in semitones spanning C-1 up to C5. Switch on scale awareness and the pitch is instead given in scale degrees. With a tuning system active, the pitch reads as note indices drawn from that system’s set of pitches. For finer movement measured in cents, turn to the Resonator I Fine Tuning parameter.

Each resonator carries its own On/Off toggle plus a Gain control. Switching a resonator off frees up its CPU load. Disabling the first resonator leaves the rest unaffected.

From Resonator II through Resonator V, the resonators track the Note parameter set on Resonator I, yet each can be shifted on its own by ±24 semitones — or ±21 scale degrees when the effect is scale aware — via its individual Pitch control. The Resonator II–V Fine Tuning parameters supply further fine adjustment.

For output, the device offers Width, Gain, and Dry/Wet controls. Acting only on the wet signal, the Width parameter collapses the combined output of Resonators II-V to mono at 0.0%. Unless Dry/Wet sits at 0%, Gain governs the resonated signal’s level. The balance between processed and unprocessed signal is handled by Dry/Wet.

<a id="source-2832-reverb"></a>
### 28.32 Reverb

The Reverb Effect.

Reverb is an audio effect that recreates how a sound behaves acoustically as it reverberates inside a physical space.

Out in the physical world, reverberation arises when sound waves bounce off the hard surfaces around them, and as absorptive materials in their path subsequently reshape the tone of those waves. Digitally, though, that behavior is modeled through a mix of filters paired with modulated delay lines.

Fine control over every one of these elements is what the Reverb device offers, letting you build distinctive spaces for sound to move through — anything from a cozy recording room to a vast canyon and all points between.
