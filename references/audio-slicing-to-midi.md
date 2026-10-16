# Audio Slicing To MIDI

Open when you need guidance on Audio Slicing To MIDI in Ableton Live.

Context: [Converting Audio to MIDI](mpe-and-audio-midi-routes.md#13-converting-audio-to-midi).

<a id="source-131-slice-to-new-midi-track"></a>
### 13.1 Slice to New MIDI Track

This command breaks the audio into chunks, each mapped to an individual MIDI note. Slicing isn't like the Convert commands further down, because it never examines the _musical_ context of your source audio. Rather, it merely cuts the source audio into stretches of time without regard to what they contain. The [Drum Rack](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#drum-racks) makes an excellent home for sliced files, and the bulk of the configuration occurs on its own once you settle a few options:

The Slicing Dialog.

Choosing Slice to New MIDI track brings up a dialog box. It presents a list of slicing divisions plus a chooser for picking the Slicing Preset. With the top chooser you can slice across an assortment of beat resolutions, or based on the clip’s transients or Warp Markers. Because a Rack holds no more than 128 chains, Live blocks you from continuing whenever your selection would yield over 128 slices. The remedy is to drop to a coarser slice resolution or to slice a narrower stretch of the clip.

A handful of Ableton-supplied slicing templates sit in the Slicing Preset chooser, alongside any you've created yourself and stored in your User Library’s [default presets folder](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#default-presets).

When “Preserve warped timing” is on, the clip gets sliced so that any timing shifts produced by warping carry over. Turn that option off and the warping-driven changes won't show up in the sliced clip; instead the sliced result plays back like the original, “raw” audio.

After you've set your slicing options and pressed OK, several things take place:

1. A new MIDI track gets built, holding a MIDI clip. That clip carries one note per slice, laid out in a chromatic sequence.
2. A Drum Rack joins the freshly made track, with a single chain for each slice. Every chain is fired by one of the clip's notes and holds a Simpler loaded with its matching audio slice.
3. The Drum Rack’s Macro Controls arrive pre-mapped to handy parameters on the Simplers, governed by whatever the chosen slicing preset specifies. Within the factory Slicing presets, those cover basic envelope controls plus parameters that tweak each slice's loop and crossfade properties. Turning one Macro Control adjusts the linked parameter across all the Simplers at the same time.

Note: Live needs a brief moment to crunch through all of this data.

When you play the MIDI clip, it fires each Drum Rack chain in sequence, following the timing you set or the timing baked into the audio. That opens the door to plenty of fresh editing options, such as:
