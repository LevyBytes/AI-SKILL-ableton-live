# MIDI Remote Control Overview

Open when you need guidance on MIDI Remote Control Overview in Ableton Live.

Context: [MIDI and Key Remote Control](midi-and-key-remote-control.md#33-midi-and-key-remote-control).

<a id="source-331-midi-remote-control"></a>
### 33.1 MIDI Remote Control

External MIDI control surfaces — MIDI keyboards or controller boxes, for instance — can drive Live from a distance. Dedicated control is likewise available through Ableton [Push 1](https://www.ableton.com/en/live-manual/12/using-push-1/#using-push-1), [Push 2](https://www.ableton.com/en/live-manual/12/using-push-2/#using-push-2), and [Push 3](https://www.ableton.com/push/manual/).

Before getting into how remote control assignments get created and carried out, it helps to separate MIDI remote control from another job MIDI does in Live: feeding our MIDI tracks. Imagine you’re playing an instrument in one of Live’s MIDI tracks from a MIDI keyboard. The moment you map C-1 on that keyboard to a Session View Clip Launch button, the key stops sounding C-1 on your MIDI track’s instrument, because it now ”belongs” exclusively to the Clip Launch button.

_Once a MIDI key is folded into a remote control assignment, it stops working as input to MIDI tracks_. People are frequently tripped up by this, though a glance at the Control Bar’s [MIDI indicators](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#midi-inout-indicators) clears it up right away.

Prior to creating any MIDI assignments, Live has to be configured to detect your control surfaces. You handle this within the Link, Tempo & MIDI tab of Live’s Settings, which the Ctrl+, (Win) / Cmd+, (Mac) keyboard shortcut brings up.
