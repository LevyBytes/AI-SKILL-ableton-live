# Max Envelope MIDI And Expression Control

Open when you need guidance on Max Envelope MIDI And Expression Control in Ableton Live.

Context: [Max for Live MIDI Effects](max-for-live-devices.md#323-max-for-live-midi-effects).

<a id="source-3231-envelope-midi"></a>
### 32.3.1 Envelope MIDI

The Envelope MIDI Effect.

Envelope MIDI is a modulator device that drives mapped parameters through an ADSR envelope.

Within Live, any automatable parameter — device or mixer controls included — can be tied to Envelope MIDI. To do so, switch on the Map button and click the parameter you want as the mapping target.

The Show/Hide Multimap button at the display's top right exposes more mapping buttons, allowing as many as eight parameters to be mapped.

You Can Map up to Eight Parameters.

To remove an assignment, click the Unmap button located to the right of the Map button.

Envelope MIDI steers mapped parameters by one of two methods: Modulation and Remote Control. Modulation is chosen by default, and the Mod toggle moves you to Remote Control.

While Modulation is active, you can keep adjusting parameter values by hand after mapping. The Modulation Polarity toggle alternates between Bipolar and Unipolar modes. Bipolar mode modulates both ways around a centered base value; Unipolar mode works in a single direction out from the base value. Set the modulation depth with the Modulation Amount slider, which determines the range relative to the base value.

Once Remote Control is active, the mapped values are fixed entirely by Envelope MIDI and resist manual change. Scale the modulation range using the Min and Max sliders.

The Loop Mode drop-down offers four choices: Free, Sync, Loop, and Echo.

- Free: Every note that plays fires the envelope once.
- Sync: The envelope retriggers on the beat division chosen in the Sync Rate drop-down.
- Loop: The envelope repeats at the rate the Global Time control specifies.
- Echo: The envelope spawns echoes spaced by the Env Echo Time control. How much of each echo carries into the following one is set by the Env Feedback control, which in turn governs how long the echoes linger; raising feedback yields longer-lasting repeats.

Each time the envelope fires, the LED beside the Loop Mode drop-down flashes.

The envelope's duration is scaled by Global Time. Its default of 1.00 keeps the envelope at the timing the ADSR values dictate. Settings above 1.00 stretch the envelope proportionally, and settings below 1.00 squeeze it.

For all mapped parameters, the modulation amount is governed by the Amount control. At 0% nothing is modulated; at 100% the envelope output reaches its peak strength.

Attack fixes how long the envelope takes to climb to its peak once a note sounds. Decay sets how long it takes to fall from that peak down to the Sustain level.

The level the envelope holds after the Decay stage while a note stays down is defined by the Sustain control. The Release control determines how long the envelope takes to fall back to zero after the note lifts.

For the matching stages, curved envelope segments can be drawn using the Slope sliders sitting beneath Attack, Decay, and Release.

You can likewise set the Attack, Decay, Sustain, and Release values — plus the ADR slopes — by grabbing and dragging the envelope handles in the display.

Turn on the Velocity toggle and the envelope's peak scales in proportion to each incoming note's velocity. Softer notes yield a lower peak and gentler modulation, whereas harder ones produce a higher peak and stronger modulation.

The Sustain toggle turns the sustain behavior on or off. When on, the envelope holds at the Sustain level for the duration the note is held and only advances to the Release stage once the note lifts. When off, the envelope acts as a one-shot — it runs through the Attack and Decay stages and then moves into Release no matter how long the note is held.

<a id="source-3232-expression-control"></a>
### 32.3.2 Expression Control

The Expression Control Effect.

Expression Control is a modulator device that governs mapped parameters from a choice of MIDI and MPE sources.

It provides five Mod Source tabs, and each one can be pointed at a particular MIDI or MPE source. From the MIDI Input Source drop-down menu you pick whichever expression parameter you need; the ten on offer are Velocity, Modwheel, Pitchbend, Pressure, Keytrack, Expression, Random, Increment, Slide, and Sustain.

Within Live, any automatable parameter — device or mixer controls among them — can be assigned to the chosen modulation source. To do this, switch on the Map button and click a parameter to set it as the mapping target.

Which controls appear in the Output Range section is dictated by the Modulation toggle at the device's top right. That toggle decides how Expression Control produces its modulation values and offers two modes: Modulate or Remote Control.

Pick Modulate and you can still nudge a mapped parameter's base value with the cursor. In this mode, whatever Expression Control sets or automates blends with the value you dial in as you adjust that parameter. Pick Remote Control instead and Expression Control alone determines the modulated values, leaving the base parameter values beyond reach.

<a id="source-max-for-live-devices-part-2"></a>

The Modulation toggle additionally influences the polarity behavior of Expression Control. Choosing Modulate reveals a Modulation Polarity toggle within the Output Range section, where you pick either bipolar or unipolar operation. With Bipolar mode active, the modulation pivots around whichever base parameter value is currently being modulated. With Unipolar mode active, the modulation gets summed onto that base parameter value instead. The Output Range Max slider determines the modulation output produced once the incoming signal hits its peak amplitude. Selecting Remote Control instead turns the Output Range section into a place where you define both a floor and a ceiling for the modulation output, controlled through the Output Range Min and Output Range Max sliders.

Use the Curve Type buttons sitting underneath the Curve Display to pick either a linear or an S-shaped curve. Whichever curve type you pick governs the set of controls offered within the Curve section.

With a linear curve chosen (it carries two breakpoints), the Curve A dial reshapes the whole modulation curve at once. Pick an S-shaped curve (which has three breakpoints) and the Curve A dial then governs the upper part of the curve while the Curve B dial governs the lower part. Enabling the Curve Link button means the upper and lower portions move in opposite directions through the single Curve A dial alone.

The Curve Display gives you a visual look at the modulation curve the device is currently producing. You define the curve's lowest and highest values through the Min/Max sliders. With an S-shaped curve active, the X-Y sliders let you position the middle breakpoint both horizontally and vertically. You can equally reshape the breakpoints and overall curve by dragging the rendered curve right inside the display.

Picking Increment as the modulation source from any MIDI Input Source drop-down menu switches on the Increment Steps slider. That setting governs the number of note triggers required to traverse the device's full modulation range, accepting any value from 1 to 32 steps. Halting transport clears the counter, meaning the very first note after transport resumes emits whatever minimum modulation value you configured.

Picking Random as the modulation source from any MIDI Input Source drop-down menu switches on the Random Amount slider. Use this slider to dial in how much random spread is applied around the target modulation value at every note trigger.

Through the Smoothing Type toggle you decide whether smoothing across modulation values follows a linear or a logarithmic path.

The Smoothing Rise and Fall sliders govern how long, between 0 and 1000 milliseconds, rising and falling modulation values take before they arrive at the latest value.
