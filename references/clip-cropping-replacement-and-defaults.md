# Clip Cropping Replacement And Defaults

Open when you need guidance on Clip Cropping Replacement And Defaults in Ableton Live.

Context: [Clip View](clip-view.md#8-clip-view).

<a id="source-811-cropping-clips"></a>
### 8.11 Cropping Clips

Cropping a clip lets you hold onto just the portions you care about and discard whatever you don't need. Maybe you only want a brief slice of a longer sample inside an audio clip, or you'd rather drop a few of the MIDI notes you [captured](https://www.ableton.com/en/live-manual/12/recording-new-clips/#capturing-midi).

For unlooped audio clips, the start and end marker let you mark out a region to crop. From there, the Crop Clip Sample command in the Sample Editor’s context menu spawns a fresh, trimmed sample running no longer than the stretch between those two markers. With looped clips, the crop region opens at whichever comes earlier — the start marker or the loop start marker — and closes at the loop end marker.

There's also the Crop Clip Sample to Time Selection command for cropping the sample down to the current time selection; it shows up in the context menu any time you've made a time selection inside the clip.

Much like the Reverse function does, cropping a sample produces a new sample by storing a slice of the longer one. Once you've saved the Live Set, that new sample turns up in the Set’s Project folder beneath Samples/Processed/Crop. Before the Set is saved, though, the new sample sits wherever the Temporary Folder points.

You can fire off either the Crop Clip Sample or the Crop Clip Sample to Time Selection command using the Ctrl+Shift+J (Win) / Cmd+Shift+J (Mac) keyboard shortcut.

Cropping MIDI clips proceeds just as it does for audio clips, aside from slightly different command names: Crop Clip handles cropping to the span between start and end marker (with unlooped clips) or, in a looped clip, between the start/loop start marker and the loop end marker. Meanwhile, cropping down to a time selection falls to the Crop Clip to Time Selection command.

<a id="source-812-replacing-and-editing-the-sample"></a>
### 8.12 Replacing and Editing the Sample

Swapping the clip's referenced sample for another one is as simple as dragging the replacement straight out of the browser onto the Clip View. As an alternative, highlight a sample in the browser and either double-click it or hit Enter to drop that sample onto whichever clip is currently selected.

Performing this swap preserves clip settings such as pitch and volume. As for the Warp Markers, they survive only when the incoming sample matches the outgoing one's length precisely.

To hunt down samples that are [similar](https://www.ableton.com/en/live-manual/12/live-concepts/#sound-similarity) to the one loaded now, choose the Show Similar Files command from the Sample Editor’s context menu.

That same context menu carries a Manage Sample File command too. Choosing it launches the File Manager for the active Set, with the [sample referenced](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#viewing-and-changing-a-live-sets-file-references) by the chosen clip already selected. From there you're free to swap the sample out or edit it destructively — changes that ripple through to every clip and instrument that points at it.

<a id="source-813-editing-clip-properties-for-multiple-clips"></a>
### 8.13 Editing Clip Properties for Multiple Clips

It's possible to adjust the Clip View properties across several clips in one go. Building a multi-clip selection means dragging out from an empty clip slot to sweep up the clips, or picking a single clip and then tacking on more with the Ctrl (Win) / Cmd (Mac) or Shift modifiers. Whichever Clip View properties show up for such a selection hinge on what the clips hold; as a rule, only the properties the clips share appear.

Sliders, knobs, and the like respond a touch differently once several clips are in play. Where the selected clips carry mismatched values for some parameter — clip transposition, say — the control surfaces that spread of values and lets you tweak it. Push the knob or slider hard to its top or bottom limit and the clips’ settings all snap into alignment from then on, moving together as one value.

<a id="source-814-clip-defaults-and-update-rate"></a>
### 8.14 Clip Defaults and Update Rate

How quickly Live pushes your Clip View settings onto a clip that's already playing is adjustable. Edits in the Clip View get quantized to whatever rate you've picked from the Clip Update Rate chooser inside the Record, Warp & Launch Settings. A handful of clip settings — Launch Mode and Warp Mode among them — can be established as defaults that every new clip inherits, which is likewise handled in the Record, Warp & Launch Settings.

The Record, Warp, and Launch Options in Live’s Settings.
