# Meld Filters And Resonators

Open when you need guidance on Meld Filters And Resonators in Ableton Live.

Context: [Meld](impulse-and-meld-routes.md#308-meld).

<a id="source-3089-filters"></a>
### 30.8.9 Filters

Meld’s Filters Section.

A dedicated filter, A and B, belongs to each of Meld’s two engines, and you can flip each one on or off on its own with the switches in the Filters section.

Where the filter’s cutoff frequency is centered is set by the Filter Frequency knob.

Seventeen different filter types are on offer through the Filter Type drop-down menu. Every filter carries two macro knobs, and these adjust according to the filter type you pick.

Q and Drive are the macro knobs you’ll encounter most often across Meld’s filters. Q controls how strongly the frequencies surrounding a filter’s cutoff frequency are emphasized. Drive feeds saturation into the input signal ahead of the filter stage, which comes in handy for generating distortion.

State variable filters, the SVF 12dB and 24dB filters use an L-B-H-N macro control that sweeps through this filter type’s four available shapes: low-pass, band-pass, high-pass, and notch.

The MS2 filters take their cue from a Sallen-Key circuit found in a well-known semi-modular Japanese monosynth, using soft clipping to keep resonance in check. Meld offers them in low-pass and high-pass forms.

Based on a state variable filter from an obscure British monosynth, the OSR filter holds its resonance back with a distinctive hard-clipping diode. Meld offers it in a band-pass form.

LP Crunch 12dB is a dual-mode low-pass filter that routes the distortion it generates back into its own path.

The LP Switched Res filter draws on low-pass filters in which the resistors give way to fast switches, yielding downsampling artifacts. The Lofi macro knob shifts the frequency of those filter resistors. Crank it high and the filter turns out a more crushed tone; keep it low and the result is smoother.

Filther is built around a low-pass filter that distorts both a signal’s input and its output. A hard diode clipper handles the input signal while soft saturation handles the output signal.

Working as peak and notch filters, the Eq Peak and Eq Notch filters impose gain and width upon a signal fed into them. On the Eq Peak filter, the Boost macro knob lifts frequencies surrounding the filter’s cutoff point. On the Eq Notch filter, the Cut macro knob trims frequencies surrounding the filter’s cutoff point.

The Phaser filter is a six-stage delayless inverted feedback phaser offering variable feedback and notch spacing. On the Phaser filter, the Feedback macro knob governs how much output gets routed back into the filter’s input. The Spread macro knob tunes how the filter’s notches are spaced out across the frequency spectrum.

The Redux filter is a resampler and bitcrusher providing a variable sample rate, quantization, and a knob governing how many resampling artifacts it turns out. The Crush macro knob fixes the bit depth of the filter’s output. The Lofi macro knob balances a filtered, sample rate-reduced take on the signal against the unfiltered, downsampled artifacts that Redux has turned out.

The Vowel filter is a formant filter that imitates the qualities of spoken vowels, offering several shapes you can sweep through with the filter’s Morph macro knob.

Operating as feedforward and feedback filters are the Comb + and Comb - filters. The Feedback macro knob governs how much feedforward or feedback travels from the filter’s delayed output back to its input. The Damp knob places a low-pass filter on the filter’s output to tame high frequencies.

<a id="source-live-instrument-reference-part-5"></a>

The Plate Resonator filter feeds the incoming signal through a bank of modal resonators tuned to a rectangular plate’s first 32 modes. Its macro knobs let you reshape the plate’s size, resonance, and dimension ratio. Switching on Filter Scale Awareness keeps the filter’s resonant peaks locked to scale.

The Membrane Resonator filter feeds the incoming signal through a bank of modal resonators tuned to a circular membrane’s first 32 modes. Its macro knobs let you reshape the membrane’s size, resonance, and high frequency damping. Switching on Filter Scale Awareness keeps the filter’s resonant peaks locked to scale.
