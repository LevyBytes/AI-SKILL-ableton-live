# Arrangement View (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

To adjust how wide the grid lines are drawn — for both the zoom-adaptive and the fixed varieties — open the context menu found either in the Arrangement View track main lanes or within the MIDI Note Editor over in the [Clip View](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view).

These keyboard shortcuts, mirrored as entries under the Options menu, let you reshape the grid in a hurry:

- Ctrl1 (Win) / Cmd1 (Mac) _narrows_ the grid, packing twice as many grid lines into the same space (say, shifting from eighth notes down to sixteenth notes).
- Ctrl2 (Win) / Cmd2 (Mac) _widens_ the grid, thinning the grid lines out to half their count (say, moving from eighth notes up to quarter notes).
- Ctrl3 (Win) / Cmd3 (Mac) toggles _triplets_ mode; as an example, that switches the grid from straight eighth notes over to eighth note triplets.
- Ctrl4 (Win) / Cmd4 (Mac) turns grid snapping on or off. With snapping disabled, the cursor stops locking onto meter subdivisions.
- Ctrl5 (Win) / Cmd5 (Mac) toggles fixed and adaptive grid modes.

Whatever distance currently separates one grid line from the next is shown just above the time ruler, over in the lower right corner of the Arrangement View.

Holding the Alt (Win) / Cmd (Mac) modifier as you carry out an action lets you sidestep grid snapping temporarily. And when snapping happens to be off, pressing that same modifier turns it back on for the moment.

### 6.11 Using the …Time Commands

The ordinary commands — Cut, Copy and Paste — touch only whatever you have selected, but their “… Time“ relatives reach across every track, adding or pulling out time as a whole. Put differently, inserting time pushes the chosen span into all tracks of the Arrangement at once, and taking time away strips that span from all tracks alike. Any time signature markers sitting inside the chosen region get shifted along too.

- _Cut Time_ removes a stretch of time from the Arrangement, so that audio or MIDI clips flanking the removed gap slide nearer one another along the timeline. As a result, your Arrangement shrinks by exactly the span you took out.
  On the left, the span of time marked for removal; on the right, how things look once Cut Time has run.
- _Paste Time_ drops previously copied time back into the Arrangement, stretching its total runtime by however much you had copied.
- _Duplicate Time_ lays a duplicate of the chosen span into the Arrangement, lengthening the overall runtime by the size of that selection.
- _Delete Time_ clears a stretch of time out of the Arrangement, drawing the audio or MIDI clips on each side of the cleared gap closer together along the timeline. Doing so trims your Arrangement by the span you erased.
- _Insert Silence_ drops a span of blank time of your choosing into the Arrangement, beginning right at the insert marker.

### 6.12 Splitting Clips

The Split command carves a clip up into separate pieces, which comes in handy when you want to peel a particular region of a clip off into its own standalone clip, or chop a single clip down into several pieces.

Click at any point across a clip’s waveform or MIDI display, then reach for the shortcut CtrlE (Win) / CmdE (Mac) or the Split entry in the context menu to break the clip apart at that spot. Each piece that results carries its own clip edges and behaves exactly like any other clip when you move or edit it.

Alternatively, single out a particular stretch inside a clip by dragging across the region you want on the clip’s waveform or MIDI display, then applying the same shortcut or context menu entry to lift that selection out into a clip of its own.

The Result of Splitting a Clip.

### 6.13 Consolidating Clips

The Consolidate command fuses chosen content drawn from several neighboring clips into a single fresh clip. You can aim it at clips within one track, or at neighboring clips spanning multiple tracks of the Arrangement. Reaching for Consolidate is a handy way to merge content from a handful of clips into a brand-new loop.

