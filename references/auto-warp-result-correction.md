# Auto Warp Result Correction

Open when you need guidance on Auto Warp Result Correction in Ableton Live.

Context: [Auto-Warping Long Samples](audio-clips-tempo-and-warping.md#925-auto-warping-long-samples).

<a id="source-9251-adjusting-auto-warp-results"></a>
#### 9.2.5.1 Adjusting Auto-Warp Results

More often than not, the [Auto-Warp algorithm](https://help.ableton.com/hc/en-us/articles/9230108251164) nails the audio clip's tempo, so it falls neatly in step with the Set's tempo. Still, when the auto-warped outcome isn't what you had in mind, you can refine it by hand.

While reworking Warp Markers on longer samples, it helps to switch on the metronome in the Control Bar so you have a constant tempo reference.

The Metronome Switch.

There are times when Auto-Warp lands the tempo but misses the downbeat. Any of these approaches will set it straight:

- Hold Shift and drag from a Warp Marker to shift where the waveform sits beneath that marker.
- Drag the insert marker onto the downbeat, then invoke the context menu's _Set 1.1.1 Here_ command to relocate the start marker there.
- Zoom in, drop a Warp Marker on the downbeat, and then pull that marker to the start of the timeline's first bar.
  Dragging a Warp Marker to Set the Start Position.

For a sample already trimmed for gapless looping, refining the Auto-Warp outcome is easy via the _Warp Sample as…_ command found in the Sample Editor's context menu. That command offers up a suggested loop length suited to the Set's tempo.

The Warp Sample As… Context Menu Option.

Auto-Warp can be aimed at just one part of a sample as well — pulling and warping a breakbeat out of a longer track, for instance. Do this by dragging across the slice of the sample you want to single out to make a time selection in the Sample Editor. Then call the _Warp Selection as…_ command from the context menu. Auto-Warp settles on what it figures is the best-fitting loop length, drops matching start and end loop markers, and warps the selection so it fills that loop.

Warping a Chosen Portion of a Sample.

Some samples call for tighter command over the Auto-Warp outcome. The surest route there is to warp the audio piece by piece, moving from left to right. Pinning Warp Markers at the start and end of each well-warped stretch holds it in place. [Various shortcuts](https://www.ableton.com/en/live-manual/12/live-keyboard-shortcuts/#clip-view-sample-editor) for the Sample Editor can speed this along — for example, holding the Ctrl (Win) / Cmd (Mac) modifier lets you grab several Warp Markers and shift them as a group.

The Sample Editor's context menu carries a set of _Warp From Here…_ commands, each offering a different way to reset Warp Markers lying to the right of a grid division or Warp Marker while leaving everything to the left alone. You can fire these off anywhere along the timeline, the start marker included.

- _Warp From Here_ applies the Auto-Warp algorithm to the audio sitting right of the selected marker. With no marker selected, one gets dropped at the chosen point on the grid.
- _Warp From Here (Start At …)_ takes the Set's tempo as the reference for auto-warping. To first bring the Set's tempo in line with the clip's BPM, turn warping off for the clip so it plays at its native speed. Next, tap the [Tap Tempo](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#tapping-the-tempo) button in the Control Bar to match the clip's tempo to the Set. Once that's set, switch warping back on for the clip and run the Warp From Here (Start At …) command so your tapped tempo becomes the reference.
- _Warp From Here (Straight)_ is the right pick for samples with no tempo drift. One lone Warp Marker gets placed at the starting point, derived from the sample's estimated original BPM.
- _Warp … BPM From Here_ likewise drops a single Warp Marker at the starting point, but here the clip is treated as sharing the Set's tempo. It's handy when you already know the sample's exact BPM and can enter it into the Control Bar's tempo field ahead of warping.
