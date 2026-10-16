# Rack Creation Layout And Chain List

Open when you need guidance on Rack Creation Layout And Chain List in Ableton Live.

Context: [Instrument, Drum and Effect Racks](instrument-drum-and-effect-racks.md#24-instrument-drum-and-effect-racks).

<a id="source-242-creating-racks"></a>
### 24.2 Creating Racks

Live’s devices are spanned by four kinds of Rack: Instrument Racks, Drum Racks, Audio Effect Racks and MIDI Effect Racks. Much like the track types, every Rack variety follows its own rules about which devices may live inside it:

- _MIDI Effect Racks_ hold MIDI effects exclusively and are only allowed on MIDI tracks.
- _Audio Effect Racks_ hold audio effects exclusively and belong on audio tracks. They may also sit on MIDI tracks, provided they are “downstream“ from an instrument.
- _Instrument Racks_ hold instruments, yet they may additionally take in both MIDI and audio effects. When they do, every MIDI effect must come first along the Instrument Rack’s device chain, with an instrument next, and any audio effects after that.
- _Drum Racks_ resemble Instrument Racks; they accept instruments together with MIDI and audio effects, and the ordering of those devices obeys the very same signal flow rules. On top of that, Drum Racks may house as many as six return chains of audio effects, each driven by its own send level from the chains in the main Rack.

Racks can be made in more than one way. To spin up a brand-new, empty Rack, drag a generic Rack preset (“_Audio Effect Rack_,“ say) out of the browser and onto a track. From there you can drop devices straight into the Rack’s Chain List or Devices view, both covered in the section that follows.

Suppose a track already holds one or more devices you’d like to bundle into a Rack. In that case, click the title bars of those devices in the Device View, then right-click one of those title bars to bring up the _Group_ and _Group to Drum Rack_ commands in the context menu. Keep in mind that issuing this command once more on the same device produces a Rack nested inside a Rack. The identical method lets you group several chains within a Rack, and that too yields a Rack inside a Rack. Throughout the Device View, a Rack’s contents always sit enclosed by end brackets: much like with punctuation or in mathematics, a Rack lodged within a Rack carries one pair of brackets nested inside another.

When you want to ungroup devices and break apart their Racks, click the _Rack’s_ title bar, then reach for the _Ungroup_ command either via the Edit menu or through the context menu.

<a id="source-243-looking-at-racks"></a>
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

<a id="source-244-chain-list"></a>
### 24.4 Chain List

The Chain List in an Audio Effect Rack.

The moment signals arrive at a Rack, the Chain List is what meets them first. For that reason, we’ll begin our own tour right here too.

For signals coming in, the Chain List is where the split happens: every parallel device chain begins right here as its own listing. Underneath the list sits a drop area into which you can introduce new chains by dragging and dropping presets, devices, or even chains that already exist.

Note: Racks, chains and devices may be dragged in and out of other Racks at will, and even passed from track to track. If you select a chain and then drag while hovering over a different Session or Arrangement View track, that track takes focus; its Device View springs open so you can drop your chain where you want it.

Because the Device View can only display a single device chain at any moment, the Chain List doubles as a way to get around: whatever you pick in the list governs what appears in the neighboring Devices view (when it’s switched on). Give the up and down arrow keys on your computer keyboard a try to shift which entry is selected in the Chain List, and you’ll see how rapidly you can page through everything a Rack holds.

On top of that, the Chain List lets you select multiple chains at once, which makes copying, arranging and regrouping them easy. When you do, the Devices view reports just how many chains you have selected at the moment.

Every chain comes with its own Chain Activator plus Solo and Hot-Swap buttons. Chains living in Instrument, Drum and Audio Effect Racks additionally carry their own volume and pan sliders, while Drum Rack chains throw in extra send level and MIDI assignment controls. Just as with Live Clips, whole chains may be stored and called back up as presets from the browser. To label a chain meaningfully, select it and then pick the Edit menu’s Rename command. You can likewise attach your own info text to a chain through the Edit Info Text command, found in the Edit menu or in the chain’s context menu. That context menu also offers a color palette from which you can assign a custom chain color.
