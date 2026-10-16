# Vocoder Carriers Bands And Controls

Open when you need guidance on Vocoder Carriers Bands And Controls in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2842-vocoder"></a>
### 28.42 Vocoder

The Vocoder Effect.

(Note: You won't find the Vocoder effect in the Intro and Lite Editions.)

A vocoder is an effect that fuses the frequency content of one audio signal (the _carrier_) with the amplitude shape of a second audio signal (the _modulator_). The modulator usually carries a distinct rhythmic feel, such as speech or drums, while the carrier is most often a harmonically dense synth tone like a string or pad. People reach for a vocoder most commonly to conjure ”talking synthesizer” or robotic voice sounds.

A vocoder operates by passing both the carrier and the modulator through banks of band-pass filters. It then reads the output level from each of the modulator’s filters and uses that to drive the volume of the matching carrier filter.

Place Live’s Vocoder on whichever track holds the audio you intend to serve as the modulator. From there, the Carrier chooser offers several possibilities for the carrier signal:

- _Noise_ draws on Vocoder’s built-in noise generator for the carrier. Choosing it brings up an X-Y display for shaping the noise’s character. Its horizontal axis tunes downsampling — drag leftward to lower the sample rate of the carrier’s output. Its vertical axis tunes the noise density — drag downward to thin it out.
- _External_ lets you tap any of the internal routing points available in the choosers underneath. This is the pick for the classic ”robot voice” sound.
- _Modulator_ feeds the modulator back in as the carrier. In effect it puts out a resynthesized take on the modulator signal, while still letting Vocoder’s sound-shaping controls reshape the tone.
- _Pitch Tracking_ turns on a monophonic oscillator that tunes itself to the modulator’s pitch. With the High and Low sliders you can hem in the frequency span the oscillator tries to follow. Pick sawtooth or one of three pulse waveforms and set the oscillator’s coarse tuning through the Pitch slider. Pitch tracking works especially well on monophonic modulators like melodic instruments or voices. Keep in mind the oscillator refreshes its frequency only on detecting a definite pitch, after which it holds that pitch until a fresh one arrives. So tweaking the oscillator’s parameters or forcing it to reset (say, when [grouping](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks) Vocoder’s track) may produce surprising shifts in the sound. On polyphonic material or drums, pitch tracking is mostly unpredictable (though it can be quite intriguing.)

Especially with external carrier sources, a vocoder’s output may shed a good deal of high end. Switching on the Enhance button brightens the tone by evening out the carrier’s spectrum and dynamics.

The Unvoiced knob sets the level of an extra noise generator, which rebuilds the pitchless parts of the modulator, such as ”f” and ”s” sounds.

Sens. governs how readily the unvoiced detector fires. At 100% the unvoiced noise generator stays on the whole time; at 0% only the primary carrier source plays. The Fast/Slow switch sets how rapidly Vocoder flips between unvoiced and voiced detection.

The wide central panel of Vocoder displays the levels of each band-pass filter. A click inside this panel lets you pull those levels down.

How many filters are in play comes from the Bands chooser. More bands sharpen the read on the modulator’s frequency content while drawing more CPU.

The Range sliders set the frequency span the band-pass filters cover. A reasonably wide span suits most sources, though you may want to trim the outer edges if the sound turns too shrill or boomy. The BW control fixes the filters’ bandwidth. At low percentages each filter narrows toward a single frequency; widening the bandwidth makes the filter bands overlap more. A bandwidth of 100% is the truest, yet figures above or below it can yield intriguing results.

The Precise/Retro switch flips between two filter behaviors. Under Precise mode every filter shares one gain and bandwidth. Under Retro mode the bands grow tighter and louder as frequency rises.

Gate fixes a threshold for the filterbank. Any band sitting under that threshold falls silent.

The Level slider lifts or trims Vocoder’s output.

Depth controls how much of the modulator’s amplitude envelope lands on the carrier signal. At 0% that envelope is thrown away; at 200% only the loud peaks come through; 100% gives ”classic” vocoding.

The Attack and Release controls govern how fast Vocoder reacts to amplitude swings in the modulator. Very quick settings hold onto the modulator’s transients but may breed distortion artifacts.

The Mono/Stereo switches set how many channels serve the carrier and modulator. Under Mono mode both carrier and modulator count as mono sources. Stereo keeps the modulator mono but runs the carrier in stereo. L/R runs both carrier and modulator in stereo.

The carrier filterbank’s frequencies can slide up or down through the Formant knob. With a voice as the modulator, slight Formant moves can shift the perceived gender of the source.

The Dry/Wet control balances the dry signal against the processed one.
