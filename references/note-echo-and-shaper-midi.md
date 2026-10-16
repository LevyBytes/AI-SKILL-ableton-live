# Note Echo And Shaper MIDI

Open when you need guidance on Note Echo And Shaper MIDI in Ableton Live.

Context: [Max for Live MIDI Effects](max-for-live-devices.md#323-max-for-live-midi-effects).

<a id="source-3235-note-echo"></a>
### 32.3.5 Note Echo

The Note Echo Effect.

Note Echo is a delay-style echo effect that spawns extra MIDI notes at set time intervals while the velocity tapers off.

Switch on the Sync switch so the Delay Time beat division chooser becomes available. Each numbered switch stands for a delay measured in 16th notes. Picking "4," for instance, holds the signal back by four 16th notes, the equivalent of a single beat (a quarter note) of delay.

Adjusting the percentage in the Delay Time field nudges delay times shorter or longer by fractional amounts, which yields the "swing" feel of timing heard in drum machines.

When the Sync switch is off, delay time switches back to milliseconds. Set the delay time by dragging the Delay Time slider upward or downward, or by clicking the field and entering a number.

The Input switches let you flip between Thru/Mute playback modes. Under Thru, you hear both the MIDI note and the echo. Under Mute, the MIDI note is silenced and only the echo sounds.

Pitch determines how much transposition each echo repeat applies to the note.

Delay determines how much velocity reaches the echo. The Fback parameter governs the share of the channel's output signal routed back into the input of the delay line.

Turning the MPE toggle on lets arriving MPE data be echoed together with MIDI notes and velocity data. If it stays off, the MPE data gets filtered out.

Once the MPE toggle is on, the Press, Slide, and Note PB sliders go live; respectively, each one governs how much feedback applies to the pressure, slide and per-note pitch bend data. Dialing the feedback amount below 100% makes the echoed MPE data fade away gradually with each repeat.

<a id="source-3236-shaper-midi"></a>
### 32.3.6 Shaper MIDI

The Shaper MIDI Effect.

Shaper MIDI is a modulator device that relies on a breakpoint envelope to produce mappable modulation data. In contrast to the [Shaper audio effect](https://www.ableton.com/en/live-manual/12/max-for-live-devices/#shaper), the envelope modulation of Shaper MIDI fires on every MIDI note and responds to velocity.

Inside Live you can map any automatable parameter onto Shaper MIDI, whether device or mixer parameters. Do this by switching on the Map button, then clicking a parameter to set it as a mapping target.

Click the Show/Hide Multimap button at the display's upper right to bring up further mapping buttons. The total number of parameters you can map is eight.

You Can Map up to Eight Parameters.

Remove a parameter assignment by clicking the Unmap button positioned to the right of the Map button.

Shaper MIDI offers two distinct ways to drive mapped parameters: Modulation and Remote Control. Modulation is the default choice, though the Mod toggle lets you switch over to Remote Control.

With Modulation active, you remain free to change parameter values even once they are mapped. The Modulation Polarity toggle flips between the Bipolar and Unipolar modes. Under Bipolar mode, modulation travels both ways with the base value sitting at the midpoint. Under Unipolar mode, modulation moves only one way starting from the base value. The Modulation Amount slider sets how deep the modulation goes. That establishes the modulation range measured against the base value.

With Remote Control active, Shaper MIDI alone dictates the parameter values and you cannot move them by hand. The Min and Max sliders let you scale how far the modulation reaches.

Make a breakpoint by clicking anywhere within the display. Holding Ctrl (Win) / Cmd (Mac) as you click in the display produces a sustain breakpoint. That sustain breakpoint appears larger so it stands apart from the ordinary breakpoints on screen. Each envelope allows just a single sustain breakpoint. Where a sustain breakpoint exists, the envelope holds at the sustain level the whole time a note stays held.

A sustain breakpoint holds the envelope at a chosen level for the duration that a note stays held.

Drag between breakpoints while holding the Alt (Win) / Option (Mac) key to bend a segment into a curve. Holding Shift and clicking a breakpoint removes it.

Clear the whole envelope from the display by pressing the Clear button down in the lower left corner. Beside the Clear button, on its right, you can pick from six presets to spin up a fresh breakpoint envelope in a hurry.

The Grid slider lets you change how many grid divisions appear in the display. With Snap turned on, every breakpoint you add or move jumps automatically to the closest grid line.

Up at the top right of the device, a smaller display offers an oscilloscope-style look at the envelope's output signal. Each time the envelope fires, the LED in that display flashes.

The Jitter slider injects randomness into the envelope output, whereas the Smooth control rounds off any abrupt changes in the output, jitter-driven ones included.

The Velocity control lets you decide how strongly velocity shapes the modulation depth. Set to 0%, velocity does nothing and the envelope output holds a steady amplitude. Raise it and softer velocities pull the envelope output down for gentler modulation, while harder velocities push the output up for a stronger effect.

The Offset control moves the envelope output's center point. At 0%, the output sits centered. Positive values lift the output, and negative values drop it. That horizontal line across the oscilloscope display marks the center and serves as a useful guide while you set Offset.

You Can Shift the Center Point of the Envelope Output Using Offset.

Switch on the Loop toggle to keep the envelope repeating at whatever speed the Rate control sets for the whole time a MIDI note is held. With Loop on, the sustain breakpoint level gets skipped.

The Rate control governs the envelope rate. The Time Mode toggles let you flip between frequency values in Hertz and tempo-synced beat divisions.

Depth governs how much modulation reaches every mapped parameter. At 0%, nothing is modulated, while at 100% the envelope output arrives at full strength.

Echo and Time let you layer echoes onto the envelope output. The Echo control sets how much of each echo carries into the following one, shaping how long the echoes linger. Raise the value for more drawn-out repeats. The Time control fixes the spacing between echoes.

The Echo and Time controls let you layer echoes onto the output of the envelope.
