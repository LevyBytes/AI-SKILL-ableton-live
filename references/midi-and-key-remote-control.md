# Midi And Key Remote Control

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 33. MIDI and Key Remote Control

So that you needn’t reach for the mouse so often, nearly all of Live’s controls can be _remote-controlled_ using an outboard MIDI controller plus the computer keyboard. The pages that follow cover the specifics of mapping to these particular kinds of controls within Live’s interface:

1. _Session View slots_ — Keep in mind that MIDI and computer key assignments attach to the slots themselves, rather than to whatever clips sit inside them.
2. _Switches and buttons_ — These include the Track and Device Activator switches, plus the Control Bar’s tap tempo, metronome and transport controls.
3. _Radio buttons_ — Such a button picks one choice out of several. A typical example is the crossfader assignment area found on every track, which presents three choices: the track sits at the crossfader’s A position, the track ignores the crossfader entirely, or the track responds to the crossfader’s B position.
4. _Continuous controls_ — For instance the mixer’s volume, pan and sends.
5. _The crossfader_ — Its workings get a thorough treatment in the matching part of the [Mixing](https://www.ableton.com/en/live-manual/12/mixing/#using-lives-crossfader) chapter.

### 33.1 MIDI Remote Control

External MIDI control surfaces — MIDI keyboards or controller boxes, for instance — can drive Live from a distance. Dedicated control is likewise available through Ableton [Push 1](https://www.ableton.com/en/live-manual/12/using-push-1/#using-push-1), [Push 2](https://www.ableton.com/en/live-manual/12/using-push-2/#using-push-2), and [Push 3](https://www.ableton.com/push/manual/).

Before getting into how remote control assignments get created and carried out, it helps to separate MIDI remote control from another job MIDI does in Live: feeding our MIDI tracks. Imagine you’re playing an instrument in one of Live’s MIDI tracks from a MIDI keyboard. The moment you map C-1 on that keyboard to a Session View Clip Launch button, the key stops sounding C-1 on your MIDI track’s instrument, because it now ”belongs” exclusively to the Clip Launch button.

_Once a MIDI key is folded into a remote control assignment, it stops working as input to MIDI tracks_. People are frequently tripped up by this, though a glance at the Control Bar’s [MIDI indicators](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#midi-inout-indicators) clears it up right away.

Prior to creating any MIDI assignments, Live has to be configured to detect your control surfaces. You handle this within the Link, Tempo & MIDI tab of Live’s Settings, which the Ctrl, (Win) / Cmd, (Mac) keyboard shortcut brings up.

### 33.1.1 Natively Supported Control Surfaces

You set up Control Surfaces through the menus found in the Link, Tempo & MIDI tab. Live lets you run as many as six supported control surfaces at the same time.

Setting Up Control Surfaces.

To find out if Live natively supports your control surface, open the first chooser in the _Control Surface_ column; should it appear in the list, pick it by name and then assign its MIDI input and output ports with the pair of columns alongside. Don’t worry if your controller is absent from that list — the upcoming [Manual Control Surface Setup](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#manual-control-surface-setup) section lets you enable it by hand.

For certain controllers, Live may require a ”preset dump” before the setup is finished. When that applies, the _Dump_ button — found just past your control surface’s choosers, over on their right within the Live Settings — becomes active. Make sure your control surface is prepared to accept preset dumps before you click it. Since the steps for switching this on differ from one maker and model to the next, check your hardware’s documentation whenever you’re uncertain. At last, click the Dump button, and Live configures your hardware on its own.

#### 33.1.1.1 Instant Mappings

Typically, Live follows a consistent scheme when it maps its functions and parameters onto physical controls. Naturally, the particulars shift according to how the knobs, sliders and buttons are laid out on a given control surface. Such layout-driven schemes carry the name _instant mappings_.

At any point you may _manually override_ an instant mapping with assignments of your own. When you do, you’ll likewise want to switch on the Remote switches for whichever MIDI ports your control surface relies on. That happens in the MIDI Ports section of the Link, Tempo & MIDI Settings tab, which the following section covers.

The benefit of instant mappings is that a control surface’s controllers re-map themselves on the fly to operate whatever device is currently selected in Live.

Control Surfaces Can Follow Device Selection.

Beyond merely tracking device selection, _natively supported_ control surfaces may be ”locked” onto particular devices, so you keep hands-on reach regardless of where focus sits within your Live Set. You turn locking on or off by right-clicking a device’s title bar and then choosing the controller you want from the ”Lock to…” context menu. The list there matches the control surfaces you set up in the Link, Tempo & MIDI Settings. Out of the box, arming a MIDI track for recording locks its instrument to the control surface automatically.

Getting Hands-On: Control Surfaces Can Be Locked to Devices.

You can spot a locked device by the hand icon shown in its title bar, a convenient cue to its state.

Bear in mind that not every control surface supports locking to devices.

### 33.1.2 Manual Control Surface Setup

Should your MIDI control surface be missing from the Link, Tempo & MIDI Settings’ Control Surface chooser, you can still ready it for hand mapping over in this tab’s _MIDI Ports_ section.

Defining Control Surfaces Manually.

Every MIDI input and output port that’s available shows up in the MIDI Ports table. To put an input port to work for remotely controlling Live, confirm that the matching switch in its _Remote_ column reads ”On.” There’s no limit on how many MIDI ports you map remotely; Live combines all of their incoming MIDI signals.

If your control surface offers physical or visual feedback, you’ll need to switch on the Remote switch for its output port as well. That lets Live talk back to these control surfaces whenever a value shifts, so they can move their motorized faders or update their LEDs accordingly.

Try firing off some MIDI data to Live from your control surface as a way to check the setup. Each time Live picks up an arriving MIDI message, the Control Bar’s MIDI indicators flash.

After Live recognizes your controller, the setup stage is done (though it’s worth pausing to choose a Takeover Mode before you exit the Settings). What comes next is building MIDI mappings linking your control surface to Live. Happily, that’s easy, and you tackle just one parameter at a time.

### 33.1.3 Takeover Mode

MIDI Controller Takeover Mode.

Whenever MIDI controls that emit absolute values (faders, say) sit in a bank-switching arrangement, where every controller bank points them at a different destination parameter, you’ll have to settle on how Live should cope with the abrupt value leaps that crop up the first time you nudge a control after a bank change. There are three takeover modes to pick from:

_None_ — The instant you move the physical control, its fresh value goes straight to the destination parameter, which generally causes jarring value jumps.

_Pick-Up_ — Nothing happens when you move the physical control until it catches up to the destination parameter’s value. Once the two match, the destination follows the control’s value 1:1. The upside is smooth value changes, though it’s hard to judge precisely where the pick-up occurs.

_Value Scaling_ — Picking this guarantees gradual value transitions. It weighs the physical control’s value against the destination parameter’s and works out a smooth convergence between them while you move the control. The moment they line up, the destination value follows the control’s value 1:1.

### 33.2 The Mapping Browser

The Mapping Browser.

The _Mapping Browser_ takes charge of every manual MIDI, [computer keyboard](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control) and [Macro Control](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#macro-controls) mapping. It stays out of view until you switch on one of the three mapping modes, whereupon it shows every mapping belonging to that mode. Per mapping, it spells out the control element, the route to the mapped parameter, that parameter’s name, plus the mapping’s _Min_ and _Max_ value ranges. You can revise the assigned Min and Max ranges whenever you like, and a context menu command flips them in an instant. To remove mappings, press your computer’s Backspace (Win) or Delete (Mac) key.

Keep in mind that Instant Mappings depend on context and therefore never appear in the Mapping Browser.

### 33.2.1 Assigning MIDI Remote Control

The MIDI Map Mode Switch.

After your remote control setup is in place in the Link, Tempo & MIDI Settings, handing MIDI controllers and notes their remote control assignments is straightforward:

1. Step into MIDI Map Mode by clicking the MIDI switch at Live’s upper right-hand corner. You’ll see the interface’s assignable elements turn blue, and the Mapping Browser open up. Should your browser be closed, CtrlAltB (Win) / CmdOptionB (Mac) opens it.
2. Click whichever Live parameter you intend to drive via MIDI.
3. Fire off a MIDI message — press a keyboard key, twist a knob, and so on — from your MIDI controller. The Mapping Browser then shows this new MIDI mapping in its list.
4. Step back out of MIDI Map Mode by clicking the MIDI switch a second time. The Mapping Browser closes, yet re-entering MIDI Map Mode lets you look over your mappings whenever you wish.

### 33.2.2 Mapping to MIDI Notes

MIDI notes deliver plain Note On and Note Off messages to elements of Live’s interface. Here is what those messages can do to controls in Live:

- _Session View Slots_ — Note On and Note Off messages act on the slot’s clips in line with their [Launch Mode](https://www.ableton.com/en/live-manual/12/launching-clips/#launch-modes) settings.
- _Switches_ — The switch’s state flips with a Note On message.
- _Radio Buttons_ — Each Note On message steps through the choices on offer.
- _Variable Parameters_ — Mapped to a lone note, Note On messages flip the parameter back and forth between its Min and Max values. Mapped across a span of notes, every note receives its own discrete value, spread evenly across the parameter’s value range.

You can map Session View slots to a MIDI note range for chromatic performance: first strike the _root_ key (the one that triggers the clip at its default transposition), then, _while holding down the root key_, press one key beneath the root and one above it to set the range’s edges.

### 33.2.3 Mapping to Absolute MIDI Controllers

Absolute MIDI controllers hand Live their messages as absolute values spanning 0 to 127. The outcome those values produce hinges on which kind of Live control receives them. Take a value message of 127: it could push a Live track’s Volume control to maximum or trigger a Session View clip. To be precise, MIDI controller messages spanning 0 to 127 can do the following to controls in Live:

- _Session View Slots_ — Controller values from 64 upward behave like Note On messages, whereas controller values of 63 and under behave like Note Off messages.
- _Switches_ — On track activators and on/off buttons inside devices, a controller value falling inside the mapping’s Min and Max range switches it on, while any value above or below that range switches it off. Flip this logic by assigning a Min value greater than its matching Max value; then values lying outside the range switch it on and values inside switch it off. With every other kind of switch (transport controls, for example), controller values from 64 upward switch it on and values under 64 switch it off.
- _Radio Buttons_ — The controller’s 0…127 value range gets mapped across the available choices.
- _Continuous Controls_ — The controller’s 0…127 value range gets mapped across the parameter’s span of values.

Pitch bend messages and high-precision (”14-bit Absolute”) controller messages carrying a 0…16383 value range are supported by Live too. Everything stated above holds for these as well, with the one difference that the value range’s midpoint falls at 8191/8192.

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

#### 33.2.4.1 Relative Session View Navigation

Bear in mind that besides _absolute mappings_ onto particular slots and scenes, you can also create _relative mappings_ that shift the highlighted scene and act on the highlighted clips.

Within both MIDI Map Mode and [Key Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control), a row of assignable controls shows up beneath the Session grid:

The Relative Session Mapping Strip.

1. Map these buttons to keys, notes or controllers so you can shift the highlighted scene upward and downward.
2. Map this scene number value box to a MIDI controller — ideally an endless encoder — for scrolling among the scenes. See the earlier section on [Relative Map Modes](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#mapping-to-relative-midi-controllers) for the specifics.
3. Map this button to launch the highlighted scene. With the Record, Warp & Launch Settings’ Select Next Scene on Launch option ticked, you can advance one after another (and, fingers crossed, successfully!) through the scenes.
4. Map this button to call off the launch of a scene you’ve triggered.
5. Map these buttons to launch the clip sitting at the highlighted scene within each respective track.

Relative Session mapping comes in handy when you’re moving around a big Live Set, since Live consistently parks the highlighted scene at the heart of the Session View.

#### 33.2.4.2 Mapping to Clip View Controls

The [Clip View](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view) shows the settings of whatever clip is selected at the moment, and it likewise shows the settings when several clips are selected together. So you don’t run into jarring musical surprises, bear in mind that adding a remote control mapping to any Clip View control might touch _any_ clip in the Live Set. That’s why we suggest mapping Clip View controls to relative MIDI controllers, which keeps parameter values from leaping unexpectedly.

### 33.2.5 Computer Keyboard Remote Control

The Key Map Mode Switch.

Setting up control surface assignments for your computer keyboard is easy:

1. Step into Key Map Mode by clicking the KEY switch, which sits at the top right of the Live screen. Once you’re in Key Map Mode, the interface’s assignable elements glow red. The Mapping Browser opens up too. Should the Browser be hidden, now is the time to reveal it with the relevant View menu command.
2. Click whichever Live parameter you’d like to bind to a key. Keep in mind that only the controls wearing a red overlay can be mapped.
3. Strike the computer key you want to tie to the control. Your new mapping’s particulars then appear in the Mapping Browser.
4. Exit Key Map Mode by clicking Live’s KEY switch once more. The Mapping Browser vanishes, yet you can look over your mappings anytime by simply re-entering Key Map Mode.

In Live, keyboard assignments can bring about the following:

- Mapped keys act on clips in Session View slots in line with their [Launch Mode](https://www.ableton.com/en/live-manual/12/launching-clips/#launch-modes) settings.
- Keys bound to switches flip switch states.
- Keys bound to radio buttons cycle through the available choices.

Take care not to mix up this remote control capability with Live’s knack for treating the [computer keyboard](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#playing-midi-with-the-computer-keyboard) as a pseudo-MIDI keyboard, which turns computer keystrokes into MIDI notes you can feed to instruments.
