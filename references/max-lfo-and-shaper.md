# Max LFO And Shaper

Open when you need guidance on Max LFO And Shaper in Ableton Live.

Context: [Max for Live Audio Effects](max-for-live-devices.md#322-max-for-live-audio-effects).

<a id="source-3223-lfo"></a>
### 32.2.3 LFO

The LFO Effect.

LFO is a modulator device that steers mapped parameters by way of low-frequency oscillation.

Within Live, any automatable parameter — device or mixer controls included — can be assigned to LFO. Do this by turning on the Map button and clicking the parameter you want to use as the mapping target.

Additional mapping buttons appear when you press the Show/Hide Multimap button at the display's top right; in all, up to eight parameters can be mapped.

You Can Map up to Eight Parameters.

To drop an assignment, click the Unmap button sitting to the right of the Map button.

LFO offers two ways to govern mapped parameters: Modulation and Remote Control. Modulation is the default, and the Mod toggle switches you over to Remote Control.

While Modulation is on, you can still tweak parameter values manually after mapping them. The Modulation Polarity toggle alternates between Bipolar and Unipolar modes. Bipolar mode modulates in both directions around a centered base value, whereas Unipolar mode pushes in just one direction away from the base value. Modulation depth is fixed by the Modulation Amount slider, which sets the range measured against the base value.

Once Remote Control is on, the mapped values are set entirely by LFO and can't be edited by hand. The Min and Max sliders scale the modulation range.

The Waveform drop-down menu lets you pick from nine shapes: Sine, Up, Down, Triangle, Square, Random, Bin, Stray, and Glider.

Bending or skewing the LFO waveform is done with the Shape control, and the Steps slider can divide the waveform into as many as 24 steps. Because of how their values arise, some waveforms can't be shaped or stepped — so the Shape control grays out for Random, Bin, Stray, or Glider, and the Steps control grays out for Random, Bin, or Square.

Randomness is sprinkled onto the LFO output by the Jitter slider, while the Smooth control rounds off abrupt changes in the output, including the ones jitter introduces.

The LFO rate is fixed by the Rate control. The Time Mode toggles flip between frequencies in Hertz and tempo-synced beat divisions, and when Hz is active the ×10 button multiplies the frequency value.

For every mapped parameter, the modulation amount is governed by Depth. At 0% nothing is modulated, and at 100% the LFO output reaches its full strength.

The Offset control repositions the center point of the LFO output. At 0% the output sits centered. Positive values raise the output, negative values lower it. A horizontal line in the display marks the center, serving as a handy visual cue while you adjust Offset.

You Can Shift the Center Point of the LFO Output Using Offset.

Where the LFO sits within its cycle is set by the Phase slider, running from 0% (cycle start) to 100% (cycle end).

To lock the LFO output at its present value, turn on the Hold toggle. Turning Hold off resumes the LFO from the value that was held.

Press the R (Retrigger) button to restart the LFO from the spot set by the Phase control.

<a id="source-3224-shaper"></a>
### 32.2.4 Shaper

The Shaper Effect.

Shaper is a modulator device that builds mappable modulation data out of a breakpoint envelope.

Within Live, any automatable parameter — device or mixer controls among them — may be routed to Shaper. To set this up, switch on the Map button and click the parameter you wish to use as the mapping target.

Pressing the Show/Hide Multimap button at the display's top right surfaces extra mapping buttons, raising the total to eight parameters.

You Can Map up to Eight Parameters.

To clear an assignment, click the Unmap button positioned to the right of the Map button.

Shaper drives mapped parameters in one of two ways: Modulation and Remote Control. The default is Modulation, and the Mod toggle takes you to Remote Control.

With Modulation engaged, parameter values stay editable by hand even once mapped. The Modulation Polarity toggle alternates between Bipolar and Unipolar modes. Bipolar modulation runs in both directions about a centered base value, while Unipolar modulation extends one way from the base value. Modulation depth is set with the Modulation Amount slider, establishing the range relative to the base value.

When Remote Control is engaged, the mapped values come solely from Shaper and admit no manual edits. Use the Min and Max sliders to scale the modulation range.

Click anywhere in the display to drop a breakpoint. Holding the Alt (Win) / Option (Mac) key as you drag between breakpoints yields curved segments, and holding Shift while clicking a breakpoint removes it.

To wipe the whole envelope from the display, hit the Clear button in the lower-left corner. Just to its right, six presets let you spin up a fresh breakpoint envelope in a hurry.

The number of grid divisions in the display is set with the Grid slider. Turn on Snap and any breakpoint you add or move will lock to the nearest grid line.

A smaller display at the device's top right offers an oscilloscope-style look at the envelope's output signal.

Randomness is added to the envelope output by the Jitter slider, while abrupt output changes — jitter-induced ones included — are smoothed out by the Smooth control.

Where the envelope output falls within its cycle is set by the Phase control, spanning 0% (cycle start) to 100% (cycle end). The R (Retrigger) button restarts the envelope output from the spot Phase defines; note that this Retrigger button grays out whenever Time Mode is set to Sync.

The Offset control repositions the center of the envelope output. At 0% the output is centered, positive values lift it, and negative values drop it. A horizontal line in the oscilloscope display marks the center, a useful visual reference as you adjust Offset.

You Can Shift the Center Point of the Envelope Output Using Offset.

Three trigger modes are available in Shaper: Loop, 1-Shot, and Manual. Switching among them is done with the matching toggles.

- Loop — The envelope cycles without pause at whatever rate the Rate control specifies.
- 1-Shot — A single pass of the envelope is fired off using the mappable T button.
- Manual — You scrub the envelope back and forth by hand with the Manual control.

The envelope rate is set by the Rate control. The Time Mode toggles switch between frequencies in Hertz and tempo-synced beat divisions.

Across all mapped parameters, the modulation amount is set by Depth. At 0% none is applied, and at 100% the envelope output hits its full level.
