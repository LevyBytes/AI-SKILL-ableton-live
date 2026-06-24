# Editing Midi (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 10. Editing MIDI

Inside Live, a [MIDI clip](https://www.ableton.com/en/live-manual/12/live-concepts/#midi-clips-and-midi-files) holds the notes plus the controller information that drives a MIDI instrument. That instrument might be a [virtual instrument in a MIDI track’s device chain](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects), or it could be an outboard synth reached through the [track’s output routing](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io). What the clip hands to the device is essentially a performance score, defining each note’s pitch, duration, placement and loudness (the MIDI term for loudness being _velocity_). You build MIDI clips in Live’s MIDI Note Editor and refine them with the various tools found across Clip View’s panels, plus the Velocity and Chance Editors.

### 10.1 The MIDI Note Editor Layout

Within the MIDI Note Editor you can insert, reposition and fine-tune MIDI notes so that the ideas in your head turn into actual music.

To bring up the MIDI Note Editor, start by opening [the Clip View](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view), which you do by double-clicking a clip or pressing the CtrlAlt3 (Win) / CmdOption3 (Mac) keyboard shortcut.

Three editor view modes live in the Clip View: the MIDI Note Editor covered here, along with [the Envelopes Editor](https://www.ableton.com/en/live-manual/12/clip-envelopes/#the-clip-envelope-editor) and [the MPE Editor](https://www.ableton.com/en/live-manual/12/editing-mpe/#viewing-mpe-data), which each get their own chapter. You reach these view modes via tabs along the Clip View header. Clicking the Notes tab brings up the MIDI Note Editor.

The MIDI Note Editor Layout.

1.

The tabs along the Clip View header let you switch among the various editor view modes. Confirm that the Notes tab is active in order to [add](https://www.ableton.com/en/live-manual/12/editing-midi/#adding-midi-notes) and [manipulate](https://www.ableton.com/en/live-manual/12/editing-midi/#editing-midi-notes) MIDI notes.

2.

MIDI notes can be placed straight into the MIDI Note Editor’s grid.

3.

Navigation in the MIDI Note Editor works in two directions, vertical and horizontal. Running along the horizontal axis is a time ruler that indicates each note’s position on a musical timeline. On the vertical axis sits the note ruler, presenting the octaves C-2–C8, the limited set of pitches belonging to a loaded [tuning system](https://www.ableton.com/en/live-manual/12/using-tuning-systems/#using-tuning-systems), or a roster of drum pads whenever a Drum Rack is in place. That vertical axis also shows a depiction of a piano keyboard, known as the piano ruler.

Note Scale Position Is Shown Vertically and Beat-Time Horizontally.

1.

Toward the left edge of the Clip View header sit controls for [folding key tracks and scale highlighting](https://www.ableton.com/en/live-manual/12/editing-midi/#folding-and-scales) (assuming a scale is turned on in the MIDI clip), together with [the Find and Select Notes toggle](https://www.ableton.com/en/live-manual/12/editing-midi/#find-and-select-notes).

2.

Whenever the Find and Select Notes toggle is switched on, note selection filters show up just above the time ruler.

3.

With the [Preview switch](https://www.ableton.com/en/live-manual/12/editing-midi/#previewing-notes) located over the piano ruler turned on, clicking a key on the piano ruler — or adding or relocating a MIDI note within a key track — plays back the matching pitch or drum pad.

4.

Underneath the MIDI Note Editor sit the Velocity and Chance Editor lanes plus their controls, which let you [edit note velocities](https://www.ableton.com/en/live-manual/12/editing-midi/#editing-velocities) and [probabilities](https://www.ableton.com/en/live-manual/12/editing-midi/#editing-probabilities). The Velocity Editor alone appears by default, but you can switch its visibility — and the Chance Editor’s — on or off through the triangular Lane Selector drop-down menu. Sitting beside that button, the Show/Hide All Expression Editors toggle reveals or conceals every enabled lane in one move.

Show/Hide All Expression Editors Toggle.

You can also decide which of the Velocity or Chance Editor occupies the visible lane by using the Swap Lane option found in the lane header’s context menu.

Dragging the divider that separates the MIDI Note Editor from the Velocity and/or Chance Editor lanes lets you resize or show/hide those lanes and their controls. Each lane can be resized on its own through its split line as well. Resizing the lanes is also possible with the mousewheel/pinch gesture while the Alt (Win) / Option (Mac) key is held.

1. Over toward the right edge of the Clip View header you can view the active grid setting and change the grid properties through the chooser.

### 10.2 Zooming and Navigating in the MIDI Note Editor

The MIDI Note Editor and what it holds can be worked with in several distinct ways:

MIDI Note Editor Navigation.

1. For fine control over the time zoom level, click and drag up or down within the time ruler. A horizontal drag in the time ruler scrolls the view from one side to the other. You can additionally hold the Ctrl (Win) / Cmd (Mac) modifier while scrolling up and down within the MIDI Note Editor to alter the time zoom level.
2. Scrolling up and down within the note ruler changes which octaves are visible. A horizontal click-drag in the note ruler resizes the zoom level applied to the key tracks, their MIDI notes and the piano ruler keys. You can additionally hold the Alt (Win) / Option (Mac) modifier while scrolling up and down within the MIDI Note Editor to alter the key tracks zoom level.
3. Drag across one or several notes to pick them, or drag across a region of the MIDI Note Editor to grab a span of time. Following that, a double-click on either the note ruler or the time ruler zooms in on whatever you selected. A double-click on the note ruler zooms toward the key tracks, whereas a double-click on the time ruler zooms toward the chosen time span. With nothing selected, double-clicking the note ruler zooms to span the lowest through the highest note present in the clip, and double-clicking the time ruler zooms out to reveal the stretch between the first and the final note. Keep in mind that should you zoom in far enough that the time selection no longer appears on screen, a double-click in the note ruler or time ruler zooms the MIDI Note Editor back out until the whole selection is visible again.
4. Navigation is also served by the clip overview within the Clip View Selector at the lower right of the Live window. It consistently displays everything in the chosen MIDI clip. A black rectangular outline marks the portion of the clip presently visible in the MIDI Note Editor. Scrolling is done by clicking inside that outline and dragging it left or right; dragging it up or down zooms in and out. The outline’s width can be changed by dragging either its left or right edge.

The computer keyboard offers another fast way to move around the current selection in the MIDI Note Editor. Pressing Page Up/Down scrolls vertically by a full octave up or down. Holding the Shift modifier as well scrolls vertically by only a single key track up or down. The + and - keys zoom in and out relative to the current time selection. The Z key zooms all the way in on the current selection. The X key zooms out so the whole clip is visible. Pairing Alt (Win) / Option (Mac) with the + or - key zooms the MIDI Note Editor in or out.

While working on MIDI, the need for additional screen real estate can come up. Dragging vertically on the window split that separates the Session or Arrangement View from the Clip View raises the Clip View’s height, which in turn enlarges the MIDI Note Editor as well.

Dragging the Window Split Between the Session and the Clip Views to Enlarge the MIDI Note Editor.

You can snap the Clip View to its tallest size with the CtrlAltE (Win) / CmdOptionE (Mac) keyboard shortcuts or by choosing the Expand Clip View entry in the View menu.

### 10.2.1 Grid Snapping

The majority of MIDI Note Editor operations respect [grid snapping](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid). What this means in practice is that when you shift note positions the grid behaves magnetically: the moment you begin dragging a note it travels freely until it reaches the first grid line, and from there onward continued dragging makes it snap to grid lines instead of sliding smoothly. To get around grid snapping, switch the grid off with the Grid Settings button, turn off the Snap to Grid option in the Options menu, or hit the Ctrl4 (Win) / Cmd4 (Mac) key combination. You can also override grid snapping momentarily by holding the Alt (Win) / Cmd (Mac) modifier as you edit. The reverse holds too: when the grid is off, holding that same modifier turns it on for the moment.

Notes additionally snap to an offset that derives from where the note originally sat in relation to the grid. That behavior helps retain a groove or a relaxed feel that you would rather not have sounding overly “quantized.”

### 10.2.2 Playback Options

You can have the MIDI Note Editor follow along with playback by engaging the Follow switch on the Control Bar. Follow halts whenever you edit something in the MIDI Note Editor, and it resumes once you click the Follow switch a second time, stop and then restart playback, or stop playback and click in the scrub area within the clip or the Arrangement View.

The Control Bar’s Follow Switch.

With Permanent Scrub Areas turned on in Live’s Display & Input Settings, a click in the scrub area beneath the beat-time ruler launches playback from that spot, quantized to the global quantization setting. Turning on the Options menu’s Chase MIDI Notes command lets MIDI notes sound even when playback gets underway past the MIDI note’s start time.

If the Permanent Scrub Areas preference is switched off, scrubbing is still available by Shift-clicking anywhere within the scrub area or the beat-time ruler. Familiarizing yourself with [looping](https://www.ableton.com/en/live-manual/12/clip-view/#looping-clips) and [scrubbing](https://www.ableton.com/en/live-manual/12/clip-view/#playing-and-scrubbing-clips) clips — and the shortcuts tied to those actions — can likewise make moving around the MIDI Note Editor and auditioning selections faster and simpler.

### 10.3 Creating a MIDI Clip

There are several routes to making a MIDI clip: - through [recording on a MIDI track](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips); - through [capturing MIDI](https://www.ableton.com/en/live-manual/12/recording-new-clips/#capturing-midi); - by double-clicking a vacant Session slot on a MIDI track; - by highlighting a vacant Session slot on a MIDI track and picking the Create menu’s Insert Empty MIDI Clip(s) command, which the CtrlShiftM (Win) / CmdShiftM (Mac) keyboard shortcut also triggers; - by double-clicking the track display of a MIDI track over in the Arrangement View; - or, within the Arrangement View, by highlighting a timespan on a MIDI track and picking the Create menu’s Insert Empty MIDI Clip(s) command, again reachable via the CtrlShiftM (Win) / CmdShiftM (Mac) keyboard shortcut.

### 10.4 Adding MIDI Notes

MIDI clips gain notes as you record yourself performing an instrument on an armed track, or when you pull back the material you played through the Capture MIDI option. Notes can also be entered by hand in the MIDI Note Editor, either by double-clicking at a spot of your choosing or by drawing them with the mouse while Draw Mode is on.

The Control Bar’s Draw Mode Toggle.

### 10.4.1 Draw Mode

To enter Draw Mode, flip the Control Bar’s Draw Mode button or tap the B key. With it turned on, you add notes by clicking and dragging within the MIDI Note Editor. While Draw Mode is on, clicking a note that already exists removes it.

Adding New Notes Using Draw Mode.

Draw Mode comes in two flavors: the “Draw Mode with Pitch Lock” option under the Display & Input Settings keeps drawn MIDI notes locked to just one key track (or pitch) at a time, whereas holding the Alt (Win) / Option (Mac) key switches to freehand melodic drawing. With that option off, Draw Mode falls back on freehand melodic drawing by default, and holding the Alt (Win) / Option (Mac) key turns on pitch-locked drawing. Under melodic Draw Mode, drawing across a note that already exists wipes it out. Under pitch-locked Draw Mode, the notes you draw get wiped out as you bring the cursor back toward the first note you placed. With the MIDI Note Editor focused, the “Draw Mode” item in the Options and context menus reflects the present setting of the “Draw Mode with Pitch Lock” preference, shown as “Draw Mode (Pitch Lock On/Off)”.

Draw Mode comes in handy for laying down notes or patterns in a hurry. With Draw Mode turned off, you reposition notes using the arrow keys or by clicking and dragging — vertically to transpose them or horizontally to shift their timing. While Draw Mode is off, a double-click on a MIDI note deletes it.

### 10.4.2 Previewing Notes

Provided that [an instrument](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects) sits in your MIDI track’s device chain, switching on the Preview switch in the MIDI Editor lets you hear notes the moment you add them or as you select and reposition ones that already exist. When the MIDI track is armed, turning on Preview additionally lets you [step record](https://www.ableton.com/en/live-manual/12/recording-new-clips/#midi-step-recording) fresh notes into the clip. Bear in mind that the Preview switch’s on/off setting carries across every MIDI track in the Live Set.

Previewing MIDI Notes.

### 10.5 Editing MIDI Notes

Working in the MIDI Note Editor mirrors [editing in the Arrangement](https://www.ableton.com/en/live-manual/12/arrangement-view/#selecting-clips-and-time). Either way the workflow revolves around selections: you pick something with the mouse or the computer keyboard, then apply a command (such as Cut, Copy, Paste, Duplicate) to whatever you picked.

### 10.5.1 Non-Destructive Editing

At any time you can roll a MIDI clip back to how it was before by invoking the Edit menu’s Undo command. On top of that, when the clip you are editing came from a MIDI file stored on your drive, nothing you do touches that original MIDI file, since Live folds its contents into your Live Set during import.

### 10.5.2 Selecting Notes and Timespan

A click within the MIDI Note Editor picks a moment in time, shown by a blinking insert marker. The insert marker can also be driven to a particular spot with the left and right arrow keys, in line with the grid settings. Holding the Ctrl (Win) / Option (Mac) key as you tap the left or right arrow key jumps the insert marker to the previous or next note boundary. Pressing the Home or End key sends the insert marker to the start or end of a MIDI clip, respectively.

A click-drag within the MIDI Note Editor picks a timespan. Should the dashed outline of that chosen timespan surround any notes, those notes get selected automatically as well. Tap Enter to flip the selection back and forth between the timespan itself and whatever notes fall inside it. To clear the time or note selection, click somewhere in the MIDI Note Editor outside the selection or hit the Esc key. The arrow keys also clear a time selection, since they reposition the insert marker. Be aware that pressing the arrow keys while a note selection is active relocates the chosen notes along the timeline (left and right arrow keys) or transposes them (up and down arrow keys).

A timespan can likewise be chosen from the computer keyboard. Keep Shift held while tapping the arrow keys to mark out a timespan beginning at the insert marker, governed by the grid settings. Repeating that combination with a time selection already present grows or shrinks it. Throwing the Alt (Win) / Cmd (Mac) key into the mix grows or shrinks the selection without regard to the grid settings. Holding Alt (Win) / Option (Mac) along with Shift while tapping the arrow keys grows or shrinks the timespan out to the next or previous note boundary.

A lone note can be chosen with a click. The keyboard works too: park the insert marker beside the note you intend to grab, then hold Ctrl (Win) / Option (Mac) and tap either the up or the down arrow key, which grabs the note closest to the insert marker. Repeating that combination shifts the selection onward to the next or previous note in time. To move the selection to the following note within the same key track, hold Ctrl (Win) / Option (Mac) while tapping the left or right arrow keys.

Several notes at once can be chosen by clicking and dragging within the MIDI Note Editor. Tacking on the Shift modifier folds more notes into your existing selection. A single note can likewise be pulled out of your selection by holding Shift and clicking it. Holding Shift and clicking the piano ruler folds every note in one key track into the selection, or strips them out if they were already part of it. Click somewhere away from the selection in the MIDI Note Editor or hit Esc to drop the notes.

Several notes can also be chosen from the keyboard by grabbing one note and then pressing CtrlShift (Win) / OptionShift (Mac) along with the up or down arrow key. Trigger the shortcut repeatedly, or hold it down, to keep extending your current note selection. The CtrlA (Win) / CmdA (Mac) keyboard shortcut grabs every note, and the Esc key clears all selected notes.

When you have several notes selected but not the whole clip, you can flip between the notes presently selected and those left unselected with the Invert Selection command, found in the Edit menu or the MIDI Note Editor’s context menu. The CtrlShiftA (Win) / CmdShiftA (Mac) keyboard shortcut does the same job.

### 10.5.3 Find and Select Notes

Note selection filters let you hunt for notes that satisfy particular criteria. The notes turned up this way are selected for you automatically, which comes in handy when you want to rapidly edit many notes sharing, say, a given pitch or duration.

Find and Select Notes Using Filters.

To reveal the filters, switch on the Find and Select Notes toggle in the Clip View header. A chooser sitting beneath the toggle is where you pick a filter for locating and selecting notes. Every filter carries its own set of controls, among them the ability to invert the search so that notes falling outside the filter’s criteria get selected. You may also chain several filters together to build more exact note selections.

Filtering is available across eight separate note properties:

- _Pitch_ locates and grabs the notes carrying whatever pitch or pitches you set through the Pitch toggles. This filter looks across every octave.
- _Time_ locates and grabs notes that fall inside a defined time range. The Start and Length fields establish the range’s starting point and length in beats, while the Repeat field sets how often, in beats, the chosen range repeats.
- _Chance_ locates and grabs notes carrying a defined probability or sitting inside a defined probability range, either of which you dial in with the Min/Max Probability sliders.
- _Condition_ locates and grabs notes satisfying one of three conditions: Active, Chance, or Velocity Deviation. Turning on the Active toggle selects every active note. Turning on the Chance toggle selects every note whose probability sits below 100%. Turning on the Velocity Deviation toggle selects every note that has velocity deviation.
- _Count_ locates and grabs each nth note or chord across a sequence. The Every slider sets which nth note lands in the selection. As an example, a value of 2 selects every second note. The Offset slider lets you shift which note counts as the first one in the selection. The Quantized toggle bundles selected notes by the current grid settings. With it on, every cluster of notes inside a single grid step counts as a value of 1 toward the Every slider. As an example, with the Every slider at 3 and the Quantized toggle on against a fixed grid of 1/16, every third sixteenth note is selected.
- _Duration_ locates and grabs notes of a defined length or sitting inside a defined duration range, either of which you dial in with the Min/Max Duration sliders.
- _Scale_ locates and grabs notes belonging to a defined scale. With the filter’s Use Clip Scale toggle on, the notes lying inside the current clip scale are selected. With that toggle off, you nominate a scale to filter against using the Scale Root and Scale Name choosers.
- _Velocity_ — locates and grabs notes of a defined velocity or sitting inside a defined velocity range, either of which you dial in with the Min/Max Velocity sliders.

As you tweak a filter’s parameters it takes effect and the matching notes get selected on the fly; a yellow dot shows up alongside the filter name in the Filter chooser to signal that the filter is in effect. To bring another filter into play, choose it in the Filter chooser and set its parameters. Clicking anywhere in the MIDI Note Editor switches off every filter that Find and Select Notes has in effect. Keep in mind this drops all note selections.

Every filter comes with two shared controls: the _Invert_ toggle and the _Select_ button. Switching on the Invert toggle selects all of the notes that fail to match the filter’s search criteria. The Select button grabs every note matching the current filter criteria, which is handy for re-running a switched-off filter without touching its parameters.

While the Find and Select Notes toggle is on, the mouse can be used to refine the note selections the filters produced. As an example, Shift-clicking a key on the piano ruler folds all of that key track’s notes into the selection. You can also lay down evenly spaced repeating time selections by holding Shift and then clicking and dragging left or right within the MIDI Note Editor.

### 10.5.4 Moving Notes

Within the MIDI Note Editor, notes travel horizontally (which alters their timing) as well as vertically (which alters their transposition). The movement happens either through clicking and dragging or via the arrow keys on your computer keyboard. Unless the grid is switched off, notes obey [grid snapping](https://www.ableton.com/en/live-manual/12/editing-midi/#grid-snapping). For nudging notes free of grid snapping, hold Alt (Win) / Cmd (Mac) as you tap the left or right arrow keys.

Once notes are selected, the Edit menu lets you run editing actions on them, Copy and Paste among them. Whatever is on the clipboard gets pasted beginning at the insert marker’s position. The Ctrl (Win) / Option (Mac) modifier also lets you click and drag duplicates of notes off to a new spot. Should you start a click-drag to relocate notes and then change your mind in favor of copying them, you can hit Ctrl (Win) / Option (Mac) partway through the drag.

In the course of editing or drawing, you might drop a new note over the top of an existing one. When the new note covers the start of the original, the original gets overwritten. When the new note covers the end of the original, the original gets trimmed shorter.

### 10.5.5 Changing Note Length

Grabbing a note’s left or right edge and dragging it resizes the note’s length. Just like note positions, note lengths move freely as far as the previous or next grid line, then become quantized once you drag past it, unless you keep the Alt (Win) / Cmd (Mac) modifier held.

Note length can be changed from the computer keyboard as well. Shift combined with the left or right arrow keys lengthens or trims the duration of the selected notes, following the grid settings. To lengthen or pull back notes free of grid snapping, additionally hold Alt (Win) / Cmd (Mac).

Changing Note Length.

Every selected note’s duration can be stretched until its start and end points coincide with the current time or note selection. Use the Fit to Time Range option for this, or its keyboard shortcut, CtrlAltJ (Win) / CmdOptionJ (Mac). As a command, that option appears in the Edit menu, and also in the context menu of the MIDI Note Editor. A third route is to choose the option from the Duration drop-down menu within the Clip View’s Pitch and Time Utilities panel, then carry it out via the Set Length button.
