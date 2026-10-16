# MIDI Note Split Chop And Join

Open when you need guidance on MIDI Note Split Chop And Join in Ableton Live.

Context: [Note Operations](midi-note-operations-routes.md#1058-note-operations).

<a id="source-10581-split"></a>
#### 10.5.8.1 Split

Split cuts a note into two pieces. To invoke it, keep the E key down and trace a line over the notes you want cut. Alternatively, hold E while clicking and dragging sideways within a note, which lets you split it and fine-tune where the cut lands at the same moment.

Throw in the Ctrl (Win) / Cmd (Mac) modifier to lock the split point onto the current grid.

Splitting Notes with a Mouse.

With nothing selected, the Ctrl+E (Win) / Cmd+E (Mac) keyboard shortcut splits every note that crosses the insert marker or reaches past the time selection. The Split Note(s) command in the Edit menu or in the MIDI Note Editor’s context menu does the same thing. Keep in mind this command stays available only while at least one note touches the insert marker or extends beyond the time selection.

<a id="source-10582-chop"></a>
#### 10.5.8.2 Chop

Chop lets you break notes into multiple segments according to whatever the grid settings are.

Chopping Notes.

How you chop notes varies according to whether you reach for the computer keyboard or the mouse.

Chop notes using the keyboard:

- Pick your notes and hit the Ctrl+E (Win) / Cmd+E (Mac) key combination to slice the selected notes into segments that follow the current grid settings. The Chop Note(s) on Grid command in the Edit menu or the MIDI Note Editor’s context menu works as well.
- With notes selected, press the Chop shortcut, keep the Ctrl (Win) / Cmd (Mac) modifier held, and tap the up and down arrow keys to raise or lower how many segments the notes get cut into. Throwing in the Shift modifier scales that segment count up or down by a power of two.

Chop notes using the mouse:

- Select your notes, hit the E+Ctrl (Win) / E+Option (Mac) key combination, then hover over any of the selected notes and drag up or down to raise or lower how many segments the notes are cut into. Throwing in the Shift modifier scales that segment count up or down by a power of two.

Increasing the Number of Parts Into Which Notes Are Chopped.

<a id="source-10583-join"></a>
#### 10.5.8.3 Join

Join fuses every selected note that shares a pitch into a single note, holding onto the MPE contents and stitching the MPE envelopes together right alongside the MIDI notes.

To merge notes, pick out notes sitting in the same key track, then hit the Ctrl+J (Win) / Cmd+J (Mac) keyboard shortcut or reach for the Join Notes command in the Edit menu or the MIDI Note Editor’s context menu.

The Join Notes Context Menu Command.
