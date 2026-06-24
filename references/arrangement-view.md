# Arrangement View (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 6. Arrangement View

Among Live’s [two main views](https://www.ableton.com/en/live-manual/12/live-concepts/#arrangement-and-session) for laying out and composing a track, the _Arrangement View_ is one. Where [Session View](https://www.ableton.com/en/live-manual/12/session-view/#session-view) revolves around jamming, looping, and firing off clips, the Arrangement View instead has you assemble and position a song’s various parts along a horizontal timeline. That overall structure of a project or piece carries the name _Arrangement_.

A Song in the Arrangement View.

### 6.1 Layout

The Upper Area of the Arrangement View.

1. Spanning the Arrangement’s full set of clips from beginning to end, the _Overview_ serves for navigating and zooming. A black outline marks whichever portion is on screen at the moment. Horizontal dragging scrolls the view sideways, while vertical dragging zooms it closer or farther. Double-clicking inside that black outline anywhere snaps the zoom back out to the whole Arrangement.
2. The _beat-time ruler_ presents time as bars-beats-sixteenths. Dragging here behaves just like it does in the Overview: pull sideways to scroll along the timeline, or pull up and down to zoom. A double-click on the beat-time ruler zooms onto the active selection. With nothing selected, that same double-click zooms back out to the whole Arrangement.
3. A click at any spot in the _scrub area_ begins [playback](https://www.ableton.com/en/live-manual/12/arrangement-view/#transport-and-playback) right there. Holding the left mouse button at a given spot in the scrub area instead loops that region, governed by the current global launch quantization value.
4. _Locators_ may be dropped at any spot in the scrub area so that you can fire playback from [multiple areas](https://www.ableton.com/en/live-manual/12/arrangement-view/#launching-the-arrangement-with-locators) of the Arrangement. They come in handy for breaking a track into sections you can trigger.
5. The _Set Locator_ button drops locators into the scrub area as you play back or record. Once a locator is selected, that same Set Locator button turns into the Delete Locator button for removing locators.
6. Playback for locators is triggered by the _Previous and Next Locator_ buttons. The leap from one fired locator to the next follows the global launch quantization value.
7. Toggle [automation lanes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) on or off with the _Automation Mode_ control.
8. With the _Lock Envelopes_ toggle, you can pin envelopes to the song position rather than to the clips themselves. That way, shifting clips leaves the automation envelopes where they are.
   Track, Mixer, and Additional Zoom Controls in the Arrangement View.
9. A track’s _main lane_ holds and lines up its clips. While following the [comping workflow](https://www.ableton.com/en/live-manual/12/comping/#comping), clips drawn from the various take lanes can be brought into that main lane.
10. The _Arrangement Track Controls_ expose volume, panning, I/O, and further mixer settings. Which of these appear is configurable through the Arrangement Track Controls submenu under the View menu.
11. Within the Arrangement View, [_tracks_](https://www.ableton.com/en/live-manual/12/live-concepts/#tracks) sit in a vertical stack. To reorder them, select and drag a track above or below its neighbors.
12. Dropping instruments and devices into the _Mixer Drop Area_ below the tracks adds fresh tracks to the Arrangement. An instrument or MIDI effect dropped here spawns a MIDI track, whereas an audio effect spawns an audio track.
13. With the _Optimize Height_ and _Optimize Width_ toggles, every track is sized to fit the Arrangement’s present height or width. The matching keyboard shortcuts are H and W.
14. The _Waveform Vertical Zoom Level_ slider grows the waveform shown inside audio clips. That helps you spot transients and waveform detail while leaving the clip gain untouched. This zoom carries across every audio track in the Arrangement and applies to new clips at the moment they record.
15. The _time ruler_ expresses time as minutes-seconds-milliseconds. Drag within it to scroll the view sideways.
16. The [_mixer_](https://www.ableton.com/en/live-manual/12/mixing/#mixing) can be revealed in Arrangement View through the Mixer entry in the View menu, or with the Mixer View toggle down in the lower right corner of Live’s window.

### 6.2 Navigation and Zooming

Beyond several of the choices laid out in the [Layout section](https://www.ableton.com/en/live-manual/12/arrangement-view/#layout), these further ways of navigating and zooming are on hand as well:

- For gradual zoom in and out centered on the active selection, tap the + and - keys, or roll the mouse wheel or trackpad while holding Ctrl (Win) / Cmd (Mac). Panning the view is done by dragging while you hold the CtrlAlt (Win) / CmdOption (Mac) modifier.
- For a full zoom onto the active selection, hit Z or pick the Zoom to Arrangement Time Selection command from the View menu. Pressing the X key restores the zoom you had before. Bear in mind that after several successive Z zooms, repeated X presses step back through them one level at a time.
- When you select time over a clip in the Arrangement, the Clip View editor will [zoom in](https://www.ableton.com/en/live-manual/12/clip-view/#zooming-and-scrolling-in-the-clip-views-editor) to match that selected time too.
- For vertical zoom on a chosen track, roll the mouse wheel or trackpad inside that track’s main lane while holding the Alt (Win) / Option (Mac) modifier. Keep in mind that with a time selection present in the Arrangement, every track holding selected content zooms vertically.
- So that the Arrangement view trails the song position and scrolls on its own, flip on the _Follow_ switch in the Control Bar, or invoke the Follow command from the Options menu. Follow halts whenever you edit, scroll the Arrangement sideways, or click the beat-time ruler. It resumes once playback stops or restarts, or when you click within the Arrangement or a clip scrub area.
  The Follow Switch in the Control Bar.

### 6.3 Transport and Playback

Playback of the Arrangement is launched by the transport controls sitting in the Control Bar.

A click on the Play button gets playback going; clicking the Stop button halts it. The space bar offers another route, switching playback on and off.

The Play and Stop Buttons in the Control Bar.

You may additionally assign [computer keyboard keys or MIDI messages](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) to those transport controls, giving you a tailored setup for kicking off playback however you like.

Where playback begins is governed by the blinking blue insert marker on a track. Out of the box, that marker sits at the Arrangement’s start. Clicking somewhere inside a track relocates the insert marker, setting a fresh play position. To send the insert marker back to its starting play position, either double-click the Stop button or hit the Home key (Win) or Function + left arrow key (Mac).

Arrangement Playback Begins from the Insert Marker.

If you would rather resume from wherever playback last halted instead of the insert marker, hold Shift as you press the space bar.

You can also reach the play position through the Control Bar’s Arrangement Position fields.

Set the Play Position in the Arrangement Position Fields.

Within the Arrangement Position fields, the play position reads out as bars-beats-sixteenths. With one field selected, its value is editable in several ways: - Drag the mouse up or down to change it. - Key in a number, then hit Enter. - Press the up and down arrow keys to raise or lower it.

Editing the Arrangement Position fields shifts the insert marker right along with it.

The scrub area above the tracks gives you yet another way to begin playback. By default the Permanent Scrub Areas option stays on in Live’s Display & Input Settings, so a click anywhere in the scrub area kicks off playback from that spot.

Use the Scrub Area to Launch Playback.

As you click from one point in the scrub area to another, the leap between fired play positions is quantized by the Quantization Menu’s setting in the Control Bar. Holding the left mouse button at a chosen spot in the scrub area instead repeats a portion of the Arrangement, following the global launch quantization value.

Should the Permanent Scrub Areas option be turned off, you can still scrub the Arrangement by Shift-clicking somewhere in the scrub area or along the beat-time ruler.

The editor in [the Clip View](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view) carries its own per-clip scrub area as well, which can fire playback.

So that MIDI notes still sound when playback begins partway into a note, Live chases MIDI notes by default. That behavior can be switched off or back on through the Chase MIDI Notes command in the Options menu.

### 6.4 Launching the Arrangement with Locators

For several playback-trigger spots throughout the Arrangement, drop launchable locators into the scrub area.

Use Locators to Launch Playback in the Arrangement.

With the Set Locator button you can place locators anywhere in the Arrangement on the fly, whether playing back or recording. Each locator is quantized to the global launch quantization value chosen in the Control Bar.

The Set Locator Button.

Pressing the Set Locator button when the transport is idle drops a locator at the insert marker spot, or at where the time selection begins. Locators can likewise be placed through the Add Locator entry in the scrub area’s context menu or by way of the Create menu.

Keep in mind that once locators exist in the Arrangement, the Set Locator button switches to the Delete Locator button for whichever locators are selected.

Reaching a locator is a matter of clicking it or pressing the Previous and Next Locator buttons sitting beneath the Set button. Once you pass the Arrangement’s first or last locator, those Previous and Next Locator buttons carry you to the Arrangement start or end accordingly.

The Previous and Next Locator Buttons.

[MIDI/key mapping](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) can also fire locators. With the transport halted, a double-click on a locator selects it and sets playback rolling from there.

A selected locator can be relocated by dragging it or pressing the arrow keys. Renaming selected locators happens through the Rename entry in the Edit menu or the CtrlR (Win) / CmdR (Mac) shortcut. You may also attach your own info text notes to locators via the Edit Info Text entry in the Edit menu or the locator’s context menu. Removing a locator is done with the Delete key, the Delete Locator entry under the Create menu, or the Delete Locator button.

A locator’s context menu carries the Loop to Next Locator command, a fast route to [looping playback](https://www.ableton.com/en/live-manual/12/arrangement-view/#the-arrangement-loop) across two locators. The Set Song Start Time Here command overrides the standard “playback starts at selection“ behavior: with it checked, playback fires from the locator rather than the selection.

### 6.5 Time Signature Changes

By means of time signature markers, Live’s time signature is adjustable at any spot along the Arrangement. Dropping a marker at the present insert marker position is done with the Insert Time Signature Change command from the Create menu or the scrub area’s context menu.

A marker accepts any time signature whose numerator is one or two digits and whose denominator is 1, 2, 4, 8 or 16. Those two numbers need a separator between them — a slash, comma, period, or however many spaces.

Time signature values can additionally be typed or nudged through the Time Signature Numerator and Denominator fields in the Control Bar. Doing so alters the time signature at the present play spot, and functions whether the transport is halted or rolling.

Whenever the Arrangement holds time signature changes, an automation LED shows up in the upper left corner of the time signature fields.

The Time Signature Fields.

You will find time signature markers sitting right under the beat-time ruler. Bear in mind this marker strip stays hidden when a Set carries no meter changes.

Time Signature Changes.

Moving time signature markers is done with the mouse or the left and right arrow keys. To edit the values of selected markers, reach for the Edit Time Signature command — found under the Edit menu, inside the scrub area’s context menu, or bound to the CtrlR (Win) / CmdR (Mac) shortcut. Removing a time signature marker calls for the Delete key or the Delete command in the Edit menu.

Time signature markers carry no quantization; you may drop them anywhere along the timeline, with their placement bounded solely by the [editing grid](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid). So meter changes can land in “impossible“ spots — for instance, ahead of the prior measure’s close. That produces a _fragmentary bar_, shown in the scrub area as a crosshatched patch. Live will gladly leave such partial measures untouched, yet should you want your Set to obey music theory, the context menu offers options for “correcting“ those incomplete bars.

A Fragmentary Bar and its Context Menu Options.

_Delete Fragmentary Bar Time_ strips the fragmentary bar’s span out of the Arrangement, drawing whatever audio or MIDI clips flank the removed stretch nearer one another along the timeline. The following time signature marker then lands on the barline you would expect.

_Complete Fragmentary Bar_ adds time at the fragmentary bar’s front, rounding it out to full. The following time signature marker then lands on the barline you would expect.

Do bear in mind that each of these options touches _all_ tracks — removing and adding time alters how long the whole Arrangement runs.

Bringing a [MIDI file](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#midi-files) into the Arrangement offers you the choice to pull in whatever time signature data was stored alongside it. Take that option and Live drops time signature markers into all the right spots on its own. This makes handling intricate music built in other sequencer or notation programs quite painless.

### 6.6 The Arrangement Loop

For looping a stretch of the Arrangement over and over, switch on the _Arrangement Loop_ with its toggle in the Control Bar.

The Arrangement Loop Toggle in the Control Bar.

With no clip(s) or time selected, the loop brace stretches over the whole Arrangement. Its length is settable by number through the _Loop Start_ and _Loop Length_ fields in the Control Bar, which fix the loop’s starting point and its duration respectively.

The Loop Start Fields (Left) and the Loop Length Fields (Right).

The Edit menu’s Loop Selection command switches on the Arrangement loop and snaps the loop brace to the active time selection. Its matching shortcut, CtrlL (Win) / CmdL (Mac), will also flip the Arrangement loop on or off whenever a clip or time is selected.

The Arrangement’s Loop Brace.

These keys and commands adjust the loop brace:

- The left and right arrow keys inch the loop brace one way or the other according to the present [grid settings](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid).
- The up and down arrow keys move the loop brace sideways in increments matching the loop brace length.
- Ctrl (Win) / Cmd (Mac) plus the left and right arrow keys trims or extends the loop by the present grid settings.
- Ctrl (Win) / Cmd (Mac) plus the up and down arrow keys doubles or halves the loop length.

Dragging the loop brace works too: pull on its left or right edge to move the loop’s start/end points, or drag the brace bar sideways to reposition the loop while keeping its length the same.

So that playback fires from the loop brace’s start, head into the brace’s context menu and enable Set Song Start Time Here there. Doing so overrides the standard behavior of starting playback at the insert marker or the live time selection.

### 6.7 Moving and Resizing Clips

Within the Arrangement View, a chunk of [audio](https://www.ableton.com/en/live-manual/12/live-concepts/#audio-clips-and-samples) or [MIDI](https://www.ableton.com/en/live-manual/12/live-concepts/#midi-clips-and-midi-files) shows up as a clip placed at a particular song position on one of Live’s tracks.

Drag a clip and it relocates to a different song position or a different track.

Moving a Clip.

Pull on a clip’s left or right edge and its length changes.

Changing a Clip’s Length.

Bear in mind that only the clip bar responds to dragging; you cannot drag from the clip’s waveform or MIDI display.

Clips latch onto the editing grid plus assorted objects across the Arrangement, among them other clips’ edges, locators, and time signature changes.

Inside either a warped audio clip or a MIDI clip, you can slide the material around within the clip’s edges: hold CtrlShift (Win) / ShiftOption (Mac) as you drag the clip’s waveform or MIDI display. To skip grid snapping, keep CtrlAltShift (Win) / CmdOptionShift (Mac) held down while dragging the clip’s contents.

### 6.8 Audio Clip Fades and Crossfades

In the Arrangement View, the head and tail of audio clips carry volume fades you can tune. On top of that, neighboring clips sharing an audio track may be _crossfaded_.

You will find fade controls at the edges of audio clips, so long as the track is tall enough to reveal the fade handles. Where a track is folded or too short, raise its height until those handles show up.

Hovering over an audio clip brings up the fade handles, which start out as little squares at the clip’s corners.

Fade Handles in an Audio Clip.

When [Automation Mode](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) is on, holding the F key as you hover over an automation lane briefly surfaces the fade controls.

With the Fade In Start and Fade Out End handles, you reshape how long a fade in or fade out lasts while leaving the fade peaks alone. Even so, a fade edge cannot pass beyond its fade peak. Grab one of these handles and drag it across the clip to resize the fade. The fade’s steepness is further tunable through the Fade Curve handle, which bends the fade’s curve.

Adjusted Fades in a Clip.

A fade’s length can also be fixed by [selecting a range of time within the clip](https://www.ableton.com/en/live-manual/12/arrangement-view/#selecting-clips-and-time) covering the clip’s head or tail, then running the Create Fade In/Out command in the Create menu or pressing CtrlAltF (Win) / CmdOptionF (Mac).

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

### 6.9 Selecting Clips and Time

Beyond shifting and resizing clips, editing the Arrangement runs on selections: you pick something out, then run a command on that pick (Cut, Copy, Paste, Duplicate, for example).

Selection behaves as follows:

- A click on a clip selects that clip.
- A click on the empty Arrangement background marks a moment in time, drawn as a blinking insert marker. From there, the left and right arrow keys walk the insert marker along time, while the up and down arrow keys carry it between tracks. Holding Ctrl (Win) / Option (Mac) as you press the left and right arrow keys jumps the insert marker to locators and to clip edges within the chosen track or tracks.
- A click-and-drag picks out a timespan.
- To get at the time inside a clip for editing, open up its track by clicking the button beside the track name. Bear in mind selected tracks also open up via the U key. The unfolded track’s height is adjustable by dragging the split line beneath the Unfold Track button, or through the Alt+ (Win) / Option+ (Mac) and Alt- (Win) / Option- (Mac) shortcut keys. Track height can likewise be changed by holding Alt (Win) / Option (Mac) and pinching on a supported trackpad or touchscreen. To resize every track in the Arrangement View together, hold Alt (Win) / Option (Mac) as you resize a single one. You can also open up all tracks in one move by holding the Alt (Win) / Option (Mac) modifier while clicking the button, or with the AltU (Win) / OptionU (Mac) shortcut.
  Adjusting an Unfolded Track’s Height.
- Dragging through the clip’s waveform or MIDI display lets you select time inside the clip.
- A click on the loop brace acts as a shortcut for the Edit menu’s Select Loop command, picking out everything inside the loop.
- Holding Shift while you click widens an existing selection within the same track or over several tracks. You may also hold Shift and use the arrow keys to grow or shrink the selection.
- Hitting the 0 key switches off a selection of material, even one spanning several clips. Bear in mind that pressing 0 while a track header is selected switches that track off.
- A selection of audio material can be [reversed](https://www.ableton.com/en/live-manual/12/clip-view/#reversing-samples), even across several audio clips. For this, highlight the time span you wish to reverse, then pick the Reverse Clip(s) command from the clip’s context menu or tap the R shortcut key. Bear in mind a selection holding MIDI clips cannot be reversed.
- A selection of material can be nudged with the left and right arrow keys.

### 6.10 Using the Editing Grid

To make Arrangement editing smoother, the cursor latches onto grid lines standing for the meter subdivisions of the song tempo. That grid may be configured as either zoom-adaptive or fixed.
