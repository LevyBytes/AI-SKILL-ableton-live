# Loop Length And Multiclip Warping

Open when you need guidance on Loop Length And Multiclip Warping in Ableton Live.

Context: [Warping Short Samples](audio-clips-tempo-and-warping.md#924-warping-short-samples).

<a id="source-9241-even-length-loops"></a>
#### 9.2.4.1 Even-Length Loops

On import, Live presumes a sample holds a cleanly trimmed musical loop running 1, 2, 4, 8, or 16 bars, and it sets the tempo to suit. Two Warp Markers are also generated: one anchored to the sample's beginning and one to its end.

A Four-Bar Loop Shown in the Sample Editor.

You will find the sample's guessed tempo displayed in the BPM field of the Audio Utilities panel. When the exact BPM is known to you, type it straight into the field. When you're uncertain of the precise tempo, hold Shift while dragging the slider to nudge the BPM in small steps. Holding Shift and dragging from the clip's edge in Arrangement View likewise stretches or squeezes the clip's tempo.

The BPM Field Within the Audio Utilities Panel.

Now and then the original tempo gets estimated wrong, and the BPM field reports a value that runs either double-speed or half-speed. Setting it right is a matter of the ×2 and ÷2 buttons, which double or halve the tempo in turn.

<a id="source-9242-odd-length-loops"></a>
#### 9.2.4.2 Odd-Length Loops

A sample whose bar count is odd ends up out of sync, because Live starts off presuming an even bar count thanks to the standard 4/4 time signature setting.

To get playback in sync, the Warp Marker at the sample's end has to sit on the downbeat of an even bar — bar eight in a nine-bar loop, say. Correcting it is just a matter of dropping a marker onto the right bar.

Live can also misjudge some odd-bar loops as being longer or shorter than they really are; a nine-bar loop, for example, might be read as an eight-bar loop. Should that happen, the final bar may stay hidden at first. The remedy is to drag the Warp Marker at the sample's end rightward until the eighth bar comes into view.

<a id="source-9243-uneven-length-loops"></a>
#### 9.2.4.3 Uneven-Length Loops

Samples that were never trimmed for gapless looping, or that lack a clear beat pattern, will likewise drift out of sync.

The fix is to drag the insert marker onto the first downbeat of the sample, then choose the _Set 1.1.1 Here_ context menu option to drop a Warp Marker right there.

Use the Set 1.1.1 Here Command to Drop the First Warp Marker.

With that first Warp Marker in place, you can move on to the _Warp From Here_ context menu option. To clear away leftover silence at the loop's tail, set a Warp Marker just ahead of the sample's silent stretch.

<a id="source-9244-multi-clip-warping"></a>
#### 9.2.4.4 Multi-Clip Warping

Select several clips of identical length and then add or tweak Warp Markers on any one of them, and those edits roll out to every selected clip at once. This proves especially handy when a group of clips shares the same rhythm and you want their timing reworked together — for instance, when you've recorded a multitrack performance and need to fix timing problems across all the tracks.
