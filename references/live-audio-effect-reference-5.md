# Live Audio Effect Reference (part 5)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Three separate delay lines make up the Filter Delay, and ahead of each one sits a paired low-pass and high-pass filter. Because of this, you can restrict the delayed portion to specific bands of the incoming audio, governed by how the filters are set. Whatever feeds back out of each of the trio of delays travels back through those same filters as well.

You may toggle any of the three delays on or off on its own. Within the Filter Delay device, delay 1 handles the left channel of the incoming audio, delay 2 covers both the left and right channels, and delay 3 takes the right channel. Should you wish, the Pan controls on the right side can reroute each delay channel’s output; without that override, a delay simply emerges on whichever channel supplied it.

Sitting to the left of every X-Y controller, each delay channel’s filter carries its own On switch. Both the low-pass and high-pass filters for a given delay move together when you operate the X-Y controllers. Dragging vertically reshapes the filter bandwidth, whereas dragging horizontally tunes where the filter band sits in frequency.

Switching on the Sync switch ties the delay timing to the project tempo and unlocks the Delay Time beat division chooser. Each numbered switch corresponds to a delay measured in 16th notes. Picking ”4”, for instance, holds the audio back by four 16th notes — the equivalent of a single beat, or a quarter note. While Sync Mode is engaged, nudging the Delay Time field percentage value lengthens or trims the delays by partial amounts, which yields the ”swing” feel familiar from drum machines.

Turn the Sync switch off and the delay timing returns to milliseconds. Then you can adjust the figure by dragging upward or downward inside the Delay Time field, or by clicking there and entering a number directly.

How much of the processed output is routed back into the delay line’s input is governed by the Feedback parameter. Pushing it very high risks self-perpetuating feedback and a loud, screaming tone — mind your ears and monitors if you plan to explore the most extreme feedback settings!

A dedicated volume control accompanies each delay channel, with up to +6 dB of boost available to make up for heavy filtering happening at the input.

Use the Dry control to set the level of the untouched signal. Bring it all the way down whenever the Delay sits on a return track.

### 28.20 Gate

The Gate Effect.

Only audio that climbs past a threshold you define is permitted through the Gate effect. It can scrub away quiet background noise lurking between sounds (hiss or hum, say), or it can sculpt a sound: raise the threshold high enough and it will lop off reverb or delay tails or cut an instrument’s natural decay short.

In Gate’s display area, the incoming signal’s level appears in light gray while the outgoing signal’s level shows up as a darker gray edged with a white outline. Seeing both at once lets you gauge how much gating is happening from moment to moment, which makes dialing in the right parameters easier.

Sensitivity is controlled by the Threshold knob. Its value appears in the display as a horizontal blue line that you can also drag directly.

The gap between the level that opens the gate and the level that shuts it is governed by Return (sometimes called “hysteresis”). Raising the hysteresis cuts down on the “chatter” you get when a signal hovering close to the threshold makes the gate flicker open and shut repeatedly. A second horizontal orange line in the display marks the Return value.

Turn on the Flip button and the gate’s logic inverts; now only signal sitting below the threshold is allowed through.

Because a gate cannot respond to a signal before that signal arrives, and because it still has to impose an attack/release envelope, its action is inevitably slightly delayed. A digital gate gets around this by holding the incoming signal back by a tiny amount. Gate gives you a choice of three Lookahead settings: zero ms, one ms and ten ms. Each can sound quite distinct from the others.

How quickly the gate moves from closed to open as a signal rises past the threshold is set by the Attack time. Keep attack times extremely brief and you may hear sharp clicks; stretch them out and the onset of the sound is smoothed instead.

Once the signal drops back below the threshold, the Hold time takes over. When that hold interval runs out, the gate shuts over a span determined by the Release parameter.

The degree of attenuation imposed while the gate is shut comes from the Floor knob. At -inf dB, a closed gate silences the input completely. At 0.00 dB, closing the gate leaves the signal untouched. Any value between those extremes thins the input out by some intermediate amount whenever the gate is closed.

Typically the audio being gated and the source that opens the gate are one and the same. With _sidechaining_, though, you can gate one signal according to the level of a different one. Reveal the Sidechain parameters by clicking the button in the Gate window’s title bar to unfold it.

Gate’s Sidechain Parameters.

Switch this section on with the Sidechain button and you can pick a different track from the choosers underneath. The chosen track’s signal then becomes what opens and closes the gate, in place of the audio that is actually passing through it.

Level of the incoming external sidechain is set by the Gain knob, and the Dry/Wet knob lets you blend the sidechain together with the original signal to form the gate’s trigger. Set Dry/Wet to 100% and the sidechain source alone drives the gate. At 0%, the sidechain has essentially no role. Keep in mind that turning the gain up does _not_ make the source signal any louder in the mix. That sidechain audio merely triggers the gate; you never actually hear it.

One use for sidechain gating is stamping the rhythm of one source onto a different one. A sustained pad, for example, can be made to pulse in time with a drum loop: place a Gate on the pad’s track and pick the drum loop’s track as its sidechain source.

The sidechain EQ controls live on the right-hand side of the external section. Switch this part on and only a chosen band of frequencies — rather than the whole signal — will trigger the gate. Those frequencies can come from the signal being gated, or, when the EQ is paired with an external sidechain, from another track’s audio.

Sitting between the external and EQ sections, the headphones button lets you monitor the sidechain input by itself while muting the gate’s actual output. Because that sidechain audio never reaches the output and exists only to trigger the gate, this temporary monitoring makes it far simpler to tune the sidechain parameters and to hear exactly what is driving the gate. While it is engaged, the display area renders the sidechain input level in green.

### 28.21 Glue Compressor

The Glue Compressor Effect.

