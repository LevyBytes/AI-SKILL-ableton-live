# Rack Macro Mapping Variations And Mixing

Open when you need guidance on Rack Macro Mapping Variations And Mixing in Ableton Live.

Context: [Using the Macro Controls](instrument-drum-and-effect-racks.md#247-using-the-macro-controls).

<a id="source-2471-map-mode"></a>
### 24.7.1 Map Mode

Making Macro Control Assignments in Map Mode.

Given how intricate device chains can get, Macro Controls hold the complexity in check by assuming command of a Rack’s most important parameters (the ones you’ve picked, naturally). After you’ve dialed in the mapping you want, everything else in the Rack can be put out of sight.

It’s the Map button, dedicated to the Macro Control view, that unlocks this behavior. Switching on Macro Map Mode brings about three results:

- Each parameter on a Rack’s devices that can be mapped is highlighted by a tinted overlay;
- Below every Macro Control dial, a Map button becomes visible;
- The Mapping Browser (see [‘The Mapping Browser’](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#the-mapping-browser)) will open.

Use the procedure below to begin assigning mappings:

1. Turn on Macro Map Mode by pressing the Map mode button;
2. Click a device parameter a single time to choose it for assignment;
3. Assign the parameter by hitting the Map button on whichever Macro Control you want. That entry then shows up in the Mapping Browser. As a default, the Macro Control adopts both the name and the units of the parameter it now governs.
4. Adjust the span of values, if you wish, with the Min/Max sliders found in the Mapping Browser. To produce an inverted mapping, give the Min slider a higher value than the Max slider. You may also flip existing values by right-clicking the relevant Mapping Browser entry and choosing Invert Range.
5. Pick a further device parameter to build additional mappings, or press the Map mode button again to leave Macro Map Mode.

Keep in mind that, after a device parameter is tied to a Macro Control, it shows as greyed out, because it surrenders its control fully to the Macro Control (though external modulation remains possible, for instance through [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes)).

Your assignments may be modified or removed whenever you like through the Mapping Browser, which is only visible while Map Mode is active.

When several parameters share a single Macro Control, that control’s label falls back to its default form (for instance, Macro 3). The Macro Control’s units likewise shift onto a 0 to 127 scale, unless every assigned parameter shares an identical unit type along with an identical unit range.

Through the matching entries in the Edit menu or the context menu, Macro Controls may receive custom names, colors and info text entries.

### 24.7.2 Randomizing Macro Controls

When you’re after a touch of unpredictability, or simply looking to spark a fresh idea in your Set, randomizing Macro Controls is a handy device. Hitting the Rand button on a Rack’s title bar randomizes every mapped Macro Control value within that Rack.

This Button Randomizes Macro Controls.

According to the sounds you’re working with, it may make sense to randomize a handful of parameters and keep the rest as they are. Switch on the Exclude Macro from Randomization option in the context menu to keep a particular mapped Macro Control out of the process. Be aware that, within Instrument Rack presets, any Macro Controls tied to Volume parameters skip randomization automatically.

### 24.7.3 Macro Control Variations

Macro Control Variations.

Distinct configurations of Macro Controls can be saved as separate presets (referred to as “variations”). That comes in handy if, say, you’d like to freeze a Rack’s condition as a “snapshot” mid sound-design session, or compare alternative positions of a mapped Macro Control inside an Audio Effect Rack built for mixing. These variations also lend themselves to crafting builds and drops, or to leaping instantly between assorted Macro Control settings as you record or play live.

Hit the Show/Hide Macro Variations view selector button to reveal a panel for saving, organizing and triggering Macro Control variations.

This Selector Button Opens the Macro Control Variations View.

Hit the New button to save a Rack’s present Macro Controls condition as a fresh variation. Out of the box, every saved variation receives a sequential label such as “Variation 1”, “Variation 2”, and onward. A chosen Macro Control variation may be renamed, duplicated, or removed through commands in the Edit menu or the context menu.

To recall a Macro Control variation in the form it was saved, use the Launch Macro Variation button on the right; to replace it, use the “Overwrite Macro Variation” button on the left. Bear in mind that the Exclude Macro From Variations command in the context menu lets you keep a given Macro Control fixed whenever another Macro Control variation fires. Turning that context menu entry off restores the control’s ability to change.

### 24.8 Mixing With Racks

Whenever an Instrument or Drum Rack holds more than a single chain, it can be displayed and mixed next to the tracks inside the Session View’s mixer. The title bar of a track holding such Racks carries a button that folds the Rack’s mixer open or closed. The same button appears on any chains nested inside the Rack as well. That gives you a quick look at how your Rack is structured — or lets you tuck it away when your focus is purely the mix.

Mixing Rack Chains in the Session View.

Within the Session View mixer, chains resemble tracks but lack clip slots. Because their mixing and routing controls echo those in the Rack’s chain list, an adjustment in one location shows up instantly in the other. In the same way, plenty of chain tasks — reordering, renaming, regrouping and so on — work from either the mixer or the chain list. A click on a chain’s mixer title bar restricts the Device View to that one chain’s devices.

Just as with tracks, multiselecting chains in the Session View mixer means that tweaking a mixer parameter on one chain applies that same change across the other selected chains. Keep in mind this holds only for parameters touched through the Session mixer, not for those same parameters when edited in the Rack’s chain list.

### 24.8.1 Extracting Chains

Every chain may be pulled out of the Rack that holds it and dropped onto different tracks or Racks, working either from the chain list or from the Session View mixer. The return chains of a Drum Rack are extractable too, spawning fresh return tracks when you drag them to the mixer. Drum chains carry an extra trait: dragging one from the mixer onto a new track brings its MIDI notes along. Suppose, for instance, you’re building a MIDI drum loop in one track and decide the snare belongs on a track of its own — just grab the snare chain’s title bar in the mixer and drop it on the mixer’s drop area. The result is a new track holding everything from the snare chain: its devices together with its MIDI data. Should you want the devices alone, drag from the chain list rather than the mixer.

Extracting Drum Chains in the Mixer Extracts MIDI Data.
