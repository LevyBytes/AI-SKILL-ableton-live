# Live Audio Effect Reference (part 8)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Switching on the DC Shift button introduces an amplitude offset ahead of quantization. The character of the quantization distortion shifts noticeably as a result — most audibly when Bits sits at lower values, where the level rises and extra crunch appears!

Use the Dry/Wet control to balance how much processed versus dry signal you hear. When Redux runs in a return track, dial this to 100%.

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

### 28.32 Reverb

The Reverb Effect.

Reverb is an audio effect that recreates how a sound behaves acoustically as it reverberates inside a physical space.

Out in the physical world, reverberation arises when sound waves bounce off the hard surfaces around them, and as absorptive materials in their path subsequently reshape the tone of those waves. Digitally, though, that behavior is modeled through a mix of filters paired with modulated delay lines.

Fine control over every one of these elements is what the Reverb device offers, letting you build distinctive spaces for sound to move through — anything from a cozy recording room to a vast canyon and all points between.

### 28.32.1 Input Filter

Reverb’s Input Filter Section.

First in the chain, the signal meets low and high cut filters whose X-Y controller sets the band’s center frequency on the X-axis and its bandwidth on the Y-axis. You can also operate the filters with the sliders sitting beneath the X-Y controller. When either filter isn’t required, switching it off conserves CPU power.

### 28.32.2 Early Reflections

Reverb’s Early Reflections Section.

What you hear soonest are these echoes, arriving as the sound rebounds off the room’s walls ahead of the diffused reverberation tail setting in. The way they spread out, and how loud they are, conveys a sense of the room’s character.

Modulation of the early reflections is handled by Spin. Its Amount and Rate sliders govern how much modulation occurs and how fast, respectively. Pushing the Amount higher generally yields a late diffusion response that is more spectrally neutral and less colored. Should the modulation rate climb too high, doppler-style pitch shifting of the source sound creeps in, accompanied by surreal panning artifacts. To save a little CPU, Spin can be switched off via its associated switch.

How prominent the early reflections are, and how much they overlap the diffused sound, is shaped by the Shape control. At lower settings, the reflections fade more gently and the diffused sound arrives earlier, so these two elements overlap more. At higher settings, the reflections fade quicker and the diffused onset comes later. Raising the value can occasionally sharpen the source’s clarity, whereas a lower value tends toward a smoother decay.

### 28.32.3 Diffusion Network

Reverb’s Diffusion Network Section.

It is the Diffusion Network that generates the reverberant tail trailing the early reflections.

Frequency-dependent reverberation decay comes from the high and low shelving filters. The decay at high frequencies mirrors how air, walls, and other materials in the room — occupants, carpet, and the like — absorb sound energy. A thinner decay is supplied by the low shelf. Switching either filter off lowers CPU consumption.

Density and coarseness of the diffusion can be further shaped with the Diffusion and Scale parameters, which, when the room is set to an extremely small size, weigh heavily on the coloration the diffusion introduces.

### 28.32.4 Chorus

Reverb’s Chorus Section.

A touch of modulation and movement is added to the diffusion by the Chorus section. You can set its modulation Amount and Rate, or switch it off entirely.

### 28.32.5 Global Settings

Reverb’s Global Settings.

How long the device waits, in milliseconds, before the first early reflection begins is governed by Predelay, which pushes the reverberation back in time relative to the input. Part of how large a real room seems comes down to this delay. For natural-sounding material, expect figures somewhere between 1 ms and 25 ms.

When you adjust the Size parameter, the Smooth chooser dictates how that change behaves. Choose None and the Diffusion Network’s delay times jump instantly, which can introduce artifacts as the Size value moves. Choose Slow or Fast and the new delay times settle in across a set interval, giving a smoother transition between values.

How big the room is comes down to the Size parameter. Pushed to its upper limit, a very large size gives the reverb a shifting, diffused delay quality. Pulled to the opposite extreme, a very small value makes it sound highly colored and metallic.

Use the Decay control to set how long the reverb tail takes to fall to 1/1000th (-60 dB) of where it started.

What the Freeze control does is hold the diffuse response of the incoming sound in place; with it on, the reverberation rings on nearly forever. While Freeze is engaged, Flat bypasses both the high and low shelf filters. Leave Flat off and the frozen reverberation will bleed energy from the attenuated bands according to how the high and low shelving filters are set. Cut alters Freeze so the input signal no longer feeds the frozen reverberation; with it off, the input does add to the diffused amplitude.

The width of the output’s stereo image is set by the Stereo control. Turned all the way up to 120 degrees, each ear gets its own reverberant channel fully independent of the other — something real rooms exhibit in their diffusion too. Turned all the way down, the output is summed to mono.

A balance between reverb quality and CPU cost is struck with the Density chooser. Sparse keeps CPU usage to a minimum, whereas High produces the most lavish reverberation.

### 28.32.6 Output

Reverb’s Output Section.

Right at the reverb’s output stage, the Reflect and Diffuse controls let you scale the level of reflections and diffusion, and you can set the effect’s overall Dry/Wet mix here as well.

### 28.33 Roar

The Roar Effect.

Roar is a device for saturation and coloration, offering as many as three processing stages alongside an assortment of adaptable routing layouts. By pairing its array of non-linear shaper curves with its filters, you can conjure a broad span of saturation flavors — pinpoint warmth, sweeping harmonic movement, or glitchy bursts of noise. Layered on top, Roar’s feedback controls and onboard compressor open up further distinctive territory, letting the device generate sounds you won’t find in any other instrument or effect Live currently ships.

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

### 28.33.3 Modulation Section

Clicking the toggle in the Modulation panel reveals Roar’s modulation parameters and opens up the Mod Sources and Matrix tabs.

Roar’s Modulation Toggle.Roar’s Modulation Section.

Four modulation sources sit in the Mod Sources tab: _LFO 1_, _LFO 2_, _Env_ (Envelope), and _Noise_. Every one of these sources arrives with its own signal-visualizing display plus its own dedicated set of parameters.

Each LFO offers a pick of five waveforms: sine, triangle, square, up, or down.

Through the Mode chooser you can put the LFO rate into Free, Synced, Triplet, Dotted, or Sixteenth mode. The Rate slider then sets that rate, in Hertz under Free mode or as tempo-synced beat divisions in the rest. You can dial the Morph control by hand or modulate it to further shape the LFO. Adding smoothing to the LFO signal is handled by the Smooth control, which helps tame abrupt jumps during modulation.

Drawing on Roar’s input, the envelope follower in the Env tab produces a modulation signal. The tab’s parameters let you tune how that follower reacts to the incoming signal.

How fast the envelope tracks the input is shaped by the Attack and Release controls. The Envelope Hold toggle also governs the move from attack into release: switch it on and the envelope runs its full attack phase before the release phase begins.

Sensitivity and strength of the envelope are set by the Threshold and Gain controls, while Frequency and Width pin down a particular frequency band for the signal feeding the envelope follower.

Switch on the Envelope Input Listen toggle to monitor only the input signal.

Within Roar’s Modulation Matrix, the envelope follower really shines as a source. Point it at a snare in a drum loop, for instance, and let it drive Roar’s Dry/Wet balance or Shaper Amount on every snare hit.

Four noise flavors live in the Noise modulation source: Simplex, Wander, S & H, and Brown. Like Roar’s LFO curves, noise curves can run in Hertz or tempo-synced, and they accept smoothing too.

Both Simplex and Wander put out smoothed random signals, each relying on a different interpolation algorithm to give the signal its own dynamics. Simplex draws on interrate modulation, so its value intervals come out more erratic than Wander’s. Such noise types are great for sneaking small, random, organic-feeling motion into Roar’s output, especially at low rates.

S & H (Sample and Hold) holds a random value steady, then jumps to a fresh random value on an interval set by the Noise Rate. It’s handy for building stepped random modulation in Roar’s output.

Brown delivers low-pass filtered white noise, useful for laying down a steady noise floor or sprinkling crackle and hiss across Roar’s output.

Through the Matrix tab you wire modulation sources to modulation targets inside the device. With the Matrix tab open, clicking any parameter marks it as a target. The sources run along the horizontal axis and the targets down the vertical one. Drag a cell up or down to set the modulation between two parameters.

Drag the Global Modulation Amount slider up or down to raise or lower how much modulation is applied across the board. Hitting the X button wipes out every modulation the Modulation Matrix has applied.

You can also expand the Modulation Matrix from the toggle in the device header. Expanded, the device shows all its gain stages together, along with the full set of sources and targets in the Modulation Matrix.

Roar’s Expanded Matrix.

Beyond the visualization displays, LEDs in the Modulation column also flag modulation signals. Every LED takes on a color tied to a particular modulation source. That lets you tell at a glance whether a source is active, and get a feel for its setup, without opening the Modulation Matrix.

### 28.33.4 Feedback Section

Roar’s Feedback Section.

Among Roar’s standout traits is the Feedback section. Routing Roar’s signal back through itself layers in fresh ringing, otherworldly tones and textures.

Five feedback modes are available from the Feedback Mode drop-down: Time, Synced, Triplet, Dotted, and Note. Pick Synced or Time to run Roar’s Feedback as a delay. Choose Note to pin the feedback’s ring to a chosen pitch.

How much signal loops back into Roar’s input is set by the Feedback Amount knob. Since a compressor sits inside Roar’s feedback loop, loud material momentarily pulls the generated feedback down as the compressor applies gain reduction.

Switch the Feedback Invert toggle on and Roar’s feedback signal has its phase flipped. When that inverted signal meets the original, the resulting phase cancelation opens up yet another avenue to explore in Roar’s signal path.

With the Feedback Gate toggle engaged, Roar’s feedback fades away on its own once the device stops receiving an input. Leave it off and the feedback carries on without end.

The center frequency of the band-pass filter that treats Roar’s feedback is set with the Feedback Filter Frequency slider, while the Feedback Filter Width slider sets how wide that filter’s band is.

### 28.33.5 Global Section

Roar’s Global Section.

How much compression lands on the output — and therefore on whatever loops back into Roar — is set by the Compression Amount knob.
