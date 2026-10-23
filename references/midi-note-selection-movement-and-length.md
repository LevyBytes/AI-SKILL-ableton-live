# MIDI Note Selection Movement And Length

Open when you need guidance on MIDI Note Selection Movement And Length in Ableton Live.

Context: [Editing MIDI Notes](editing-midi.md#105-editing-midi-notes).

<a id="source-1051-non-destructive-editing"></a>
### 10.5.1 Non-Destructive Editing

At any time you can roll a MIDI clip back to how it was before by invoking the Edit menu’s Undo command. On top of that, when the clip you are editing came from a MIDI file stored on your drive, nothing you do touches that original MIDI file, since Live folds its contents into your Live Set during import.

<a id="source-1052-selecting-notes-and-timespan"></a>
### 10.5.2 Selecting Notes and Timespan

A click within the MIDI Note Editor picks a moment in time, shown by a blinking insert marker. The insert marker can also be driven to a particular spot with the left and right arrow keys, in line with the grid settings. Holding the Ctrl (Win) / Option (Mac) key as you tap the left or right arrow key jumps the insert marker to the previous or next note boundary. Pressing the Home or End key sends the insert marker to the start or end of a MIDI clip, respectively.

A click-drag within the MIDI Note Editor picks a timespan. Should the dashed outline of that chosen timespan surround any notes, those notes get selected automatically as well. Tap Enter to flip the selection back and forth between the timespan itself and whatever notes fall inside it. To clear the time or note selection, click somewhere in the MIDI Note Editor outside the selection or hit the Esc key. The arrow keys also clear a time selection, since they reposition the insert marker. Be aware that pressing the arrow keys while a note selection is active relocates the chosen notes along the timeline (left and right arrow keys) or transposes them (up and down arrow keys).

A timespan can likewise be chosen from the computer keyboard. Keep Shift held while tapping the arrow keys to mark out a timespan beginning at the insert marker, governed by the grid settings. Repeating that combination with a time selection already present grows or shrinks it. Throwing the Alt (Win) / Cmd (Mac) key into the mix grows or shrinks the selection without regard to the grid settings. Holding Alt (Win) / Option (Mac) along with Shift while tapping the arrow keys grows or shrinks the timespan out to the next or previous note boundary.

A lone note can be chosen with a click. The keyboard works too: park the insert marker beside the note you intend to grab, then hold Ctrl (Win) / Option (Mac) and tap either the up or the down arrow key, which grabs the note closest to the insert marker. Repeating that combination shifts the selection onward to the next or previous note in time. To move the selection to the following note within the same key track, hold Ctrl (Win) / Option (Mac) while tapping the left or right arrow keys.

Several notes at once can be chosen by clicking and dragging within the MIDI Note Editor. Tacking on the Shift modifier folds more notes into your existing selection. A single note can likewise be pulled out of your selection by holding Shift and clicking it. Holding Shift and clicking the piano ruler folds every note in one key track into the selection, or strips them out if they were already part of it. Click somewhere away from the selection in the MIDI Note Editor or hit Esc to drop the notes.

Several notes can also be chosen from the keyboard by grabbing one note and then pressing Ctrl+Shift (Win) / Option+Shift (Mac) along with the up or down arrow key. Trigger the shortcut repeatedly, or hold it down, to keep extending your current note selection. The Ctrl+A (Win) / Cmd+A (Mac) keyboard shortcut grabs every note, and the Esc key clears all selected notes.

When you have several notes selected but not the whole clip, you can flip between the notes presently selected and those left unselected with the Invert Selection command, found in the Edit menu or the MIDI Note Editor’s context menu. The Ctrl+Shift+A (Win) / Cmd+Shift+A (Mac) keyboard shortcut does the same job.

<a id="source-1053-find-and-select-notes"></a>
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
- _Velocity_: locates and grabs notes of a defined velocity or sitting inside a defined velocity range, either of which you dial in with the Min/Max Velocity sliders.

As you tweak a filter’s parameters it takes effect and the matching notes get selected on the fly; a yellow dot shows up alongside the filter name in the Filter chooser to signal that the filter is in effect. To bring another filter into play, choose it in the Filter chooser and set its parameters. Clicking anywhere in the MIDI Note Editor switches off every filter that Find and Select Notes has in effect. Keep in mind this drops all note selections.

Every filter comes with two shared controls: the _Invert_ toggle and the _Select_ button. Switching on the Invert toggle selects all of the notes that fail to match the filter’s search criteria. The Select button grabs every note matching the current filter criteria, which is handy for re-running a switched-off filter without touching its parameters.

While the Find and Select Notes toggle is on, the mouse can be used to refine the note selections the filters produced. As an example, Shift-clicking a key on the piano ruler folds all of that key track’s notes into the selection. You can also lay down evenly spaced repeating time selections by holding Shift and then clicking and dragging left or right within the MIDI Note Editor.

<a id="source-1054-moving-notes"></a>
### 10.5.4 Moving Notes

Within the MIDI Note Editor, notes travel horizontally (which alters their timing) as well as vertically (which alters their transposition). The movement happens either through clicking and dragging or via the arrow keys on your computer keyboard. Unless the grid is switched off, notes obey [grid snapping](https://www.ableton.com/en/live-manual/12/editing-midi/#grid-snapping). For nudging notes free of grid snapping, hold Alt (Win) / Cmd (Mac) as you tap the left or right arrow keys.

Once notes are selected, the Edit menu lets you run editing actions on them, Copy and Paste among them. Whatever is on the clipboard gets pasted beginning at the insert marker’s position. The Ctrl (Win) / Option (Mac) modifier also lets you click and drag duplicates of notes off to a new spot. Should you start a click-drag to relocate notes and then change your mind in favor of copying them, you can hit Ctrl (Win) / Option (Mac) partway through the drag.

In the course of editing or drawing, you might drop a new note over the top of an existing one. When the new note covers the start of the original, the original gets overwritten. When the new note covers the end of the original, the original gets trimmed shorter.

<a id="source-1055-changing-note-length"></a>
### 10.5.5 Changing Note Length

Grabbing a note’s left or right edge and dragging it resizes the note’s length. Just like note positions, note lengths move freely as far as the previous or next grid line, then become quantized once you drag past it, unless you keep the Alt (Win) / Cmd (Mac) modifier held.

Note length can be changed from the computer keyboard as well. Shift combined with the left or right arrow keys lengthens or trims the duration of the selected notes, following the grid settings. To lengthen or pull back notes free of grid snapping, additionally hold Alt (Win) / Cmd (Mac).

Changing Note Length.

Every selected note’s duration can be stretched until its start and end points coincide with the current time or note selection. Use the Fit to Time Range option for this, or its keyboard shortcut, Ctrl+Alt+J (Win) / Cmd+Option+J (Mac). As a command, that option appears in the Edit menu, and also in the context menu of the MIDI Note Editor. A third route is to choose the option from the Duration drop-down menu within the Clip View’s Pitch and Time Utilities panel, then carry it out via the Set Length button.

<a id="source-editing-midi-part-2"></a>

Fitting Notes into Time Range.
