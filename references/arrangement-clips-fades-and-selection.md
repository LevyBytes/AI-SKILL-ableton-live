# Arrangement Clips Fades And Selection

Open when you need guidance on Arrangement Clips Fades And Selection in Ableton Live.

Context: [Arrangement View](arrangement-view.md#6-arrangement-view).

<a id="source-67-moving-and-resizing-clips"></a>
### 6.7 Moving and Resizing Clips

Within the Arrangement View, a chunk of [audio](https://www.ableton.com/en/live-manual/12/live-concepts/#audio-clips-and-samples) or [MIDI](https://www.ableton.com/en/live-manual/12/live-concepts/#midi-clips-and-midi-files) shows up as a clip placed at a particular song position on one of Live’s tracks.

Drag a clip and it relocates to a different song position or a different track.

Moving a Clip.

Pull on a clip’s left or right edge and its length changes.

Changing a Clip’s Length.

Bear in mind that only the clip bar responds to dragging; you cannot drag from the clip’s waveform or MIDI display.

Clips latch onto the editing grid plus assorted objects across the Arrangement, among them other clips’ edges, locators, and time signature changes.

Inside either a warped audio clip or a MIDI clip, you can slide the material around within the clip’s edges: hold Ctrl+Shift (Win) / Shift+Option (Mac) as you drag the clip’s waveform or MIDI display. To skip grid snapping, keep Ctrl+Alt+Shift (Win) / Cmd+Option+Shift (Mac) held down while dragging the clip’s contents.

<a id="source-68-audio-clip-fades-and-crossfades"></a>
### 6.8 Audio Clip Fades and Crossfades

In the Arrangement View, the head and tail of audio clips carry volume fades you can tune. On top of that, neighboring clips sharing an audio track may be _crossfaded_.

You will find fade controls at the edges of audio clips, so long as the track is tall enough to reveal the fade handles. Where a track is folded or too short, raise its height until those handles show up.

Hovering over an audio clip brings up the fade handles, which start out as little squares at the clip’s corners.

Fade Handles in an Audio Clip.

When [Automation Mode](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) is on, holding the F key as you hover over an automation lane briefly surfaces the fade controls.

With the Fade In Start and Fade Out End handles, you reshape how long a fade in or fade out lasts while leaving the fade peaks alone. Even so, a fade edge cannot pass beyond its fade peak. Grab one of these handles and drag it across the clip to resize the fade. The fade’s steepness is further tunable through the Fade Curve handle, which bends the fade’s curve.

Adjusted Fades in a Clip.

A fade’s length can also be fixed by [selecting a range of time within the clip](https://www.ableton.com/en/live-manual/12/arrangement-view/#selecting-clips-and-time) covering the clip’s head or tail, then running the Create Fade In/Out command in the Create menu or pressing Ctrl+Alt+F (Win) / Cmd+Option+F (Mac).

Neighboring audio clips can be crossfaded. Building and tweaking crossfades resembles building and tweaking start and end fades:

- Drag a fade handle past the neighboring clip’s edge to form a crossfade.
- Drag the slope handle to reshape the crossfade’s curve.
- Highlight a span of time crossing the seam between the two clips, then run the Create Crossfade command from the Create menu.
  Crossfaded Clips.

Picking a fade handle and hitting the Delete key erases the fade — unless the Create Fades on Clip Edges option is switched on under the Record, Warp & Launch Settings. In that situation, Delete snaps the fade handle back to a default 4 ms length. Such default fades guard against pops or clicks at the clip edges.

Automatically Create Short Fades At Clip Edges.

Switching on the Create Fades on Clip Edges option has a further effect: neighboring audio clips pick up automatic 4 ms crossfades. From there they are editable exactly like crossfades you made by hand.

A few caps apply to how long fades and crossfades can be:

- A fade cannot reach across a clip’s loop boundaries.
- A clip’s start fade and end fade are not allowed to overlap.

Once a fade handle is selected, a dotted black line shows on the clip to mark that handle’s limit. This proves handy when working on crossfades, since one clip’s loop boundary can be tucked under the other clip.

Bear in mind that fades belong to the clips themselves rather than the tracks holding them, and they stand apart from [automation envelopes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#automation-and-editing-envelopes).

<a id="source-69-selecting-clips-and-time"></a>
### 6.9 Selecting Clips and Time

Beyond shifting and resizing clips, editing the Arrangement runs on selections: you pick something out, then run a command on that pick (Cut, Copy, Paste, Duplicate, for example).

Selection behaves as follows:

- A click on a clip selects that clip.
- A click on the empty Arrangement background marks a moment in time, drawn as a blinking insert marker. From there, the left and right arrow keys walk the insert marker along time, while the up and down arrow keys carry it between tracks. Holding Ctrl (Win) / Option (Mac) as you press the left and right arrow keys jumps the insert marker to locators and to clip edges within the chosen track or tracks.
- A click-and-drag picks out a timespan.
- To get at the time inside a clip for editing, open up its track by clicking the button beside the track name. Bear in mind selected tracks also open up via the U key. The unfolded track’s height is adjustable by dragging the split line beneath the Unfold Track button, or through the Alt++ (Win) / Option++ (Mac) and Alt+- (Win) / Option+- (Mac) shortcut keys. Track height can likewise be changed by holding Alt (Win) / Option (Mac) and pinching on a supported trackpad or touchscreen. To resize every track in the Arrangement View together, hold Alt (Win) / Option (Mac) as you resize a single one. You can also open up all tracks in one move by holding the Alt (Win) / Option (Mac) modifier while clicking the button, or with the Alt+U (Win) / Option+U (Mac) shortcut.
  Adjusting an Unfolded Track’s Height.
- Dragging through the clip’s waveform or MIDI display lets you select time inside the clip.
- A click on the loop brace acts as a shortcut for the Edit menu’s Select Loop command, picking out everything inside the loop.
- Holding Shift while you click widens an existing selection within the same track or over several tracks. You may also hold Shift and use the arrow keys to grow or shrink the selection.
- Hitting the 0 key switches off a selection of material, even one spanning several clips. Bear in mind that pressing 0 while a track header is selected switches that track off.
- A selection of audio material can be [reversed](https://www.ableton.com/en/live-manual/12/clip-view/#reversing-samples), even across several audio clips. For this, highlight the time span you wish to reverse, then pick the Reverse Clip(s) command from the clip’s context menu or tap the R shortcut key. Bear in mind a selection holding MIDI clips cannot be reversed.
- A selection of material can be nudged with the left and right arrow keys.