Say you have gathered a batch of clips that play nicely in [Arrangement Loop mode](https://www.ableton.com/en/live-manual/12/arrangement-view/#the-arrangement-loop) and you would like them welded into a single loop — pick out the clips you want, then invoke Consolidate either from the Edit menu, from the main lane context menu, or by way of the shortcut CtrlJ (Win) / CmdJ (Mac).

The Result of Consolidating Clips.

From here on the consolidated clip behaves just like any other clip; you might, say, shift it to a fresh spot in the Arrangement, or pull on MIDI clip edges to spin out additional repetitions.

Consolidating audio clips spawns a brand-new sample for each track caught in the selection. Think of those samples as captures of what the time-warping engine puts out, recorded before the track’s effects chain and mixer get a chance to act on it. As a result, the samples carry over the influence of in-clip attenuation, time-warping and pitch shifting, plus the matching [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) — yet the effects themselves are left out. Should you want a sample taken from the post-effects signal instead, reach for the [Export Audio/Video command](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video) and render a chosen group of clips down into a single audio file.

Samples produced by consolidation live inside the active Set’s Project folder, beneath Samples/Processed/Consolidate. Where the Set remains unsaved, those samples instead sit wherever the [Temporary Folder](https://www.ableton.com/en/live-manual/12/recording-new-clips/#where-are-the-recorded-samples) points.

### 6.14 Linked-Track Editing

With linked-track editing in play, the [comping workflow](https://www.ableton.com/en/live-manual/12/comping/#comping) along with other phase-locked editing moves can be carried out across several tracks together.

### 6.14.1 Linking and Unlinking Tracks

To link a set of selected tracks, reach for the Link Tracks command sitting in the track header’s context menu.

The Link Tracks Command.

Tracks living inside a [Group Track](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks) can be linked as well — open the Group Track header’s context menu and choose the Link Tracks command there.

Once linked, tracks show a linked-track indicator button within their track headers.

A Track’s Linked-Track Indicator Button.

Keep in mind that a Set may hold several separate instances of linked tracks, yet any single track is allowed membership in just one of them.

Pause your pointer over a track’s linked-track indicator and the tracks bound together with it light up. That comes in particularly handy when you need to tell apart several instances of linked tracks. Give that indicator a click and every track tied into the same group gets selected.

To fold extra tracks into an instance that already exists, start by selecting the tracks you wish to bring in, then hold Ctrl (Win) / Cmd (Mac) while choosing the Link Tracks command from the context menu of one of the headers already in that linked group.

Whether it is a portion of some linked tracks, or a blend of linked and unlinked ones, you can bind such a grouping by highlighting the relevant track headers and then choosing Link Tracks from the context menu.

When you need to pull tracks back out of a linked instance, select the ones you intend to unlink and pick the Unlink Track(s) option from the track or Group Track header’s context menu.

### 6.14.2 Editing Linked Tracks

After an instance of linked tracks is in place, you can carry out the following operations on every one of its tracks at the same time:

- [Moving and resizing clips](https://www.ableton.com/en/live-manual/12/arrangement-view/#moving-and-resizing-clips).
- [Selecting clips and time](https://www.ableton.com/en/live-manual/12/arrangement-view/#selecting-clips-and-time).
- Using the [“… Time” commands](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-time-commands).
- [Splitting](https://www.ableton.com/en/live-manual/12/arrangement-view/#splitting-clips) and [consolidating clips](https://www.ableton.com/en/live-manual/12/arrangement-view/#consolidating-clips).
- [Creating and editing audio clip fades](https://www.ableton.com/en/live-manual/12/arrangement-view/#audio-clip-fades-and-crossfades). Simultaneous adjustment is limited to fades that share the same starting time position.
- [Arming and disarming tracks](https://www.ableton.com/en/live-manual/12/recording-new-clips/#arming-record-enabling-tracks).
- [Renaming, inserting, and deleting take lanes](https://www.ableton.com/en/live-manual/12/comping/#inserting-and-managing-take-lanes), along with [enabling and disabling Audition Mode](https://www.ableton.com/en/live-manual/12/comping/#auditioning-take-lanes) on take lanes. The same holds true even where take lanes happen to be hidden on some of the linked tracks.

### 6.15 The Mixer in Arrangement View

Arrangement View hands you two distinct groupings of [mixer controls](https://www.ableton.com/en/live-manual/12/mixing/#mixing): the _mixer_ on the one hand and the _Arrangement track controls_ on the other.

The Mixer (Bottom) and Arrangement Track Controls (Right).

Bring up the mixer through the Mixer command under the View menu, or with the shortcut CtrlAltM (Win) / CmdOptionM (Mac). The mixer view control tucked into the bottom right corner of Live’s window lets you toggle it into and out of sight as well.

To decide which controls actually appear in the mixer, head to the Mixer Controls submenu found in the View menu.

The Mixer Controls Submenu.

Likewise, the View menu carries its own submenu that governs whether the various Arrangement track controls stay visible or hidden.

Because the mixer and the Arrangement track controls draw on one shared pool of values and settings, either one serves equally well for adjusting tracks. Bear in mind, though, that a handful of controls live only in the mixer — among them the [Performance Impact indicators](https://www.ableton.com/en/live-manual/12/mixing/#performance-impact-track-indicators), the [track delays](https://www.ableton.com/en/live-manual/12/mixing/#track-delays) and the [crossfader](https://www.ableton.com/en/live-manual/12/mixing/#using-lives-crossfader).
