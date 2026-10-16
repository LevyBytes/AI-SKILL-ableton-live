# Gate And Glue Compressor

Open when you need guidance on Gate And Glue Compressor in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2820-gate"></a>
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

<a id="source-2821-glue-compressor"></a>
### 28.21 Glue Compressor

The Glue Compressor Effect.

Built in partnership with Cytomic, the Glue Compressor is an analog-modeled processor modeled on the well-known bus compressor found in a celebrated 80’s mixing desk. Just like Live’s own [Compressor](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#compressor), it can handle straightforward dynamics duties on a single track, yet its real purpose is sitting on the Main track or a Group Track, where it binds several sources into one unified-sounding mix.

Where compression kicks in is determined by the Threshold knob. Any signal climbing above that point is reduced by an amount the Ratio parameter dictates, that ratio describing the relationship between input and output. The Glue Compressor, unlike the Compressor, gives you no adjustable knee; rather, its knee tightens automatically as you raise the ratio.

How quickly full compression is reached after a signal crosses the threshold is governed by Attack, whose Attack knob is calibrated in milliseconds. Release decides how long the compressor needs to relax back to normal once the signal drops under the threshold, and its Release knob is marked in seconds. Choosing A (Auto) for Release lets the release time track the incoming material on its own. In practice the Glue Compressor’s Auto Release juggles two timings — a slow one acting as the baseline compression and a quick one chasing transients in the audio. Auto Release can lag behind abrupt level jumps, yet it’s generally a gentle, dependable way to handle a broad mix of source material.

The proportion of compressed versus untouched signal is set by Dry/Wet. At 100% you hear only the compressed result, and at 0% the device essentially does nothing. The Range slider gives you another handle on compression amount, capping how much can take place. Settings of roughly -60 to -70 dB mimic the original hardware, whereas the -40 to -15 dB region can serve as a substitute for the Dry/Wet control. At 0 dB there is no compression at all.

Makeup feeds gain back into the signal so you can offset the level lost to compression. Setting a Makeup value that lines up roughly with where the display needle sits should land you near the level you had prior to compressing.

A fixed waveshaper is switched in by the Soft clip control, handy for reining in extremely loud transients. Once it is on, the Glue Compressor tops out at -.5 dB of output. Bear in mind that when Oversampling is on, exceptionally loud peaks can still pass 0 dB. This soft clipper is not a clean limiter — it deliberately distorts the signal while engaged. Unless you specifically want that flavor of “colored” distortion, it’s best left switched off.

Gain reduction in dB is shown on the Glue Compressor’s needle display. Should the device’s output cross 0 dB, the Clip LED lights red. With Soft clipping active, that same LED instead glows yellow to signal that peaks are getting clipped.
