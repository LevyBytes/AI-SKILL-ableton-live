# Max For Live Devices (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

The Modulation toggle additionally influences the polarity behavior of Expression Control. Choosing Modulate reveals a Modulation Polarity toggle within the Output Range section, where you pick either bipolar or unipolar operation. With Bipolar mode active, the modulation pivots around whichever base parameter value is currently being modulated. With Unipolar mode active, the modulation gets summed onto that base parameter value instead. The Output Range Max slider determines the modulation output produced once the incoming signal hits its peak amplitude. Selecting Remote Control instead turns the Output Range section into a place where you define both a floor and a ceiling for the modulation output, controlled through the Output Range Min and Output Range Max sliders.

Use the Curve Type buttons sitting underneath the Curve Display to pick either a linear or an S-shaped curve. Whichever curve type you pick governs the set of controls offered within the Curve section.

With a linear curve chosen (it carries two breakpoints), the Curve A dial reshapes the whole modulation curve at once. Pick an S-shaped curve (which has three breakpoints) and the Curve A dial then governs the upper part of the curve while the Curve B dial governs the lower part. Enabling the Curve Link button means the upper and lower portions move in opposite directions through the single Curve A dial alone.

The Curve Display gives you a visual look at the modulation curve the device is currently producing. You define the curve's lowest and highest values through the Min/Max sliders. With an S-shaped curve active, the X-Y sliders let you position the middle breakpoint both horizontally and vertically. You can equally reshape the breakpoints and overall curve by dragging the rendered curve right inside the display.

Picking Increment as the modulation source from any MIDI Input Source drop-down menu switches on the Increment Steps slider. That setting governs the number of note triggers required to traverse the device's full modulation range, accepting any value from 1 to 32 steps. Halting transport clears the counter, meaning the very first note after transport resumes emits whatever minimum modulation value you configured.

Picking Random as the modulation source from any MIDI Input Source drop-down menu switches on the Random Amount slider. Use this slider to dial in how much random spread is applied around the target modulation value at every note trigger.

Through the Smoothing Type toggle you decide whether smoothing across modulation values follows a linear or a logarithmic path.

The Smoothing Rise and Fall sliders govern how long, between 0 and 1000 milliseconds, rising and falling modulation values take before they arrive at the latest value.

### 32.3.3 MIDI Monitor

The MIDI Monitor Effect.

MIDI Monitor serves as a utility MIDI device for showing incoming MIDI together with MPE data.

You can inspect MIDI data through either the Note display or the Flow diagram.

Within the Note display, arriving MIDI notes appear on a keyboard layout together with their root note and any associated chords (when chords are played). The velocity of each note appears as well.

The Flow diagram builds an ongoing stream listing arriving MIDI notes and data, including messages like pitch bend and aftertouch, as the notes are performed. Use the Freeze toggle to halt or resume the display, and the Clear button wipes everything from it.

The Flow Diagram.

You inspect MPE data inside the MPE display. Arriving note, velocity, slide, pressure and per-note pitch data flow through as an ongoing stream while notes are performed.

The MPE Display.

### 32.3.4 MPE Control

The MPE Control Effect.

MPE Control is a Max for Live MIDI effect for reshaping and transforming arriving MPE (MIDI Polyphonic Expression) signals, providing separate, tailored adjustments for every MPE data source. You normally pair it with a second device so you can refine how the MPE data influences mapped parameters. On top of that, MPE Control can turn MPE signals into global MIDI, which lets you drive non-MPE enabled instruments from an MPE controller.

Before digging into how the MPE Control effect reshapes arriving MPE data, it helps to consider what separates MPE from ordinary MIDI messages. With MPE, MIDI Control Change (or MIDI CC) messages travel on a per-note basis, so each note can be articulated on its own. Lacking MPE, the same messages travel globally, so every note responds to whatever MIDI CC is in play. To read more about MPE, see the [Editing MPE](https://www.ableton.com/en/live-manual/12/editing-mpe/#editing-mpe) chapter.

MPE already opens up far more musical expression than plain MIDI data, yet MPE Control lets you sculpt those MPE signals even further through curves, which makes still more expressive performances possible. Imagine you have the Expression Control device in use and routed its Slide MIDI input onto the Filter Freq knob inside Operator. Every bit of arriving MPE slide data then drives the filter frequency. From there MPE Control can refine that signal so that only the very highest slide values push toward a high cutoff frequency.

Inside MPE Control, arriving MPE signals get reshaped through two kinds of curves, both of which support smoothing for even rise and fall behavior. Three signal sources exist: Press (pressure), Slide, and also NotePB (per-note pitch bend), with each one adjustable on its own.

Whichever MPE source you select has its curve drawn in the front of the display, putting that curve and its associated controls within reach for editing. Out of the box every MPE source is switched on, yet you can turn each one off on its own by clicking the toggle beside its name.

Every MPE source offers two curve-setting choices at the lower left of the display: linear or S-shaped. A linear curve carries two breakpoints, whereas an S-shaped curve carries three.

Pick the linear setting and you can shape the curve through two methods. Either turn the Curve control knob or drag the curve straight inside the display. Beyond reshaping the curve, you can also set its floor and ceiling through the Min and Max sliders, or by hauling the breakpoints sitting at each end of the curve.

A single curve comes from the linear setting, producing a smooth ramp for whichever modulation source you chose, either "compressing" the data so staying in the lower value range is easier, or "expanding" it so reaching higher values takes less input.

Pick the S-shaped curve and a third breakpoint appears at the center of the curve's line, splitting the curve into two separate segments. Because that breakpoint moves freely, you have full say over where the two segments cross over, opening the door to far more extreme curves. By default the two segments stay linked. Flip the Curve Link button to detach the segments from one another, after which each can be compressed or expanded on its own through the two separate Curve dials.

Keep in mind that the breakpoint dividing the two segments can be moved either by clicking and dragging it directly, or through the X-Y controls along the bottom of the display. Those X-Y controls come alive only while the S-shaped curve is in use.

Click the triangular button at the lower right of the visualization to reveal the advanced settings panel.

MPE Control's Expanded View.

Each of the three modulation sources carries a Smooth toggle that turns on smoothing for whichever source is currently selected. You can dial in separate Rise and Fall values per curve through the matching controls, and further controls appear depending on which source you happen to be editing.

#### 32.3.4.1 Press

The Press source lets you reshape MPE pressure data, which, much like polyphonic aftertouch, travels on a per-note basis whenever pressure lands on a controller's key or pad once it has already been struck.

Press Advanced Settings.

Press carries a Default toggle, letting you assign a default MPE value for use with MIDI notes that arrive without MPE data. You may also route the MPE pressure data toward the Slide rather than the Press source through the Swap to Slide toggle. That comes in handy when, say, you'd rather adjust modulation along the vertical axis yet your controller offers only polyphonic aftertouch.

The Press to AT setting turns the MPE pressure data into monophonic aftertouch, so an MPE controller can modulate non-MPE instruments.

#### 32.3.4.2 Slide

The Slide source reshapes MPE slide data (sent as MIDI CC 74), which maps to where the finger sits vertically on the controller key or pad.

Slide Advanced Settings.

Slide likewise carries a Default toggle for non-MPE data, plus a Centered switch that helps when performing on pad-based MPE controllers. Turn Centered on and MPE slide data gets reshaped so that striking the pad's center yields a modulation value of zero, with that value climbing steadily as the finger travels away from center along the vertical axis.

Out of the box, Slide sits in Abs mode, treating MPE slide values as absolute. Flipping the mode to Rel (relative) makes the slide values begin at the middle of the range no matter where the finger rests on the key or pad. They can then change only by sweeping the finger further up and down while a note is held. Under Ons (onset) mode, MPE slide values refresh only at a Note On. Be aware that onset mode switches smoothing off automatically.

The Slide to Mod option turns MPE slide messages into Mod Wheel (CC1) messages, which lets an MPE controller modulate non-MPE enabled instruments.

#### 32.3.4.3 NotePB

The NotePB source reshapes the MPE per-note pitch bend data, which comes from horizontal motion across the controller's keys or pads. By its nature, pitch bend influences only the pitch or pitches being sounded.

NotePB Advanced Settings.

Within the NotePB advanced settings you can set the Pitch Range, handy when the hardware controller's pitch bend range and the instrument's do not line up. As an example, a 2x setting lets you map an MPE controller carrying a +/- 48 semitone pitch bend range onto an instrument whose range is +/- 24 semitones. Should the Note Pitch Bend MIDI CC be routed to something besides pitch, higher values let you span a wider modulation range from a smaller gesture.

Turn the NotePB to PB switch on and MPE per-note pitch bend messages get converted into standard MIDI messages, allowing MPE-enabled MIDI controllers to keep feeding MIDI information to instruments that cannot receive MPE messages.

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
