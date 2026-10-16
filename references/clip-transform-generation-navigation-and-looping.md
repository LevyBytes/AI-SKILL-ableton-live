# Clip Transform Generation Navigation And Looping

Open when you need guidance on Clip Transform Generation Navigation And Looping in Ableton Live.

Context: [Clip View](clip-view.md#8-clip-view).

<a id="source-86-transform-and-generate-panels"></a>
### 8.6 Transform and Generate Panels

A range of utilities for reshaping a clip's content lives inside the Transform and Generate panels.

With audio clips, the [Quantize tool](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#quantizing-audio) is housed in the Transform panel. On a warped clip, this tool lets you quantize the sample to either the grid size in force or some specific meter value you name. Through the Amount control you decide what percentage of that quantization figure governs how far Warp Markers get shifted.

Quantization Options for an Audio Clip.

Keep in mind that audio clips don't come with a Generate panel.

For MIDI Clips, the Transform and Generate panels hold an assortment of [MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#midi-tools) — utilities meant to support your composing, giving you ways to sculpt MIDI material by transforming or generating notes or MPE data.

A transformation tool operates on the selected notes, the notes within a time selection, or every note in the clip. As soon as you apply one, transformed notes take the place of the originals. With [Scale Mode](https://www.ableton.com/en/live-manual/12/clip-view/#clip-scale) switched on, the tool's pitch controls count in scale degrees rather than semitones.

Thanks to generative tools, you can rapidly introduce fresh material as Live builds note patterns automatically inside MIDI clips. The notes land either across the time selection range or across the clip loop range. Once Scale Mode is active, the pitches of generated notes stay locked within the chosen scale.

For the specifics on each transformation and generative tool that Live offers, turn to the [MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#midi-tools) chapter.

<a id="source-87-zooming-and-scrolling-in-the-clip-views-editor"></a>
### 8.7 Zooming and Scrolling in the Clip View’s Editor

Within the Sample Editor or the MIDI Note Editor, zooming and scrolling behave largely the same as they do over in the [Arrangement View](https://www.ableton.com/en/live-manual/12/arrangement-view/#navigation-and-zooming).

Drag up and down inside the time ruler to fluidly adjust how far you're zoomed, and drag side to side to scroll what's shown. Scrolling via the mousewheel or trackpad works too.

Want to zoom all the way into the current time selection? Hit Z, or invoke the View menu’s Zoom to Clip Selection command. Pressing the X key takes you back to where the zoom was before. Bear in mind that if you've zoomed in several times with the Z key, each press of the X key walks you back one of those steps.

Extra zooming and scrolling lives in the Clip View Selector, which forever displays the whole clip from beginning to end. Whatever portion is on screen right now is marked by the black rectangular outline. Click inside that outline and drag it either way — horizontally or vertically — to scroll or zoom.

The Clip View Selector Zoomed In.

If you'd like the editor to track the play position and scroll on its own, switch on the Follow toggle or pick the Follow command in the Options menu. Making an edit inside the Sample Editor/MIDI Note Editor pauses Follow. It resumes the moment you halt or restart playback, or click somewhere in the Arrangement or clip scrub area.

The Follow Toggle.

<a id="source-88-playing-and-scrubbing-clips"></a>
### 8.8 Playing and Scrubbing Clips

Which stretch of the clip sounds once you launch it is determined by the clip’s [region and loop controls](https://www.ableton.com/en/live-manual/12/clip-view/#clip-and-loop-region-settings). A clip that isn't looped runs from its start marker through to its end marker, or carries on until you stop it.

The Clip Start and End Markers.

You can grab these markers and drag them to fresh spots within the Sample Editor/MIDI Note Editor, or nudge them along with the left and right arrow keys. Shifting the clip region as a whole — that is, both markers together — means selecting one marker, holding Alt (Win) / Option (Mac), and pressing the arrow keys.

With Permanent Scrub Areas turned on under Live’s Display & Input Settings, a click in the bottom portion of the waveform, or in the scrub area beneath the time ruler, sends clip playback leaping straight to that spot.

The Clip Scrub Areas.

How big that leap is gets quantized according to the global quantization setting, which you can change in a hurry through the Ctrl+6, 7, 8, 9, and 0 (Win) / Cmd+6, 7, 8, 9, and 0 (Mac) shortcuts. Holding the left mouse button over the scrub area replays a chunk of the clip sized to your chosen quantization setting, over and over. Pick a small quantization setting — or “None“ — and you can effectively scrub across the music. Switch on the Options menu’s Chase MIDI Notes command and MIDI notes will still sound even when playback kicks off past where the MIDI note begins.

Should the Permanent Scrub Areas preference be turned off, scrubbing remains possible by Shift-clicking anywhere across the scrub area or along the beat-time ruler.

<a id="source-89-looping-clips"></a>
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

<a id="source-810-clip-view-sample-details"></a>
### 8.10 Clip View Sample Details

With audio clips loaded, the Sample Editor header shows the loaded sample's name together with its sample rate, bit depth, and channel count.

The Sample Properties in the Sample Editor Header.

Select more than one audio clip and the sample properties for every sample appear. Wherever a value differs across the samples, an asterisk stands in for it. The header also reports how many samples you've selected in total.

Click a sample’s name in Clip View and that sample file opens up in the browser. The Show in Browser command, found in the Sample Editor’s context menu, likewise surfaces the file there.
