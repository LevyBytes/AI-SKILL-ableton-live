# Rack Signal Flow And Macros

Open when you need guidance on Rack Signal Flow And Macros in Ableton Live.

Context: [An Overview of Racks](instrument-drum-and-effect-racks.md#241-an-overview-of-racks).

<a id="source-2411-signal-flow-and-parallel-device-chains"></a>
### 24.1.1 Signal Flow and Parallel Device Chains

Inside An Audio Effect Rack.

Within every one of Live’s tracks, the devices sit in series along a device chain, each handing its signal to the following one as you move from left to right. The Device View initially shows just one chain, yet a track can in fact hold as many chains as you like.

One of the things Racks make possible is appending extra device chains onto any track. Once a track holds several chains, those chains run in _parallel_: within Instrument and Effect Racks, every chain is fed the identical input signal simultaneously, after which it handles that signal _serially_ through the devices it contains. The results from all the parallel chains are then blended together to form the Rack’s output.

Drum Racks likewise permit several parallel chains to run at once, though they treat their input in a distinct way: instead of all sharing the same input signals, each Drum Rack chain is driven by just one MIDI note assigned to it.

_Everything held inside a given Rack behaves, in effect, as one self-contained device_. So dropping a fresh Rack anywhere along a device chain works exactly like inserting any ordinary device, and a Rack may hold as many further Racks as you wish. Should additional devices sit after a Rack along a track’s device chain, that Rack’s output flows onward to them in the usual manner.

<a id="source-2412-macro-controls"></a>
### 24.1.2 Macro Controls

The Macro Controls.

A distinctive feature that sets Racks apart is the Macro Controls they provide.

The Macro Controls amount to a row of knobs, and any one of them can be wired to as many parameters as you like, drawn from whichever devices sit inside a Rack. What you do with them is entirely your call — perhaps simply for ease, surfacing a key device parameter so it’s within quick reach; perhaps to sculpt unusual, multi-parameter shifts of rhythm and tone; or perhaps to assemble a mega-synth and then tuck it out of view behind one bespoke panel. Consult [Using the Macro Controls](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#using-the-macro-controls) for a thorough walkthrough of the process.

To squeeze out maximum expressiveness, consider [MIDI-mapping](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#assigning-midi-remote-control) the Macro Controls onto an outboard control surface.
