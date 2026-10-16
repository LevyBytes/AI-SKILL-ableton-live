# Arrangement Time Splitting And Consolidation

Open when you need guidance on Arrangement Time Splitting And Consolidation in Ableton Live.

Context: [Arrangement View](arrangement-view.md#6-arrangement-view).

<a id="source-611-using-the-time-commands"></a>
### 6.11 Using the …Time Commands

The ordinary commands — Cut, Copy and Paste — touch only whatever you have selected, but their “… Time“ relatives reach across every track, adding or pulling out time as a whole. Put differently, inserting time pushes the chosen span into all tracks of the Arrangement at once, and taking time away strips that span from all tracks alike. Any time signature markers sitting inside the chosen region get shifted along too.

- _Cut Time_ removes a stretch of time from the Arrangement, so that audio or MIDI clips flanking the removed gap slide nearer one another along the timeline. As a result, your Arrangement shrinks by exactly the span you took out.
  On the left, the span of time marked for removal; on the right, how things look once Cut Time has run.
- _Paste Time_ drops previously copied time back into the Arrangement, stretching its total runtime by however much you had copied.
- _Duplicate Time_ lays a duplicate of the chosen span into the Arrangement, lengthening the overall runtime by the size of that selection.
- _Delete Time_ clears a stretch of time out of the Arrangement, drawing the audio or MIDI clips on each side of the cleared gap closer together along the timeline. Doing so trims your Arrangement by the span you erased.
- _Insert Silence_ drops a span of blank time of your choosing into the Arrangement, beginning right at the insert marker.

<a id="source-612-splitting-clips"></a>
### 6.12 Splitting Clips

The Split command carves a clip up into separate pieces, which comes in handy when you want to peel a particular region of a clip off into its own standalone clip, or chop a single clip down into several pieces.

Click at any point across a clip’s waveform or MIDI display, then reach for the shortcut Ctrl+E (Win) / Cmd+E (Mac) or the Split entry in the context menu to break the clip apart at that spot. Each piece that results carries its own clip edges and behaves exactly like any other clip when you move or edit it.

Alternatively, single out a particular stretch inside a clip by dragging across the region you want on the clip’s waveform or MIDI display, then applying the same shortcut or context menu entry to lift that selection out into a clip of its own.

The Result of Splitting a Clip.

<a id="source-613-consolidating-clips"></a>
### 6.13 Consolidating Clips

The Consolidate command fuses chosen content drawn from several neighboring clips into a single fresh clip. You can aim it at clips within one track, or at neighboring clips spanning multiple tracks of the Arrangement. Reaching for Consolidate is a handy way to merge content from a handful of clips into a brand-new loop.

Say you have gathered a batch of clips that play nicely in [Arrangement Loop mode](https://www.ableton.com/en/live-manual/12/arrangement-view/#the-arrangement-loop) and you would like them welded into a single loop — pick out the clips you want, then invoke Consolidate either from the Edit menu, from the main lane context menu, or by way of the shortcut Ctrl+J (Win) / Cmd+J (Mac).

The Result of Consolidating Clips.

From here on the consolidated clip behaves just like any other clip; you might, say, shift it to a fresh spot in the Arrangement, or pull on MIDI clip edges to spin out additional repetitions.

Consolidating audio clips spawns a brand-new sample for each track caught in the selection. Think of those samples as captures of what the time-warping engine puts out, recorded before the track’s effects chain and mixer get a chance to act on it. As a result, the samples carry over the influence of in-clip attenuation, time-warping and pitch shifting, plus the matching [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) — yet the effects themselves are left out. Should you want a sample taken from the post-effects signal instead, reach for the [Export Audio/Video command](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video) and render a chosen group of clips down into a single audio file.

Samples produced by consolidation live inside the active Set’s Project folder, beneath Samples/Processed/Consolidate. Where the Set remains unsaved, those samples instead sit wherever the [Temporary Folder](https://www.ableton.com/en/live-manual/12/recording-new-clips/#where-are-the-recorded-samples) points.

<a id="source-614-linked-track-editing"></a>
### 6.14 Linked-Track Editing

With linked-track editing in play, the [comping workflow](https://www.ableton.com/en/live-manual/12/comping/#comping) along with other phase-locked editing moves can be carried out across several tracks together.
