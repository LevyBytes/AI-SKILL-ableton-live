# Control Surface Manual Setup And Takeover

Open when you need guidance on Control Surface Manual Setup And Takeover in Ableton Live.

Context: [MIDI Remote Control](midi-and-key-remote-control.md#331-midi-remote-control).

<a id="source-3312-manual-control-surface-setup"></a>
### 33.1.2 Manual Control Surface Setup

Should your MIDI control surface be missing from the Link, Tempo & MIDI Settings’ Control Surface chooser, you can still ready it for hand mapping over in this tab’s _MIDI Ports_ section.

Defining Control Surfaces Manually.

Every MIDI input and output port that’s available shows up in the MIDI Ports table. To put an input port to work for remotely controlling Live, confirm that the matching switch in its _Remote_ column reads ”On.” There’s no limit on how many MIDI ports you map remotely; Live combines all of their incoming MIDI signals.

If your control surface offers physical or visual feedback, you’ll need to switch on the Remote switch for its output port as well. That lets Live talk back to these control surfaces whenever a value shifts, so they can move their motorized faders or update their LEDs accordingly.

Try firing off some MIDI data to Live from your control surface as a way to check the setup. Each time Live picks up an arriving MIDI message, the Control Bar’s MIDI indicators flash.

After Live recognizes your controller, the setup stage is done (though it’s worth pausing to choose a Takeover Mode before you exit the Settings). What comes next is building MIDI mappings linking your control surface to Live. Happily, that’s easy, and you tackle just one parameter at a time.

<a id="source-3313-takeover-mode"></a>
### 33.1.3 Takeover Mode

MIDI Controller Takeover Mode.

Whenever MIDI controls that emit absolute values (faders, say) sit in a bank-switching arrangement, where every controller bank points them at a different destination parameter, you’ll have to settle on how Live should cope with the abrupt value leaps that crop up the first time you nudge a control after a bank change. There are three takeover modes to pick from:

_None_ — The instant you move the physical control, its fresh value goes straight to the destination parameter, which generally causes jarring value jumps.

_Pick-Up_ — Nothing happens when you move the physical control until it catches up to the destination parameter’s value. Once the two match, the destination follows the control’s value 1:1. The upside is smooth value changes, though it’s hard to judge precisely where the pick-up occurs.

_Value Scaling_ — Picking this guarantees gradual value transitions. It weighs the physical control’s value against the destination parameter’s and works out a smooth convergence between them while you move the control. The moment they line up, the destination value follows the control’s value 1:1.
