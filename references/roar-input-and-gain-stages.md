# Roar Input And Gain Stages

Open when you need guidance on Roar Input And Gain Stages in Ableton Live.

Context: [Roar](redux-resonators-reverb-and-roar-routes.md#2833-roar).

<a id="source-28331-input-section"></a>
### 28.33.1 Input Section

Roar’s Input Section.

How hot the signal arrives at Roar ahead of the gain stages is set by the Drive knob. You might use it to dial distortion up or down in a hurry — instead of tweaking each Shaper Amount control across several gain stages, say — or to reshape an input so a preset responds the way it should.

Tweaking the Tone Amount knob shifts how the input weighs its high against its low frequencies. Turn it positive and the highs come up while the lows drop back. Turn it negative and the lows rise while the highs are pulled down.

The corner frequency of the low shelving filter that the Tone Amount control relies on is set with the Tone Frequency slider.

Because the gain stages sit after the Input section in Roar’s signal path, moving Roar’s Tone parameters audibly recolors them. Pushing the Tone Amount knob into positive territory can, for instance, trim low-end on guitars or basses so heavy distortion doesn’t turn muddy.

Sitting beside the Tone Amount control, the Color Compensation toggle imposes a mirrored copy of the Tone filter onto the output of Roar’s distortion stages. With it on, Tone values get cut ahead of the shaper and lifted afterward, handing you tighter command over the gain stage processing. One handy move is engaging the Color Compensation toggle alongside negative Tone values to saturate drums while leaving their low-end punch intact.

Seven routing types are available from the Routing Mode panel: _Single_, _Serial_, _Parallel_, _Multi Band_, _Mid Side_, _Feedback_, and _Delay_. Every routing mode except Single and Multi Band carries a Blend control for setting the mix between its pair of gain stages.

In the Serial routing mode, the input runs through two shapers placed back to back. Here the Blend control fades between Stage 1 on its own and Stages 1 and 2 working together.

The Parallel mode runs the input through two shapers operating independently. Its Blend control crossfades between the Stage 1 sound and the Stage 2 sound. For a fun experiment, pick two markedly contrasting Shaper Curves — Half Wave Rectifier and Fractal, perhaps — and modulate the Blend control so Roar slides seamlessly from one to the other.

With Multi Band, the spectrum is divided into three independently processed bands: Low, Mid, and High. A pair of Crossover Filters (Low and High) sets where those three bands hand off to one another. The mode lends itself to many tasks, drum processing and saturating whole mixes among them.

Mid Side treats the input’s mono and stereo content separately. It comes in handy when you want to widen a signal’s stereo image while keeping the sound at the dead center of the field intact.

In the Feedback routing mode, the input and its feedback are processed apart from one another, which can yield unexpected tones or recast Roar as a distinctive delay. As an example, drive Roar’s Shaper Amount from an envelope for saturation with a shuffled delay feel, or nudge Shaper Bias slightly to build delays that erode over time.

Under the Delay mode, the second stage works on the delayed signal handed over by the first. That delayed signal reaches the second stage without the feedback gain scaling it, giving you single distorted repeats or slapbacks. The second stage’s output then loops back into itself, scaled by the feedback gain, which yields multiple repeats and lengthy tails.

<a id="source-28332-gain-stage-section"></a>
### 28.33.2 Gain Stage Section

Roar’s Gain Stage Section.

Every routing mode supplies its own collection of gain stages, and you can enable or disable each one on its own through the Stage toggles found in the Gain Stage tabs.

The same trio of controls appears on every Gain Stage tab: Shaper Amount, Shaper Bias, and Filter Frequency. You pick the Shaper and Filter Types from the drop-down menus along the bottom edge of each Gain Stage tab.

How much saturation hits the input is governed by the Shaper Amount control. You can also drag the shaper waveform directly in the Shaper Visualization display to set this value. Distortion kicks in once the input reaches the curve’s non-linear regions on screen.

By offsetting the signal, the Shaper Bias control produces asymmetrical distortion. Push it higher and it can mimic a faulty circuit. Take it to extremes and the signal drops to total silence.

Twelve curves are available from the Shaper Type drop-down menu beneath the Shaper Visualization display:

_Soft Sine_ leans on a sinusoidal curve to lend the input gentle, warm saturation. Even driven hard, this curve generally keeps its agreeable, analog-flavored distortion.

_Digital Clip_ lays a hard clipping curve over the input. As the signal hits the curve’s outer edges, it spits out coarse, higher-order harmonics.

_Bit Crusher_ recreates the signature distortion you get when quantized amplitudes meet an input signal, much like Live’s Redux device. Raising the Shaper Amount cuts the bit count used for quantization and pushes the built-in compander of the bit crusher harder. Pairing this curve with bias modulation works nicely, and it makes its presence felt most on quieter material.

_Diode Clipper_ this type emulates an analog clipping circuit virtually. It carries the same smooth warmth as the Soft Sine curve, only with its high end rolled off.

_Tube Preamp_ captures the gentle, analog saturation of a valve preamp. Transients and dynamics survive intact even with the Shaper Amount cranked up.

_Half Wave Rectifier and Full Wave Rectifier_ deliver striking, waveshaper-flavored results. Half Wave Rectifier hits the input with fully asymmetrical distortion, great for putting crunch into drums. Full Wave Rectifier lifts the signal an octave, handy for thickening certain synth parts with extra harmonic weight.

_Polynomial_ travels between a sinusoidal curve and richer waveforms. This curve responds well to modulation and excels at metallic tones.

_Fractal_ pours a heavy dose of high-end harmonics into the input.

_Tri Fold_ this type acts as a triangular wavefolder. As Fractal does, it loads the input with plenty of high-end harmonics, yet pushes toward a rougher, more distorted outcome.

_Noise Injection_ layers stereo noise ahead of smooth distortion on the input. The curve is well suited to smooth saturation that still carries some grit and grime.

_Shards_ keeps reshaping the slope of its stereo curve segments to chop the input apart rhythmically.

You can also switch shapers on or off using the toggle along the bottom of the Shaper Visualization display.

To make up for level shifts that arise as you reshape the curve, reach for the Shaper Level control.

The filter’s cutoff is set by Filter Frequency. Switch the Pre toggle on and the filter lands ahead of the Shaper stage. With Pre engaged, changing Filter Frequency leaves the harmonics the shaper generates untouched.

The lineup runs to nine filter types. The first three are _LP_ for low-pass, _BP_ for band-pass, and _HP_ for high-pass; rounding out the set are _Notch_, _Peak_, _Morph_, _Comb_, _Resampling_, plus _Dispersion_.

Frequencies sitting above the cutoff are cut by the LP filter; BP trims away the lows and highs outside a chosen band, and HP removes anything beneath the cutoff.

A slim band of frequencies is cut by Notch, while everything around it stays mostly intact.

Seamless morphing from low-pass through to high-pass, passing through band-pass along the way, is what the Morph filter provides.

Comb lays down a row of notches across the spectrum. Modulate its cutoff and the filter can deliver flanger-style effects.

The Resampling filter introduces sample-rate reduction artifacts, akin to Live’s Redux device.

Dispersion nudges separate frequencies forward in time by varying amounts while leaving their levels alone. That slight skew between frequencies can yield metallic, spring-like tones, all the more so under modulation.

Every filter except Resampling carries its own Resonance control. A Filter Peak Gain control on the Peak filter lifts or trims a chosen frequency band. The Morph filter, meanwhile, has a Morph control to dial in its shape.
