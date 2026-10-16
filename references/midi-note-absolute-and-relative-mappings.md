# MIDI Note Absolute And Relative Mappings

Open when you need guidance on MIDI Note Absolute And Relative Mappings in Ableton Live.

Context: [The Mapping Browser](midi-and-key-remote-control.md#332-the-mapping-browser).

<a id="source-3321-assigning-midi-remote-control"></a>
### 33.2.1 Assigning MIDI Remote Control

The MIDI Map Mode Switch.

After your remote control setup is in place in the Link, Tempo & MIDI Settings, handing MIDI controllers and notes their remote control assignments is straightforward:

1. Step into MIDI Map Mode by clicking the MIDI switch at Live’s upper right-hand corner. You’ll see the interface’s assignable elements turn blue, and the Mapping Browser open up. Should your browser be closed, Ctrl+Alt+B (Win) / Cmd+Option+B (Mac) opens it.
2. Click whichever Live parameter you intend to drive via MIDI.
3. Fire off a MIDI message — press a keyboard key, twist a knob, and so on — from your MIDI controller. The Mapping Browser then shows this new MIDI mapping in its list.
4. Step back out of MIDI Map Mode by clicking the MIDI switch a second time. The Mapping Browser closes, yet re-entering MIDI Map Mode lets you look over your mappings whenever you wish.

<a id="source-3322-mapping-to-midi-notes"></a>
### 33.2.2 Mapping to MIDI Notes

MIDI notes deliver plain Note On and Note Off messages to elements of Live’s interface. Here is what those messages can do to controls in Live:

- _Session View Slots_ — Note On and Note Off messages act on the slot’s clips in line with their [Launch Mode](https://www.ableton.com/en/live-manual/12/launching-clips/#launch-modes) settings.
- _Switches_ — The switch’s state flips with a Note On message.
- _Radio Buttons_ — Each Note On message steps through the choices on offer.
- _Variable Parameters_ — Mapped to a lone note, Note On messages flip the parameter back and forth between its Min and Max values. Mapped across a span of notes, every note receives its own discrete value, spread evenly across the parameter’s value range.

You can map Session View slots to a MIDI note range for chromatic performance: first strike the _root_ key (the one that triggers the clip at its default transposition), then, _while holding down the root key_, press one key beneath the root and one above it to set the range’s edges.

<a id="source-3323-mapping-to-absolute-midi-controllers"></a>
### 33.2.3 Mapping to Absolute MIDI Controllers

Absolute MIDI controllers hand Live their messages as absolute values spanning 0 to 127. The outcome those values produce hinges on which kind of Live control receives them. Take a value message of 127: it could push a Live track’s Volume control to maximum or trigger a Session View clip. To be precise, MIDI controller messages spanning 0 to 127 can do the following to controls in Live:

- _Session View Slots_ — Controller values from 64 upward behave like Note On messages, whereas controller values of 63 and under behave like Note Off messages.
- _Switches_ — On track activators and on/off buttons inside devices, a controller value falling inside the mapping’s Min and Max range switches it on, while any value above or below that range switches it off. Flip this logic by assigning a Min value greater than its matching Max value; then values lying outside the range switch it on and values inside switch it off. With every other kind of switch (transport controls, for example), controller values from 64 upward switch it on and values under 64 switch it off.
- _Radio Buttons_ — The controller’s 0…127 value range gets mapped across the available choices.
- _Continuous Controls_ — The controller’s 0…127 value range gets mapped across the parameter’s span of values.

Pitch bend messages and high-precision (”14-bit Absolute”) controller messages carrying a 0…16383 value range are supported by Live too. Everything stated above holds for these as well, with the one difference that the value range’s midpoint falls at 8191/8192.

<a id="source-3324-mapping-to-relative-midi-controllers"></a>
### 33.2.4 Mapping to Relative MIDI Controllers

Rather than absolute values, certain MIDI controllers can transmit ”value increment” and ”value decrement” messages. Such controls head off parameter jumps whenever a control’s state in Live and the matching control on the hardware MIDI controller don’t agree. Picture, for instance, mapping the pan knob on your control surface onto a Live track’s pan parameter. With the hardware control panned hard right and the Live control panned hard left, the slightest twist of a hardware pan knob sending absolute values would instruct Live to pan right, jerking the track’s panning abruptly. A pan knob emitting relative messages sidesteps that, because its incremental note to Live merely amounts to ”Pan slightly to the left of your current position.”

Relative controllers come in four flavors: Signed Bit, Signed Bit 2, Bin Offset and Twos Complement.

A ”linear” variant of each is offered as well. A number of MIDI encoders apply ”acceleration” under the hood, producing bigger value changes the faster you spin them. When a control surface isn’t natively supported, Live attempts to work out the controller type along with whether acceleration is at play.

Help the detection along by easing the relative controller leftward slowly as you create an assignment. Live posts its guess in the Status Bar’s ”mode” chooser, but should you already know the relative controller type, you’re free to choose it by hand.

Relative MIDI controller messages prompt Live to behave as follows:

- _Session View Slots_ — Value increment messages behave like Note On messages, and value decrement messages behave like Note Off messages.
- _Switches_ — An increment message switches it on; a decrement message switches it off.
- _Radio Buttons_ — An increment message advances the radio button to the next available choice, while a decrement message steps it back.
- _Continuous Controls_ — Every kind of relative MIDI controller reads the 0…127 MIDI controller value range its own way to work out value increments and decrements.

Refer to the documentation supplied with your MIDI controller should you want to learn more about relative MIDI controllers.
