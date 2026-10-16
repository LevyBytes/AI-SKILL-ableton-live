# Drum Rack Pad View

Open when you need guidance on Drum Rack Pad View in Ableton Live.

Context: [Drum Racks](instrument-drum-and-effect-racks.md#246-drum-racks).

<a id="source-2461-pad-view"></a>
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
