# MPE Control Pressure Slide And Pitch

Open when you need guidance on MPE Control Pressure Slide And Pitch in Ableton Live.

Context: [MPE Control](max-midi-modulation-and-monitoring-routes.md#3234-mpe-control).

<a id="source-32341-press"></a>
#### 32.3.4.1 Press

The Press source lets you reshape MPE pressure data, which, much like polyphonic aftertouch, travels on a per-note basis whenever pressure lands on a controller's key or pad once it has already been struck.

Press Advanced Settings.

Press carries a Default toggle, letting you assign a default MPE value for use with MIDI notes that arrive without MPE data. You may also route the MPE pressure data toward the Slide rather than the Press source through the Swap to Slide toggle. That comes in handy when, say, you'd rather adjust modulation along the vertical axis yet your controller offers only polyphonic aftertouch.

The Press to AT setting turns the MPE pressure data into monophonic aftertouch, so an MPE controller can modulate non-MPE instruments.

<a id="source-32342-slide"></a>
#### 32.3.4.2 Slide

The Slide source reshapes MPE slide data (sent as MIDI CC 74), which maps to where the finger sits vertically on the controller key or pad.

Slide Advanced Settings.

Slide likewise carries a Default toggle for non-MPE data, plus a Centered switch that helps when performing on pad-based MPE controllers. Turn Centered on and MPE slide data gets reshaped so that striking the pad's center yields a modulation value of zero, with that value climbing steadily as the finger travels away from center along the vertical axis.

Out of the box, Slide sits in Abs mode, treating MPE slide values as absolute. Flipping the mode to Rel (relative) makes the slide values begin at the middle of the range no matter where the finger rests on the key or pad. They can then change only by sweeping the finger further up and down while a note is held. Under Ons (onset) mode, MPE slide values refresh only at a Note On. Be aware that onset mode switches smoothing off automatically.

The Slide to Mod option turns MPE slide messages into Mod Wheel (CC1) messages, which lets an MPE controller modulate non-MPE enabled instruments.

<a id="source-32343-notepb"></a>
#### 32.3.4.3 NotePB

The NotePB source reshapes the MPE per-note pitch bend data, which comes from horizontal motion across the controller's keys or pads. By its nature, pitch bend influences only the pitch or pitches being sounded.

NotePB Advanced Settings.

Within the NotePB advanced settings you can set the Pitch Range, handy when the hardware controller's pitch bend range and the instrument's do not line up. As an example, a 2x setting lets you map an MPE controller carrying a +/- 48 semitone pitch bend range onto an instrument whose range is +/- 24 semitones. Should the Note Pitch Bend MIDI CC be routed to something besides pitch, higher values let you span a wider modulation range from a smaller gesture.

Turn the NotePB to PB switch on and MPE per-note pitch bend messages get converted into standard MIDI messages, allowing MPE-enabled MIDI controllers to keep feeding MIDI information to instruments that cannot receive MPE messages.
