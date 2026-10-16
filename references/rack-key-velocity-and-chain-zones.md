# Rack Key Velocity And Chain Zones

Open when you need guidance on Rack Key Velocity And Chain Zones in Ableton Live.

Context: [Zones](instrument-drum-and-effect-racks.md#245-zones).

<a id="source-2451-signal-flow-through-zones"></a>
### 24.5.1 Signal Flow through Zones

To get a feel for how zones operate, let’s trace the signal flow through a MIDI Effect Rack. The MIDI Effect Rack in question sits within the device chain of a MIDI track, so what it handles is MIDI signals. Picture it holding four parallel device chains, with a single MIDI effect in each one.

1. Every bit of MIDI data on the track flows into its device chain and from there into the input of the MIDI Effect Rack.
2. The four device chains in our MIDI Effect Rack each take in that same MIDI data simultaneously.
3. No MIDI data reaches a device chain until it has managed to clear every zone belonging to that chain. Inside a MIDI Effect Rack, each chain carries three zones: one for key, one for velocity and one for chain select.
4. An arriving MIDI note is checked against a chain’s key zone. Should the note fall inside the key zone, it moves along to the next zone to be checked; should it fall outside, we already know the note won’t reach that chain’s devices.
5. The chain’s velocity and chain select zones are tested in the same fashion. If the note also sits inside both of them, it then reaches the input of the first device on that chain.
6. The outputs from all the parallel chains get blended together into the MIDI Effect Rack’s finished output. Were there another device positioned after the Rack along the track’s device chain, it would at this stage take in the Rack’s output to process.

<a id="source-2452-key-zones"></a>
### 24.5.2 Key Zones

The Key Zone Editor.

Click the Key button and the Key Zone Editor shows up to the right of the Chain List, depicting how every chain lines up against the entire MIDI note range (close to 11 octaves). A chain reacts solely to MIDI notes falling inside its key zone. Since an individual chain’s zone can span however many keys you like, you’re free to build adaptable “keyboard split“ arrangements.

A key zone’s fade ranges turn down the _velocities_ of notes as they arrive at a chain.

<a id="source-2453-velocity-zones"></a>
### 24.5.3 Velocity Zones

The Velocity Zone Editor.

Every chain within an Instrument Rack or MIDI Effect Rack additionally owns a velocity zone, which lays out the span of MIDI Note On velocities the chain is willing to react to.

Whenever it’s shown, the Velocity Zone Editor takes the place of the Key Zone Editor over on the right of the Chain List. MIDI Note On velocity runs along a scale of 1-127, and that span of values stretches across the editor’s top edge. In every other respect, what you can do here matches the Key Zone Editor exactly.

In the same way, the fade ranges of a velocity zone reduce the velocities of any notes coming into a chain.

<a id="source-2454-chain-select-zones"></a>
### 24.5.4 Chain Select Zones

The Chain Select Editor.

Switching on the Chain button within an Instrument or Effect Rack brings up the Chain Select Editor. Racks of these types carry chain select zones, letting you screen chains on the fly using just one parameter. As with the Velocity Zone Editor, this editor runs along a 0-127 scale. Sitting above that value scale, though, is a draggable marker called the Chain selector.

A chain select zone works as a data filter in exactly the way the other zones do; even though every chain in a Rack is fed input signals, only the chains whose chain select zones cover the Chain selector’s present value can be reached and therefore make any output.

Out of the box, the chain select zones in Instrument and MIDI Effect Racks screen notes alone, paying no attention to any other incoming MIDI events (MIDI CCs among them). If you’d rather screen every MIDI event, switch on the Chain Selector Filters MIDI Ctrl option, which lives in the context menu of a Rack’s Chain Select Ruler.

Within MIDI Effect Racks, the fade ranges scale down the velocities of notes as they enter a chain. Within Instrument Racks and Audio Effect Racks, both of which put out audio signals, the fade ranges instead scale down the volume level at each chain’s output. So what occurs if you drag the Chain selector beyond the chain select zone of a sound that’s playing right then? Where the zone closes with a fade range, that chain’s output volume drops to zero for as long as the Chain selector sits outside the zone. Where the zone had no fade range, the output volume is _not_ scaled down at all, which lets the chain’s effects (long reverb tails or delays, for instance) trail off on their own terms.

Now let’s look at a way to put chain select zones to work during a live performance:
