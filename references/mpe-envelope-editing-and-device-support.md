# MPE Envelope Editing And Device Support

Open when you need guidance on MPE Envelope Editing And Device Support in Ableton Live.

Context: [Editing MPE](mpe-and-audio-midi-routes.md#12-editing-mpe).

<a id="source-121-viewing-mpe-data"></a>
### 12.1 Viewing MPE Data

A MIDI Clip with MPE Data in the Clip View.

To inspect a MIDI clip's MPE data, start by opening Clip View through a double-click on the clip, then either select the Note Expression Tab or press the key command Alt+3 (Win) / Option+3 (Mac), which brings up the Expression Editors along the bottom edge of Clip View. Four out of the five MPE parameters each occupy a dedicated expression lane: Slide, Pressure, Velocity, and Release Velocity. Out of the box, only Slide and Pressure are visible. The fifth parameter, Pitch, has its envelopes drawn directly over the matching notes in the MIDI Note Editor.

You can reveal or conceal any expression lane using the lane selector toggle buttons on the left side. Just below those lane selector toggle buttons sits a triangular toggle button that reveals or conceals all the active lanes together.

These Buttons Toggle Visibility of Expression Lanes.

Whenever every expression lane selector is concealed or disabled, a press of the triangular toggle button brings up all the expression lanes together. Resizing each lane on its own is done through its split line. To resize every lane at the same time, drag the split line that sits between the lanes and the MIDI Note Editor.

Holding Alt (Win) / Option (Mac) as you click the triangular toggle button shows all the expression lanes. Hide those lanes again — whether through the triangular toggle button, or instead by a drag of the Expression Editor View split line — and the lane visibility toggles vanish along with them.

Per-note controller movement under MPE shows up on the MIDI track meters. Should per-note controller changes travel through a meter, that meter's bottommost dot glows blue.

<a id="source-122-editing-mpe-data"></a>
### 12.2 Editing MPE Data

With the Note Expression tab showing, click a note inside the MIDI Note Editor (or click any one of that note's expression dimensions), and the note appears inside a see-through overlay. Its envelopes surface, together with whatever breakpoints already exist, letting you reshape the note’s Pitch, Slide, and Pressure envelopes, whereas markers handle changes to the note’s Velocity and Release Velocity values. Notes that aren't selected turn gray, and their expression envelopes fade.

Select a Note to View Its Expression Envelopes.

Once you've clicked the note or envelope you intend to work on, every expression breakpoint of the selected envelope, plus the line segments joining them, turns into a draggable object. A selection is created by clicking and dragging across the envelope’s background. The list below explains how MPE data editing operates:

- Click somewhere along a line segment and a fresh breakpoint appears at that spot.
- Click a breakpoint to remove it.
- So that breakpoint editing goes faster, expression values display whenever you make, hover above, or drag a breakpoint. Keep in mind that when you hover over or drag a selected line segment, the expression value displayed matches the breakpoint value sitting under the cursor’s present spot.
  A Breakpoint’s Expression Value.
- To reposition a breakpoint, click and drag it where you want. When the breakpoint you're dragging belongs to the active selection, every other breakpoint in that selection shifts along with it.
- Right-click any breakpoint and pick Edit Value out of the context menu. From there you can type a precise value into the editable field with your computer keyboard. When several breakpoints are selected, all of them move in a relative fashion. In the same way, new breakpoints can be placed at a precise value by right-clicking a preview breakpoint and selecting the Add Value command.
- To select a line segment, click just beside it (not on it) or hold Shift and click straight on the segment. While keeping the left mouse button pressed, drag the segment to wherever you want. Should the line segment you're dragging fall inside the active time selection, Live adds breakpoints at the edges of the selection and the whole segment shifts as a unit.
  To Move all Breakpoints Within the Selection, Drag Any One of Them.
- Within the Note Expression tab, the grid starts out switched off so you can edit more precisely. Bear in mind that this grid keeps its own settings, separate from the grid in the other tabs, and those settings are stored with the clip.
- Should you want it, turn the grid on through the Snap to Grid options menu entry or with the Ctrl+4 (Win) / Cmd+4 (Mac) shortcut. Once the grid is active, breakpoints and line segments lock onto time positions occupied by adjacent breakpoints. A breakpoint placed near a grid line snaps to that line on its own.
- As you move a line segment or breakpoint, hold Shift during the drag to confine the motion to just the horizontal or just the vertical axis.
- Keeping the Shift modifier held down while you drag vertically lets you fine-tune the breakpoint or line segment value with greater precision.
- A neighboring breakpoint can be deleted by dragging a breakpoint or line segment “over” it horizontally until it's gone.
- Hold Alt (Win) / Option (Mac) and drag a line segment to bend it into a curve. A double-click with Alt (Win) / Option (Mac) held restores the segment to a straight line.
  A Curved Envelope Segment.
- Apart from the Pitch expression envelope, the Slide, Pressure, Velocity and Release Velocity envelopes can be scaled proportionally over a note’s whole length, much like velocities are for several selected notes. The procedure: click somewhere outside the note’s region first, then float the mouse over the envelope you want. As soon as the envelope goes blue, click and drag upward or downward, and it scales to match. The same thing happens when you edit expression envelopes across multiple selected notes together.
- It's also possible to shift every selected breakpoint by the same amount instead of scaling them. For that, begin by clicking the envelope you want to change, then press Ctrl+A (Win) / Cmd+A (Mac) to grab all the breakpoints, and drag up or down with the mouse to raise or lower their value; a leftward or rightward drag slides every breakpoint horizontally as one group.
- Moving a note carries its expression envelopes along.
- Stretching a MIDI note via the MIDI stretch markers in the MIDI Editor, or with the ÷2 and x2 buttons in the Notes tab, stretches any per-note expression tied to that note as well.
- Hold Alt (Win) / Cmd (Mac) with the grid off and Pitch breakpoints snap to the closest semitone. The same applies to Pitch values while in Draw Mode. To override this, use those same shortcuts when the grid is on.
- Pitch envelopes vanish once Fold Mode is switched on in the Note Expression tab.
- While the Note Expression tab is showing, the Zoom to Clip Selection command or the Z key shortcut sets the zoom according to the pitch bend values held within the time selection.
- While the Note Expression tab is showing, the Clear All Envelopes entry found in the context menu of the MIDI Note Editor and the per-note expression lanes wipes every expression envelope from one or several selected notes.

<a id="source-123-drawing-envelopes"></a>
### 12.3 Drawing Envelopes

Once Draw Mode is active, a click-and-drag lets you sketch an envelope by hand inside the Pitch, Slide and Pressure expression lanes.

You can switch Draw Mode on or off for MPE data through the Draw Mode Option in the Option menu, by clicking the Control Bar’s Draw Mode switch, or by tapping B, then clicking the envelope you'd like to work on. Holding B as you edit with the mouse flips Draw Mode on temporarily.

Drawing an Envelope.

Keeping the Shift modifier pressed during a vertical drag lets you tune a step's expression value with more precision.

Activate the grid — via the Snap to Grid options menu entry, or else the Ctrl+4 (Win) / Cmd+4 (Mac) shortcut — and each drawn step takes on the width of the grid currently displayed; you can then reshape these with several [handy shortcuts](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid). For a brief grid-aligned draw while the grid is off, hold Alt (Win) / Cmd (Mac) as you draw.

<a id="source-124-mpe-in-lives-devices-and-on-push-2"></a>
### 12.4 MPE in Live’s Devices and on Push 2

A lot of Live devices handle MPE and ship with MPE presets that add fresh layers of interaction and playability to your sound. Thanks to the expressive range built into these devices, you can also make use of polyphonic aftertouch on Push 2.

<a id="source-125-mpe-in-external-plug-ins"></a>
### 12.5 MPE in External Plug-ins

Live also lets you reach and modulate the MPE data belonging to MPE-enabled plug-ins.

Whether a plug-in device’s MPE Mode is on or off gets stored as part of that device’s default configuration.

When a plug-in offers MIDI outs and has MPE turned on, it can send MPE out as well.

<a id="source-126-mpemulti-channel-settings"></a>
### 12.6 MPE/Multi-channel Settings

When you need a particular MPE configuration, an MPE/Multi-channel Settings dialog box is reachable from:

- The Ext. Instrument device.
- The I/O section of Live’s mixer.
- The context menu of an MPE-enabled plug-in.

Such settings come in handy for hardware synths that demand a certain MPE configuration, or for plug-ins that lack official MPE support yet still work with MPE controllers because they're multi-timbral.
