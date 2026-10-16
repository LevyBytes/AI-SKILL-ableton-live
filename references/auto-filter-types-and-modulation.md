# Auto Filter Types And Modulation

Open when you need guidance on Auto Filter Types And Modulation in Ableton Live.

Context: [Auto Filter](amp-filter-and-pan-routes.md#282-auto-filter).

<a id="source-2821-filter-types"></a>
### 28.2.1 Filter Types

The Filter Type chooser lets you pick one of ten filters. The available choices are Low-pass, then High-pass, plus Band-pass, the Notch type, Morph, the DJ option, Comb, Resampling, Notch + LP, and lastly Vowel.

The Filter Type Chooser.

The Low-pass filter cuts back frequencies sitting above the cutoff. Use it to tame brightness or strip away high-frequency content. The slope can be toggled between 12 and 24 dB.

High-pass lets through frequencies sitting above the cutoff frequency while cutting back the lower ones. It comes in handy for stripping low-frequency rumble or making sounds thinner. The slope can be toggled between 12 and 24 dB.

The Band-pass filter passes only a narrow band of frequencies surrounding the cutoff, reducing both the lower and higher frequencies that fall outside that band. This lets you single out a slice of the spectrum or build resonant, concentrated tones. The slope can be toggled between 12 and 24 dB.

Notch cuts back a slim band of frequencies while leaving nearby frequencies mostly untouched. Reach for it to strip out particular frequencies or to produce gentle phasing-style effects. The slope can be toggled between 12 and 24 dB.

The Morph filter offers a continuous sweep from low-pass through high-pass filtering, passing through band-pass response in the middle. Four filter slopes are on offer: 6, 12, 24, and 48 dB.

The DJ filter folds low-pass and high-pass filtering together under a single bipolar control, much like the ones on certain DJ mixer. Pushing above zero removes low frequencies and lifts the highs, while going below zero strips out the highs and lifts the lows. Be aware that filter resonance shifts too: settings close to 0.0% give a slight bump of the boosted frequencies, and that bump grows steadily as the value heads toward -100% or 100%.

Comb lays down a row of peaks or notches spread over the frequency spectrum and, when modulated, can yield flanger-style effects.

The Vowel filter molds the tone toward something voice-like by accentuating particular formants.

The Resampling filter trims high-frequency content by repeatedly resampling the signal at a rate tied to the cutoff frequency, which brings about aliasing and sampling degradation.

Notch + LP merges a notch filter with a low-pass filter, so a slim band of frequencies gets reduced while high frequencies are simultaneously rolled off. The slope can be toggled between 12 and 24 dB.

You dial in the chosen filter’s cutoff frequency through the Freq control positioned above the Filter Type chooser. Note that the DJ filter omits Freq and instead supplies the Control knob, letting you glide the device smoothly from low-pass toward high-pass filtering. The Vowel filter swaps Freq for the Pitch control; with it you set how many semitones the formants are nudged upward or downward.

The majority of filter types carry a Res (Resonance) control that lets you dial in how much emphasis sits at the cutoff frequency. It does nothing for the Resampling filter type and is grayed out to signal that. The Vowel filter swaps it for the Formant control; use that to fix the spot within the vowel spectrum matching the vowels a, e, i, o, and u.

The Morph, Comb, Notch + LP, and Vowel filters add an extra Morph control whose setting governs how the chosen filter’s personality shifts over the control’s span. You can lean on it to glide smoothly among different filtering styles, with the outcome tied to the filter type:

- With the Morph filter, low Morph values give low-pass filtering, mid-range settings deliver band-pass filtering, and high values give high-pass filtering.
- With the Comb filter, you can move the filter onto either the peaks (using low Morph values) or the notches (using high Morph values) that show up at multiples of the chosen cutoff frequency.
- With the Notch + LP filter, you can shift where the notch sits in relation to the low-pass cutoff. When Morph values stay low, the notch begins further from the cutoff and creeps steadily nearer as the control’s value goes up. By 100% the notch lands right at the cutoff.
- With the Vowel filter, the Morph control lets you progressively even out the gain across the formants.

<a id="source-2822-filter-display"></a>
### 28.2.2 Filter Display

Sitting in the device’s center, the display draws the filter curve for the chosen filter type, the modulated filter curves for both the left and right channels, plus the live signal spectrum of the output. Dragging the handle adjusts the Freq and Res controls (or, with the Vowel filter, Pitch and Formant in turn).

The controls beneath the display split into two groups: the LFO controls and the Envelope control. Whenever a group is active, it also brings a set of parameters that appear along the bottom of the display.

Auto Filter’s Display with Envelope Parameters Visible.

<a id="source-2823-lfo-controls"></a>
### 28.2.3 LFO Controls

Auto Filter’s LFO Controls.

Auto Filter can drive the left and right channels with independent LFO modulation, letting the modulation be staggered across the stereo field. The LFO Stereo Mode toggle along the bottom of the display flips between the two stereo offset modes: Phase and Spin.

Phase holds both LFOs at one shared frequency yet can push the two LFO waveforms out of phase, producing stereo movement. You can stagger the left and right modulation channels in degrees with the LFO Phase control. At 180° the channels sit fully out of phase, so the moment one LFO hits its peak the other rests at its minimum. The Spin mode pulls the two LFO rates apart from one another by a percentage dialed in with the LFO Spin control. With Phase at 0° or Spin at 0%, the left and right channels receive identical modulation.

The LFO Phase Offset parameter lets you slide the starting position of both LFO channels along their waveforms. Bear in mind this parameter does anything only when the LFO time mode sits on tempo-synced beat divisions or sixteenth note values.

The LFO Quantization Mode chooser lets you make the modulation step rhythmically at fixed intervals (Steps) or follow the tempo (S&H). Under Steps, each LFO cycle is split into a count of intervals chosen with the LFO Steps control. Under S&H, the LFOs are quantized to the beat-time value dialed in with the LFO S&H parameter.

The LFO Amt control governs the degree to which the low frequency oscillators influence the filter. You can run the LFOs alongside the envelope follower or in place of it.

The Rate control governs the LFO frequency, expressed either in Hertz, in seconds, as tempo-synced beat divisions, or as sixteenth note values, according to whichever LFO time mode is picked through the Mode chooser. Note that with the mode on Time, the Rate control’s display name switches to “Time.”

Through the Wave chooser you pick the LFO’s waveform from this group of shapes: Sine (whose modulations stay smooth, with peaks and valleys that are rounded), then Triangle, Saw, Square, Ramp Up, then Ramp Down, Wander, plus S&H (which yields modulation values that are randomly positive and negative). Note that with Wander or S&H picked, the Spin control has no audible effect and is grayed out.

The Morph control reshapes the LFO contour. Note that once the S&H waveform is picked, this control gives way to the Smooth parameter, which lets you soften the waveform.

<a id="source-2824-envelope-follower-controls"></a>
### 28.2.4 Envelope Follower Controls

Envelope Controls in Auto Filter.

The envelope controls let you dictate the way the envelope modulation acts on the filter frequency.

The Envelope Attack slider sitting at the foot of the display determines how the envelope reacts to incoming signals that rise. Low settings give a quick reaction to input levels, while high settings smooth out any movement over time, yielding a looser, more gradual reaction. Picture it as lending inertia to the reaction.

The Envelope Hold toggle governs the way the envelope passes from the attack into the release phase. Switched on, the envelope finishes the whole attack phase ahead of beginning the release phase.

The Envelope Release slider lets you dictate how rapidly the envelope reacts to falling input levels. Lower settings make the envelope react sooner, whereas higher settings stretch out the envelope’s decay.

You can quantize the envelope modulation to beat-time values. To turn on envelope quantization, flip on the Envelope S&H toggle and then dial the quantization value with the Envelope S&H Rate slider.

You steer both the direction and the degree to which the envelope modulation acts on the filter through the Envelope control sitting below the display.
