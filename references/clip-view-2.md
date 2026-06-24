# Clip View (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Running a sample through the Hi-Q algorithm yields lower distortion — most noticeably in the upper frequency range — whenever you transpose it or reconcile an imported file’s sampling rate with the rate your system uses. While this mode is active, you can shift a sample by about 19 semitones up or down before audible aliasing tends to creep in.

### 8.4.7 Clip Gain and Pitch

Over on the right side of the Audio Utilities panel sit the clip gain and pitch controls.

The Clip Gain and Pitch Controls.

Measured in dB, the Gain slider adjusts how loud the clip plays.

Select several audio clips that hold different Gain values, and the slider presents that spread of values through split triangle handles.

Use the Pitch control to move the clip’s pitch up or down in semitones. You can also dial in this figure through the value field tucked beneath the knob on its left. Just to the right of that semitone field sits a second value field for fine-tuning in cents (where 100 cents equals a single semitone).

### 8.5 Pitch and Time Utilities Panel

Within the Pitch and Time Utilities panel you'll find tools for rapidly reshaping the MIDI notes that live in a clip. These pitch and time tools act on whichever notes or time range you've highlighted. Should you have nothing highlighted, edits made through the button controls reach across the entire clip.

The Pitch and Time Utilities Panel.

The [Editing MIDI](https://www.ableton.com/en/live-manual/12/editing-midi/#editing-midi) chapter covers MIDI editing in greater depth.

### 8.5.1 Pitch Tools

The Pitch Tools.

Your selection gets transposed by the Transpose slider. Enter a number to shift things by semitones, or by scale degrees when a clip scale is running.

What the Fit to Scale button does is nudge the selection's pitches until they line up with the clip’s scale. Without an active scale on the clip, this toggle stays grayed out.

Press the Invert button and the selection turns “upside-down,” trading the topmost note for the bottommost one.

By how many semitones — or scale degrees, when a clip scale is on — fresh notes will sit away from the pitches of your original note selection is governed by the Interval Size slider. Pressing the Add Interval button drops in new notes spaced by whatever the slider specifies.

### 8.5.2 Time Tools

The Time Tools.

Turning the Stretch knob squeezes or expands how long the chosen notes last; the ×2 and /2 buttons, meanwhile, grow or shrink any of three things — note duration, time selection, or loop region — by a factor of 2.

With the Duration chooser you pick a note length to hand off to the note selection. Then the Set Length button puts the chooser's note length value into effect across that selection.

How much random jitter gets applied to note start times — anywhere up to half a grid division — is dictated by the Humanize Amount slider. Trigger that random variation across the note selection with the Humanize button.

A press of the Reverse button mirrors the selection, so the note pattern's sequence ends up running backwards.

Reach for the Legato button to grow or trim each chosen note until it stretches exactly far enough to touch where the following note starts.

### 8.6 Transform and Generate Panels

A range of utilities for reshaping a clip's content lives inside the Transform and Generate panels.

With audio clips, the [Quantize tool](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#quantizing-audio) is housed in the Transform panel. On a warped clip, this tool lets you quantize the sample to either the grid size in force or some specific meter value you name. Through the Amount control you decide what percentage of that quantization figure governs how far Warp Markers get shifted.

Quantization Options for an Audio Clip.

Keep in mind that audio clips don't come with a Generate panel.

For MIDI Clips, the Transform and Generate panels hold an assortment of [MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#midi-tools) — utilities meant to support your composing, giving you ways to sculpt MIDI material by transforming or generating notes or MPE data.

A transformation tool operates on the selected notes, the notes within a time selection, or every note in the clip. As soon as you apply one, transformed notes take the place of the originals. With [Scale Mode](https://www.ableton.com/en/live-manual/12/clip-view/#clip-scale) switched on, the tool's pitch controls count in scale degrees rather than semitones.

Thanks to generative tools, you can rapidly introduce fresh material as Live builds note patterns automatically inside MIDI clips. The notes land either across the time selection range or across the clip loop range. Once Scale Mode is active, the pitches of generated notes stay locked within the chosen scale.

For the specifics on each transformation and generative tool that Live offers, turn to the [MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#midi-tools) chapter.

### 8.7 Zooming and Scrolling in the Clip View’s Editor

Within the Sample Editor or the MIDI Note Editor, zooming and scrolling behave largely the same as they do over in the [Arrangement View](https://www.ableton.com/en/live-manual/12/arrangement-view/#navigation-and-zooming).

Drag up and down inside the time ruler to fluidly adjust how far you're zoomed, and drag side to side to scroll what's shown. Scrolling via the mousewheel or trackpad works too.

Want to zoom all the way into the current time selection? Hit Z, or invoke the View menu’s Zoom to Clip Selection command. Pressing the X key takes you back to where the zoom was before. Bear in mind that if you've zoomed in several times with the Z key, each press of the X key walks you back one of those steps.

Extra zooming and scrolling lives in the Clip View Selector, which forever displays the whole clip from beginning to end. Whatever portion is on screen right now is marked by the black rectangular outline. Click inside that outline and drag it either way — horizontally or vertically — to scroll or zoom.

The Clip View Selector Zoomed In.

If you'd like the editor to track the play position and scroll on its own, switch on the Follow toggle or pick the Follow command in the Options menu. Making an edit inside the Sample Editor/MIDI Note Editor pauses Follow. It resumes the moment you halt or restart playback, or click somewhere in the Arrangement or clip scrub area.

The Follow Toggle.

### 8.8 Playing and Scrubbing Clips

Which stretch of the clip sounds once you launch it is determined by the clip’s [region and loop controls](https://www.ableton.com/en/live-manual/12/clip-view/#clip-and-loop-region-settings). A clip that isn't looped runs from its start marker through to its end marker, or carries on until you stop it.

The Clip Start and End Markers.

You can grab these markers and drag them to fresh spots within the Sample Editor/MIDI Note Editor, or nudge them along with the left and right arrow keys. Shifting the clip region as a whole — that is, both markers together — means selecting one marker, holding Alt (Win) / Option (Mac), and pressing the arrow keys.

With Permanent Scrub Areas turned on under Live’s Display & Input Settings, a click in the bottom portion of the waveform, or in the scrub area beneath the time ruler, sends clip playback leaping straight to that spot.

The Clip Scrub Areas.

How big that leap is gets quantized according to the global quantization setting, which you can change in a hurry through the Ctrl6, 7, 8, 9, and 0 (Win) / Cmd6, 7, 8, 9, and 0 (Mac) shortcuts. Holding the left mouse button over the scrub area replays a chunk of the clip sized to your chosen quantization setting, over and over. Pick a small quantization setting — or “None“ — and you can effectively scrub across the music. Switch on the Options menu’s Chase MIDI Notes command and MIDI notes will still sound even when playback kicks off past where the MIDI note begins.

Should the Permanent Scrub Areas preference be turned off, scrubbing remains possible by Shift-clicking anywhere across the scrub area or along the beat-time ruler.

### 8.9 Looping Clips

For the clip to repeat as a loop that can run forever, flip on the [the Clip Loop toggle](https://www.ableton.com/en/live-manual/12/clip-view/#clip-and-loop-region-settings). With audio clips, you have to engage the Warp switch first, since the Loop switch stays out of reach and unwarped audio clips can't loop.

Once the Clip Loop toggle is engaged, the clip repeats as a loop laid out by the loop region settings.

Inside the Clip View editor, that loop region appears as the _loop brace_. Grabbing and dragging the loop start and end markers reshapes where the loop brace sits and how long it runs.

The Loop Brace.

Relocating the loop brace is a matter of clicking it and dragging with the mouse. These keyboard shortcuts adjust its position as well:

- The left and right arrow keys bump the loop brace one [current grid setting](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid) to the left or right.
- Pressing the up and down arrow keys jumps the loop brace by increments equal to its own length.
- Holding Ctrl (Win) / Cmd (Mac) alongside the left or right arrow key trims or extends the loop brace by one current grid setting.
- Holding Ctrl (Win) / Cmd (Mac) with the up or down arrow key either doubles the loop length or cuts it in half.

The Edit menu’s Duplicate Loop command lets you instantly copy both the span of the loop and what's inside it. Within MIDI clips, whatever notes sit past the loop get nudged along so their placement relative to the loop's end stays intact.

No matter where the loop brace lands, the clip kicks off at the start marker position, so you're able to arrange the clip to feed into a loop.

Setting the Clip to Run Into a Loop.

### 8.10 Clip View Sample Details

With audio clips loaded, the Sample Editor header shows the loaded sample's name together with its sample rate, bit depth, and channel count.

The Sample Properties in the Sample Editor Header.

Select more than one audio clip and the sample properties for every sample appear. Wherever a value differs across the samples, an asterisk stands in for it. The header also reports how many samples you've selected in total.

Click a sample’s name in Clip View and that sample file opens up in the browser. The Show in Browser command, found in the Sample Editor’s context menu, likewise surfaces the file there.

### 8.11 Cropping Clips

Cropping a clip lets you hold onto just the portions you care about and discard whatever you don't need. Maybe you only want a brief slice of a longer sample inside an audio clip, or you'd rather drop a few of the MIDI notes you [captured](https://www.ableton.com/en/live-manual/12/recording-new-clips/#capturing-midi).

For unlooped audio clips, the start and end marker let you mark out a region to crop. From there, the Crop Clip Sample command in the Sample Editor’s context menu spawns a fresh, trimmed sample running no longer than the stretch between those two markers. With looped clips, the crop region opens at whichever comes earlier — the start marker or the loop start marker — and closes at the loop end marker.

There's also the Crop Clip Sample to Time Selection command for cropping the sample down to the current time selection; it shows up in the context menu any time you've made a time selection inside the clip.

Much like the Reverse function does, cropping a sample produces a new sample by storing a slice of the longer one. Once you've saved the Live Set, that new sample turns up in the Set’s Project folder beneath Samples/Processed/Crop. Before the Set is saved, though, the new sample sits wherever the Temporary Folder points.

You can fire off either the Crop Clip Sample or the Crop Clip Sample to Time Selection command using the CtrlShiftJ (Win) / CmdShiftJ (Mac) keyboard shortcut.

Cropping MIDI clips proceeds just as it does for audio clips, aside from slightly different command names: Crop Clip handles cropping to the span between start and end marker (with unlooped clips) or, in a looped clip, between the start/loop start marker and the loop end marker. Meanwhile, cropping down to a time selection falls to the Crop Clip to Time Selection command.

### 8.12 Replacing and Editing the Sample

Swapping the clip's referenced sample for another one is as simple as dragging the replacement straight out of the browser onto the Clip View. As an alternative, highlight a sample in the browser and either double-click it or hit Enter to drop that sample onto whichever clip is currently selected.

Performing this swap preserves clip settings such as pitch and volume. As for the Warp Markers, they survive only when the incoming sample matches the outgoing one's length precisely.

To hunt down samples that are [similar](https://www.ableton.com/en/live-manual/12/live-concepts/#sound-similarity) to the one loaded now, choose the Show Similar Files command from the Sample Editor’s context menu.

That same context menu carries a Manage Sample File command too. Choosing it launches the File Manager for the active Set, with the [sample referenced](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#viewing-and-changing-a-live-sets-file-references) by the chosen clip already selected. From there you're free to swap the sample out or edit it destructively — changes that ripple through to every clip and instrument that points at it.

### 8.13 Editing Clip Properties for Multiple Clips

It's possible to adjust the Clip View properties across several clips in one go. Building a multi-clip selection means dragging out from an empty clip slot to sweep up the clips, or picking a single clip and then tacking on more with the Ctrl (Win) / Cmd (Mac) or Shift modifiers. Whichever Clip View properties show up for such a selection hinge on what the clips hold; as a rule, only the properties the clips share appear.

Sliders, knobs, and the like respond a touch differently once several clips are in play. Where the selected clips carry mismatched values for some parameter — clip transposition, say — the control surfaces that spread of values and lets you tweak it. Push the knob or slider hard to its top or bottom limit and the clips’ settings all snap into alignment from then on, moving together as one value.

### 8.14 Clip Defaults and Update Rate

How quickly Live pushes your Clip View settings onto a clip that's already playing is adjustable. Edits in the Clip View get quantized to whatever rate you've picked from the Clip Update Rate chooser inside the Record, Warp & Launch Settings. A handful of clip settings — Launch Mode and Warp Mode among them — can be established as defaults that every new clip inherits, which is likewise handled in the Record, Warp & Launch Settings.

The Record, Warp, and Launch Options in Live’s Settings.