Built in partnership with Cytomic, the Glue Compressor is an analog-modeled processor modeled on the well-known bus compressor found in a celebrated 80’s mixing desk. Just like Live’s own [Compressor](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#compressor), it can handle straightforward dynamics duties on a single track, yet its real purpose is sitting on the Main track or a Group Track, where it binds several sources into one unified-sounding mix.

Where compression kicks in is determined by the Threshold knob. Any signal climbing above that point is reduced by an amount the Ratio parameter dictates, that ratio describing the relationship between input and output. The Glue Compressor, unlike the Compressor, gives you no adjustable knee; rather, its knee tightens automatically as you raise the ratio.

How quickly full compression is reached after a signal crosses the threshold is governed by Attack, whose Attack knob is calibrated in milliseconds. Release decides how long the compressor needs to relax back to normal once the signal drops under the threshold, and its Release knob is marked in seconds. Choosing A (Auto) for Release lets the release time track the incoming material on its own. In practice the Glue Compressor’s Auto Release juggles two timings — a slow one acting as the baseline compression and a quick one chasing transients in the audio. Auto Release can lag behind abrupt level jumps, yet it’s generally a gentle, dependable way to handle a broad mix of source material.

The proportion of compressed versus untouched signal is set by Dry/Wet. At 100% you hear only the compressed result, and at 0% the device essentially does nothing. The Range slider gives you another handle on compression amount, capping how much can take place. Settings of roughly -60 to -70 dB mimic the original hardware, whereas the -40 to -15 dB region can serve as a substitute for the Dry/Wet control. At 0 dB there is no compression at all.

Makeup feeds gain back into the signal so you can offset the level lost to compression. Setting a Makeup value that lines up roughly with where the display needle sits should land you near the level you had prior to compressing.

A fixed waveshaper is switched in by the Soft clip control, handy for reining in extremely loud transients. Once it is on, the Glue Compressor tops out at -.5 dB of output. Bear in mind that when Oversampling is on, exceptionally loud peaks can still pass 0 dB. This soft clipper is not a clean limiter — it deliberately distorts the signal while engaged. Unless you specifically want that flavor of “colored” distortion, it’s best left switched off.

Gain reduction in dB is shown on the Glue Compressor’s needle display. Should the device’s output cross 0 dB, the Clip LED lights red. With Soft clipping active, that same LED instead glows yellow to signal that peaks are getting clipped.

### 28.21.1 Sidechain Parameters

The Glue Compressor With Sidechain Section.

Ordinarily the audio being compressed and the source that triggers the compressor are identical. Through _sidechaining_, however, you can drive compression of one signal from the level of a separate signal or even a particular frequency band. To reach the Sidechain parameters, click the button in the Glue Compressor window’s title bar to expand it.

Two sections make up the sidechain parameters. The external controls occupy the left side. Switch this part on with the Sidechain button and the choosers underneath let you tap any of Live’s internal routing points. Whatever you pick then becomes the Glue Compressor’s trigger, in place of the audio actually being compressed.

Level of the external sidechain input is handled by the Gain knob, while the Dry/Wet knob lets you mix the sidechain with the original signal to form the Glue Compressor’s trigger. Set Dry/Wet to 100% and the sidechain source drives the Glue Compressor entirely. At 0%, the sidechain plays essentially no part. Remember that raising the gain does _not_ lift the source signal’s volume in the mix. The sidechain audio serves purely as a trigger for the Glue Compressor and is never heard on its own.

To the right of the external section you’ll find the sidechain EQ controls. Switch this on and a chosen band of frequencies — instead of the whole signal — triggers the Glue Compressor. Those frequencies may come from the compressed signal itself or, when the EQ works alongside an external sidechain, from another track’s audio.

Positioned between the external and EQ sections, the headphones button lets you hear the sidechain input alone while muting the Glue Compressor’s output. Because that sidechain feed never reaches the output and only acts as the Glue Compressor’s trigger, this temporary monitoring makes it much simpler to set the sidechain parameters and to hear precisely what is driving the Glue Compressor.

#### 28.21.1.1 Context Menu Options for Glue Compressor

You switch Oversampling on or off from the context menu on the device’s title bar. Turning it on makes the Glue Compressor run its internal processing at twice the present sampling rate, which can cut down on aliasing and harsh-sounding transients. Expect a modest rise in CPU load while Oversampling is active. Note as well that with Oversampling on, the level can climb past 0 dB even when Soft clip is engaged.

### 28.22 Grain Delay

The Grain Delay Effect.

What the Grain Delay effect does is chop the incoming audio into minuscule fragments (the so-called ”grains”), each of which gets its own delay and can also be retuned away from the pitch of the original source. By randomizing both pitch and delay time you can build dense clouds of sound and rhythm that appear almost unrelated to where they came from. That makes the device handy for inventing fresh sounds and textures, and equally for scaring off unwanted visitors or alarming small pets (only joking!).

Any parameter can be tied to the horizontal or vertical axis of the X-Y controller. Picking a parameter from the row beneath the controller maps it to the X-axis; using the row along the left side maps it to the Y-axis.

Engaging the Sync switch locks the delay timing to the project tempo and makes the Delay Time beat division chooser usable. The numbered switches stand for delays counted in 16th notes. Choose ”4”, say, and the audio is held back four 16th notes — one beat, or a quarter note, of delay. While Sync Mode runs, adjusting the Delay Time field percentage value stretches or compresses the delays by partial steps, giving you the ”swing” timing characteristic of drum machines.

When the Sync switch is off, delay timing goes back to milliseconds. To change it then, drag upward or downward within the Delay Time field, or click into the field and type a value.

The Delay Time can likewise be mapped to the horizontal axis of the X-Y controller.

Randomized shifts in delay timing come from the Spray control. Small amounts blur the audio across time, lending a sense of ”noisiness” to it. Crank Spray up and the source signal’s structure dissolves entirely, with mounting degrees of rhythmic disorder. That’s the setting recommended for anarchists.

Each grain’s dimensions and length follow from the Frequency parameter. How Pitch and Spray sound leans heavily on this setting.

Using the Pitch parameter you can transpose each grain’s pitch; it behaves rather like a rough pitch shifter.

Random fluctuations in every grain’s pitch are introduced by the Random Pitch control. Modest amounts give a kind of mutated chorus, whereas large amounts can render the original pitch totally unrecognizable. Because it interacts with the main Pitch control, you can dial in varying measures of steadiness and wobble in a sound’s pitch.

How much of the output is fed back into the delay line’s input is determined by the Feedback parameter. Crank it too high and the feedback can run away into a loud, ringing tone — keep an eye on your ears and speakers should you decide to push the most extreme feedback settings!

Grain Delay also includes a dry/wet control, which you can map to the vertical axis of the X-Y controller.

### 28.23 Hybrid Reverb

The Hybrid Reverb Effect.

Within a single device, Hybrid Reverb brings together two distinct ways of producing reverberation, mixing convolution reverb alongside several digital reverb algorithms. With its assorted routing choices and controls, you can craft one-of-a-kind reverb tones, conjure drone-like soundscapes, or reshape any source material beyond recognition.

Beyond the bundled impulse responses it ships with, Hybrid Reverb lets you load any audio file to serve as an impulse response (an IR for short), which widens your sound-design possibilities considerably. A set of dedicated controls is on hand to mold whichever impulse response you’ve picked.

Several reverb modes live inside the algorithmic engine, and each supplies its own collection of parameters and tonal character, spanning everything from clean and creamy through to metallic and gong-like.

You can run the convolution and algorithmic engines on their own, or chain them in series or in parallel, with the balance of their volumes freely adjustable. There’s also an EQ section to further tailor the reverb’s tone, and it can be applied to either engine selectively. One more control adds signal degradation, recreating how vintage digital reverb units behaved.

### 28.23.1 Signal Flow

Picture the audio moving through Hybrid Reverb from the device’s left edge toward its right, entering the input section first and then reaching the reverb engines. How those two engines relate to one another is shaped by the routing section; from there the signal travels through the EQ section before it arrives at the output.

On the interface, the convolution reverb engine’s controls are colored yellow, whereas the algorithmic engine’s controls show up in blue.

### 28.23.2 Input Section

The Send knob lets you dial in how much gain is applied to the signal driving the reverb. Keep in mind the dry signal stays untouched and continues to flow through the device.

How long the device waits before the first early reflection appears is set by Predelay, which pushes the reverberation back in time relative to the input. Part of how large a real space seems comes from this gap; for “natural” results, figures from 1ms to 25ms are typical. The Predelay Sync buttons let you pick either a time-based predelay or one synced to the beat.

Feedback determines how much of the predelay’s output is returned to its own input. Note that the time-based and beat-based predelay modes each carry their own separate feedback setting.

Hybrid Reverb’s main window holds two tabs, Reverb and EQ. Every control tied to both the convolution and algorithmic engines lives under the Reverb tab. Beginning with the Routing chooser at the center, four choices are available:

- Serial feeds the convolution engine’s output into the algorithmic engine. The convolution reverb stays on at all times here, while Blend sets how much of it is passed along to the algorithmic reverb. At 100/0 you get convolution reverb alone, and at 0/100 you get purely algorithmic reverb that has been driven by the convolution reverb’s output.
- Parallel runs both the convolution and algorithmic engines but keeps them apart from each other. Here the Blend knob sets the level balance between the two engines, with 100/0 yielding only convolution reverb and 0/100 yielding only algorithmic reverb.
- Algorithm engages the algorithmic reverb engine by itself.
- Convolution engages the convolution reverb engine by itself.

The interface of Hybrid Reverb adapts on the fly, so any engine that isn’t currently active will have its controls dimmed out.

When Routing is set to Serial or Parallel, the Blend knob crossfades between the convolution and algorithm section outputs. Bear in mind that picking either Algorithm or Convolution in the Routing chooser leaves the Blend knob with nothing to do.

### 28.23.3 Convolution Reverb Engine

Hybrid Reverb’s Convolution Reverb Section.

To produce its effect, a convolution reverb relies on recordings of real spaces, known as impulse responses. That lets you situate your sounds inside nearly any environment you happen to have a recording of. For more conventional reverb, that might mean some of the world’s most renowned halls and studios. Take a more experimental route and you could use recordings of just about anything — snare drums, garbage cans, even instrumental or vocal takes!

You select impulse responses from the Convolution IR menu. The top drop-down picks the impulse response category, and the bottom drop-down selects a particular impulse response inside that category. Backward and forward arrow buttons make browsing the impulse responses easy. Once you hit the end of a category, these arrows roll over to the next one automatically, letting you sweep through every impulse response with the arrows by themselves. The selected impulse response’s waveform then appears in the main display, which redraws according to the Attack, Decay, and Size settings (covered below).

Several impulse response categories are provided. The first few cover Early Reflections, Real Places, and Chambers and Large Rooms. After those come Made for Drums, then Halls, Plates and Springs. Rounding out the set are Bigger Spaces, Textures, and finally User.

To load your own impulse responses into the User category, drag and drop the IR audio file onto Hybrid Reverb’s convolution waveform display. Should you drop in a file from a folder holding other audio files, every one of them gets added as an impulse response. Note: take Hybrid Reverb off a track and put it back, and any User samples you’d added before will be gone from the User category. You can, though, drag and drop those samples onto the waveform display once more to rebuild the list.

The impulse response’s amplitude envelope is governed by the Attack, Decay, and Size parameters. Attack sets the envelope’s attack time, Decay sets its decay time, and the Size parameter changes the impulse response’s relative size.

### 28.23.4 Algorithmic Reverb Engine

Hybrid Reverb’s Algorithmic Reverb Section.

Unlike the convolution engine, the algorithmic engine rests entirely on digital delay lines and draws on no samples whatsoever.

The controls for the algorithmic reverb engine sit to the right of the Blend knob. Which parameters appear there depends on the selection you make in the Algorithm chooser.

You have five algorithms to choose from: Dark Hall, Quartz, Shimmer, Tides and Prism. Across every one of them, the Decay, Size, Delay and Freeze parameters are present.

Decay sets roughly how long the algorithm’s reverb tail takes to fall to 1/1000th (-60 dB) of where it started. Size dictates how big the virtual room is. Delay tacks on an extra predelay, in milliseconds, for the algorithm section.

Two buttons, Freeze and Freeze In, make up the Freeze controls. Freeze cuts off all input to the reverb engine and stretches the algorithm’s decay to infinite, so the reverb output carries on without end. Switching on Freeze In folds the input signal into the frozen reverberation, which builds up an accumulating wash of reverb.

Below, each algorithm and the parameters unique to it are explained in more depth.

#### 28.23.4.1 Dark Hall

A polished, classic-sounding algorithm, Dark Hall works well for the majority of medium- to long-tailed halls.

On top of the shared parameters noted earlier, Dark Hall adds these:

- Damping governs how much high-frequency filtering takes place inside the reverb algorithms. The higher you set it, the darker the reverberation becomes.
- Mod governs how much motion there is in the algorithm’s reverb tail. Dialing it down yields less movement, while turning it up adds more movement and a chorus-like quality, though it also weakens any resonances.
- Shape shifts the artificial space’s tonal character along a range from small and resonant to large and diffuse.
- Bass X sets the crossover point for the low end of the reverb tail, which is then scaled by the Bass Mult control.
- Bass Mult scales how long the low end of the reverb tail takes to decay.

Within Dark Hall, pairing long decay times with extremely tiny Size values produces metallic, gong-like resonances.

#### 28.23.4.2 Quartz

Quartz is a hall-style reverb whose tail carries some perceptible echoes. It reproduces the input very cleanly in its early reflections, making it a good fit for vocals, drums and any signal with sharp transients, as well as for crafting echoes.

On top of the shared parameters noted earlier, Quartz adds these:
