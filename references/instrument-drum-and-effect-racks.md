# Instrument Drum And Effect Racks (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 24. Instrument, Drum and Effect Racks

Inside An Audio Effect Rack.

Think of a Rack as a versatile workspace for combining effects, plug-ins and instruments within a track’s device chain. With one you can assemble elaborate signal processors, expressive performance instruments, layered synthesizers and much else besides. At the same time, a Rack tidies up your device chain by gathering your most important controls in one spot. And although Racks shine when juggling several devices at once, they can even enrich a lone device by establishing fresh control links among its parameters.

### 24.1 An Overview of Racks

### 24.1.1 Signal Flow and Parallel Device Chains

Inside An Audio Effect Rack.

Within every one of Live’s tracks, the devices sit in series along a device chain, each handing its signal to the following one as you move from left to right. The Device View initially shows just one chain, yet a track can in fact hold as many chains as you like.

One of the things Racks make possible is appending extra device chains onto any track. Once a track holds several chains, those chains run in _parallel_: within Instrument and Effect Racks, every chain is fed the identical input signal simultaneously, after which it handles that signal _serially_ through the devices it contains. The results from all the parallel chains are then blended together to form the Rack’s output.

Drum Racks likewise permit several parallel chains to run at once, though they treat their input in a distinct way: instead of all sharing the same input signals, each Drum Rack chain is driven by just one MIDI note assigned to it.

_Everything held inside a given Rack behaves, in effect, as one self-contained device_. So dropping a fresh Rack anywhere along a device chain works exactly like inserting any ordinary device, and a Rack may hold as many further Racks as you wish. Should additional devices sit after a Rack along a track’s device chain, that Rack’s output flows onward to them in the usual manner.

### 24.1.2 Macro Controls

The Macro Controls.

A distinctive feature that sets Racks apart is the Macro Controls they provide.

The Macro Controls amount to a row of knobs, and any one of them can be wired to as many parameters as you like, drawn from whichever devices sit inside a Rack. What you do with them is entirely your call — perhaps simply for ease, surfacing a key device parameter so it’s within quick reach; perhaps to sculpt unusual, multi-parameter shifts of rhythm and tone; or perhaps to assemble a mega-synth and then tuck it out of view behind one bespoke panel. Consult [Using the Macro Controls](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#using-the-macro-controls) for a thorough walkthrough of the process.

To squeeze out maximum expressiveness, consider [MIDI-mapping](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#assigning-midi-remote-control) the Macro Controls onto an outboard control surface.

### 24.2 Creating Racks

Live’s devices are spanned by four kinds of Rack: Instrument Racks, Drum Racks, Audio Effect Racks and MIDI Effect Racks. Much like the track types, every Rack variety follows its own rules about which devices may live inside it:

- _MIDI Effect Racks_ hold MIDI effects exclusively and are only allowed on MIDI tracks.
- _Audio Effect Racks_ hold audio effects exclusively and belong on audio tracks. They may also sit on MIDI tracks, provided they are “downstream“ from an instrument.
- _Instrument Racks_ hold instruments, yet they may additionally take in both MIDI and audio effects. When they do, every MIDI effect must come first along the Instrument Rack’s device chain, with an instrument next, and any audio effects after that.
- _Drum Racks_ resemble Instrument Racks; they accept instruments together with MIDI and audio effects, and the ordering of those devices obeys the very same signal flow rules. On top of that, Drum Racks may house as many as six return chains of audio effects, each driven by its own send level from the chains in the main Rack.

Racks can be made in more than one way. To spin up a brand-new, empty Rack, drag a generic Rack preset (“_Audio Effect Rack_,“ say) out of the browser and onto a track. From there you can drop devices straight into the Rack’s Chain List or Devices view, both covered in the section that follows.

Suppose a track already holds one or more devices you’d like to bundle into a Rack. In that case, click the title bars of those devices in the Device View, then right-click one of those title bars to bring up the _Group_ and _Group to Drum Rack_ commands in the context menu. Keep in mind that issuing this command once more on the same device produces a Rack nested inside a Rack. The identical method lets you group several chains within a Rack, and that too yields a Rack inside a Rack. Throughout the Device View, a Rack’s contents always sit enclosed by end brackets: much like with punctuation or in mathematics, a Rack lodged within a Rack carries one pair of brackets nested inside another.

When you want to ungroup devices and break apart their Racks, click the _Rack’s_ title bar, then reach for the _Ungroup_ command either via the Edit menu or through the context menu.

### 24.3 Looking at Racks

Components of an Effect Rack.Components of a Drum Rack.

1. Each Rack offers separate views that you can reveal or conceal whenever you wish. To support this, every Rack carries a _view column_ along its far-left edge housing the matching view selectors. Which selectors actually show up varies according to whether you’re dealing with an Instrument, Drum or Effect Rack.
2. _Macro Controls_
3. _Chain List_ - Within Drum Racks, this view may hold drum chains as well as return chains.
4. _Devices_
5. You can also recognize Racks by their rounded corners, which frame and surround whatever they hold. Once the Devices view is on display, the _end bracket_ pulls away on its own so the Rack hierarchy stays easy to read.
6. _Pad View_ - Found only in [Drum Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#pad-view).

If you’d like to move, copy or remove a whole Rack in one go, just click its title bar to select it (not the title bars of the devices held inside). With a Rack selected, you can rename it as well through the Edit menu’s _Rename_ command. You’re also free to add your own info text to a Rack using the Edit Info Text command, reachable from the Edit menu or from the Racks’s context menu.

Once every one of a Rack’s views is concealed, its title bar tucks itself into the view column, shrinking the whole Rack down as narrow as it will go. The outcome matches what you’d get by picking Fold from the context menu or by double-clicking the Rack’s title bar.

Should you need to find a specific device inside a Rack without hunting by hand through everything it holds, you’ll be glad of this navigation trick: right-click the Device View selector, and a tiered list of every device in the track’s device chain pops up. Pick any entry from that list, and Live selects the device and brings it into view on your behalf.

Navigate Racks Quickly Via a Context Menu.

### 24.4 Chain List

The Chain List in an Audio Effect Rack.

The moment signals arrive at a Rack, the Chain List is what meets them first. For that reason, we’ll begin our own tour right here too.

For signals coming in, the Chain List is where the split happens: every parallel device chain begins right here as its own listing. Underneath the list sits a drop area into which you can introduce new chains by dragging and dropping presets, devices, or even chains that already exist.

Note: Racks, chains and devices may be dragged in and out of other Racks at will, and even passed from track to track. If you select a chain and then drag while hovering over a different Session or Arrangement View track, that track takes focus; its Device View springs open so you can drop your chain where you want it.

Because the Device View can only display a single device chain at any moment, the Chain List doubles as a way to get around: whatever you pick in the list governs what appears in the neighboring Devices view (when it’s switched on). Give the up and down arrow keys on your computer keyboard a try to shift which entry is selected in the Chain List, and you’ll see how rapidly you can page through everything a Rack holds.

On top of that, the Chain List lets you select multiple chains at once, which makes copying, arranging and regrouping them easy. When you do, the Devices view reports just how many chains you have selected at the moment.

Every chain comes with its own Chain Activator plus Solo and Hot-Swap buttons. Chains living in Instrument, Drum and Audio Effect Racks additionally carry their own volume and pan sliders, while Drum Rack chains throw in extra send level and MIDI assignment controls. Just as with Live Clips, whole chains may be stored and called back up as presets from the browser. To label a chain meaningfully, select it and then pick the Edit menu’s Rename command. You can likewise attach your own info text to a chain through the Edit Info Text command, found in the Edit menu or in the chain’s context menu. That context menu also offers a color palette from which you can assign a custom chain color.

### 24.4.1 Auto Select

Auto Select in an Audio Effect Rack.

Turn on the Auto Select switch and each chain that happens to be processing signals at that instant gets highlighted in the Chain List. Inside Drum Racks, the feature picks out a chain whenever it’s fed its assigned MIDI input note. Within Instrument and Effect Racks, Auto Select operates hand in hand with zones — covered just below — and proves rather handy when you’re trying to debug elaborate setups.

### 24.5 Zones

Zones are collections of data filters positioned at the input of every chain inside an Instrument or Effect Rack. Acting together, they set which range of values is allowed through to the device chain. Out of the box, zones stay invisible in their effect and never call for your involvement. Even so, you can reconfigure them to build refined control arrangements. There are three zone types — _Key_, _Velocity_, and _Chain Select_ — and their editors are switched on with the buttons sitting above the Chain List. The Hide button right beside them tucks the editors away again.

Note: Audio Effect Racks lack key and velocity zones, because those two zone kinds only filter MIDI data. In the same way, Drum Racks carry no zones whatsoever; instead they sift MIDI notes by means of the choosers found in their chain lists.

Each zone is built from a larger lower portion, which you grab to resize and reposition the zone itself, plus a slim upper portion that sets the fade ranges. To resize either portion, click and drag along its left or right edge; to reposition a zone, click and drag it from any spot other than those edges.

### 24.5.1 Signal Flow through Zones

To get a feel for how zones operate, let’s trace the signal flow through a MIDI Effect Rack. The MIDI Effect Rack in question sits within the device chain of a MIDI track, so what it handles is MIDI signals. Picture it holding four parallel device chains, with a single MIDI effect in each one.

1. Every bit of MIDI data on the track flows into its device chain and from there into the input of the MIDI Effect Rack.
2. The four device chains in our MIDI Effect Rack each take in that same MIDI data simultaneously.
3. No MIDI data reaches a device chain until it has managed to clear every zone belonging to that chain. Inside a MIDI Effect Rack, each chain carries three zones: one for key, one for velocity and one for chain select.
4. An arriving MIDI note is checked against a chain’s key zone. Should the note fall inside the key zone, it moves along to the next zone to be checked; should it fall outside, we already know the note won’t reach that chain’s devices.
5. The chain’s velocity and chain select zones are tested in the same fashion. If the note also sits inside both of them, it then reaches the input of the first device on that chain.
6. The outputs from all the parallel chains get blended together into the MIDI Effect Rack’s finished output. Were there another device positioned after the Rack along the track’s device chain, it would at this stage take in the Rack’s output to process.

### 24.5.2 Key Zones

The Key Zone Editor.

Click the Key button and the Key Zone Editor shows up to the right of the Chain List, depicting how every chain lines up against the entire MIDI note range (close to 11 octaves). A chain reacts solely to MIDI notes falling inside its key zone. Since an individual chain’s zone can span however many keys you like, you’re free to build adaptable “keyboard split“ arrangements.

A key zone’s fade ranges turn down the _velocities_ of notes as they arrive at a chain.

### 24.5.3 Velocity Zones

The Velocity Zone Editor.

Every chain within an Instrument Rack or MIDI Effect Rack additionally owns a velocity zone, which lays out the span of MIDI Note On velocities the chain is willing to react to.

Whenever it’s shown, the Velocity Zone Editor takes the place of the Key Zone Editor over on the right of the Chain List. MIDI Note On velocity runs along a scale of 1-127, and that span of values stretches across the editor’s top edge. In every other respect, what you can do here matches the Key Zone Editor exactly.

In the same way, the fade ranges of a velocity zone reduce the velocities of any notes coming into a chain.

### 24.5.4 Chain Select Zones

The Chain Select Editor.

Switching on the Chain button within an Instrument or Effect Rack brings up the Chain Select Editor. Racks of these types carry chain select zones, letting you screen chains on the fly using just one parameter. As with the Velocity Zone Editor, this editor runs along a 0-127 scale. Sitting above that value scale, though, is a draggable marker called the Chain selector.

A chain select zone works as a data filter in exactly the way the other zones do; even though every chain in a Rack is fed input signals, only the chains whose chain select zones cover the Chain selector’s present value can be reached and therefore make any output.

Out of the box, the chain select zones in Instrument and MIDI Effect Racks screen notes alone, paying no attention to any other incoming MIDI events (MIDI CCs among them). If you’d rather screen every MIDI event, switch on the Chain Selector Filters MIDI Ctrl option, which lives in the context menu of a Rack’s Chain Select Ruler.

Within MIDI Effect Racks, the fade ranges scale down the velocities of notes as they enter a chain. Within Instrument Racks and Audio Effect Racks, both of which put out audio signals, the fade ranges instead scale down the volume level at each chain’s output. So what occurs if you drag the Chain selector beyond the chain select zone of a sound that’s playing right then? Where the zone closes with a fade range, that chain’s output volume drops to zero for as long as the Chain selector sits outside the zone. Where the zone had no fade range, the output volume is _not_ scaled down at all, which lets the chain’s effects (long reverb tails or delays, for instance) trail off on their own terms.

Now let’s look at a way to put chain select zones to work during a live performance:

#### 24.5.4.1 Making Preset Banks Using Chain Select

Using Chain Select Zones to Create Effects Presets.

In contrast to the other zone types, a chain select zone starts out with a length of 1 and a value of 0. Beginning from that arrangement, the Chain Select Editor lets us whip up “preset banks“ in short order.

Once more, let’s take a Rack holding four chains as our point of departure. The four chains each house a different set of effects that we’d like to flip among. So that this feels truly “hands-on,“ we’ve gone ahead and MIDI-mapped the Chain selector onto an encoder on an external control surface.

Let’s shift the chain select zones belonging to the second and third chains so that every zone lands on its own neighboring value: the first chain’s zone sits at 0, the second chain’s zone at 1, the third at 2, and the fourth at 3.

Because every one of our chain select zones now holds a distinct value and none of them overlap, we’ve arrived at a state in which just a single chain can ever match the Chain selector value (displayed across the editor’s top) at any given moment. As a result, sliding the Chain selector is what decides which chain gets to process signals. With our MIDI encoder ready to go, switching between instrument or effect setups becomes wonderfully easy.

#### 24.5.4.2 Crossfading Preset Banks Using Fade Ranges

Crossfading Between Effects Presets Using Chain Select Zones.

Pushing the earlier example a notch further, we can adjust our chain select zones so they glide smoothly from one of our “presets“ to the next. Pulling that off means putting our zones’ _fade ranges_ to use.

So there’s space for fading to happen, let’s stretch our zones out a little. Arranging the zones the way shown keeps four exclusive values for the presets intact, ensuring each one still has a spot where none of the others sound. The crossfade between presets unfolds across eight steps. Should that prove too abrupt for your material, just reposition the zones to make the fade ranges as wide as possible.

### 24.6 Drum Racks

Drum Racks have come up a few times already, and the bulk of what they offer matches what you’ll find in Instrument and Effect Racks. Even so, Drum Racks sport a somewhat different layout, a handful of one-of-a-kind controls and particular behaviors tuned for building drum kits.

The Chain List in a Drum Rack.

1. On top of the usual selectors present on every Rack, Drum Racks add four further controls to the view column. Reading downward, you’ll find toggles that open the Input/Output, Send, and Return sections, capped off by the Auto Select button.
2. _Input/Output Section_ - The Receive chooser picks the incoming MIDI note the drum chain reacts to. Its list presents note names, MIDI note numbers and the standard GM drum equivalents. The Play slider determines the outgoing MIDI note dispatched to the chain’s devices. With the Choke chooser you can assign a chain to any one of sixteen choke groups. Chains sharing a choke group cut each other off whenever one is triggered. That comes in handy for choking an open hihat by hitting a closed one, say. When “All Notes“ is chosen in the Receive chooser, the Play and Choke choosers go inactive — and here the chain just hands whatever note it gets straight to its devices. The little Preview button just left of these choosers shoots a note into the chain, so verifying your mappings is simple even without a MIDI controller nearby.
3. _Mixer Section_ - Beyond the mixer and Hot-Swap controls common to the other Rack types, Drum Racks also include send sliders. Each slider lets you dial in how much post-fader signal travels from a given drum chain to whichever return chains exist. Bear in mind that the send controls stay unavailable until you’ve made some return chains.
4. _Return Chains_ - The return chains of a Drum Rack show up in their own section down at the foot of the chain list. You can place as many as six chains of audio effects there, and they’re supplied by the send sliders on each of the drum chains overhead.

Found in the mixer for return chains, the Audio To chooser lets you send a return chain’s output either to the Rack’s main output or straight to the Set’s return tracks.

### 24.6.1 Pad View

Pad View.

Belonging solely to Drum Racks, the Pad View gives you a straightforward means of mapping and working with samples and devices. A single pad stands in for one of the 128 MIDI notes on offer. Off to the left, the pad overview moves the visible group of pads up or down sixteen at a time, whether you drag the view selector to a fresh spot or press the up and down arrow keys on your computer keyboard. Hold the Alt (Win) / Cmd (Mac) modifier to nudge the view one row at a time instead.

Nearly anything out of Live’s browser — samples, effects, instruments and presets alike — can be dragged onto a pad, where it maps itself to that pad’s note and builds or rearranges the internal chains and devices as required. Drop a sample onto an empty pad, for instance, and you get a fresh chain holding a Simpler, the dropped sample primed to sound from the pad’s note. Drag an audio effect onto that same pad afterward and it lands downstream of the Simpler within the same chain. Replacing the Simpler is as easy as dropping a different sample onto the same pad — whatever audio effects sit downstream or MIDI effects sit upstream stay untouched, and only the Simpler and its sample get swapped out.

Besides dragging objects over from the browser, you can stock pads in a hurry using Hot-Swap. While Hot-Swap mode is active, tapping the D key flips the Hot-Swap target back and forth between the Drum Rack as a whole and the pad you most recently selected.

Drop a multi-selection of samples onto a pad and fresh Simplers and chains get laid out chromatically climbing from that pad, overwriting whatever other samples might already have been parked on the pads involved (yet, as before, leaving any effects devices be). Alt (Win) / Cmd (Mac)-dragging such a multi-selection stacks every sample onto one pad by spinning up a nested Instrument Rack.

Drag one pad onto another and the two pads exchange their note mappings. The upshot is that any MIDI clips firing the affected notes will now sound the “wrong“ sounds — though that may be precisely the effect you were after. Alt (Win) / Cmd (Mac)-dragging a pad onto another instead stacks the chains from both pads together inside a nested Instrument Rack.

Your mappings can be altered straight from the chain list too, simply by tweaking the Receive choosers. The Pad View refreshes on its own to mirror whatever you change. Assign the same Receive note across several chains and the pad for that note will set off every one of them.

When you’ve got plenty of nested Racks on the go, the internal arrangement can grow tangled fast. Pad View eases that considerably by letting you concentrate purely on the top tier: the notes and the sounds. Bear in mind that a pad stands for a note, not a chain. Put more precisely, it stands for every chain — however far down in the Rack it lives — that’s capable of receiving that pad’s note. How much each pad puts at your fingertips depends on the number of chains it stands for:

- A pad with nothing on it displays just the note it’s set to trigger. Hover the mouse over it and the Status Bar shows that note along with the suggested GM instrument.
- A pad tied to a single chain displays that chain’s name. Here the pad acts as a convenient front-end for many of the controls you’d ordinarily reach in the chain list — mute, solo, preview and Hot-Swap among them. From the pad you can rename and delete the chain too.
- A pad tied to several chains displays “Multi“ for its name, and its mute, solo and preview buttons act on every chain it covers. Mute and solo chains one by one in the chain list and the pad’s icons show that mixed condition. For a Multi pad, Hot-Swap and renaming are switched off, although you can wipe out all of its chains together.

While Pad View was built for painless editing and sound design, it’s equally strong as a live-performance surface, especially when you’re driving it from a hardware control surface that has pads. Should your pad controller be one of Live’s [natively supported control surfaces](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#natively-supported-control-surfaces), just choose it as a control surface over in the Link, Tempo & MIDI tab of Live’s Settings. After that, provided a Drum Rack sits on a track taking in MIDI, your pad controller will fire whichever pads are on screen. Scroll the pad overview to a different bank of pads and your controller keeps pace automatically.

### 24.7 Using the Macro Controls

A Rack can hold as many as 16 Macro Controls. Whenever you make a new Rack, eight Macro Control knobs appear by default. The and view selector buttons let you raise or lower how many Macro Controls are on view. Keep in mind that which Macro Controls are shown versus hidden gets stored in the Live Set.

These Selector Buttons Set the Number of Visible Macro Controls.

### 24.7.1 Map Mode

Making Macro Control Assignments in Map Mode.

Given how intricate device chains can get, Macro Controls hold the complexity in check by assuming command of a Rack’s most important parameters (the ones you’ve picked, naturally). After you’ve dialed in the mapping you want, everything else in the Rack can be put out of sight.

It’s the Map button, dedicated to the Macro Control view, that unlocks this behavior. Switching on Macro Map Mode brings about three results:
