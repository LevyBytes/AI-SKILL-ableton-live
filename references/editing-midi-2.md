# Editing Midi (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Fitting Notes into Time Range.

### 10.5.6 MIDI Note Stretch

MIDI Note Stretch Markers.

Selecting several notes, or a span of time, brings up Note Stretch markers beneath the scrub area, letting you rescale the notes proportionally across time. This pair of downward-pointing handles latches onto the start and the finish of whatever you have selected.

Grab one handle and drag it sideways, and the chosen notes scale up or down while keeping the ratio of their original durations. You can slide Note Stretch markers freely up to the closest grid or offset position on either side; past that they latch onto the MIDI Note Editor’s grid lines, unless the grid is hidden or you hold the Alt (Win) / Cmd (Mac) modifier as you drag.

Hover the pointer between the two Note Stretch markers and a “pseudo” stretch marker shows up. Dragging it expands or contracts whatever sits between the fixed markers while leaving everything beyond them untouched. That pseudo marker follows the very same grid-snapping rules the fixed ones do.

You can even drag a single Note Stretch marker past the other one, and doing so flips the sequence of the stretched notes around compared with how they originally ran.

Tweaking the Note Stretch markers carries over to the timing of the clip’s [linked clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#midi-controller-clip-envelopes). Unlinked clip envelopes stay as they are.

Notes can also be stretched through the purpose-built [Stretch](https://www.ableton.com/en/live-manual/12/editing-midi/#stretch) controls found in the Clip View’s Pitch and Time Utilities panel.

### 10.5.7 Deactivating Notes

To switch a note (or several) off, that is to mute it, select it and hit 0, or reach for the Deactivate Note(s) command in the Edit menu or within the context menu of either the piano ruler or the MIDI Note Editor. A deactivated note turns grey and stops sounding. Hitting 0 once more brings the notes back to life.

### 10.5.8 Note Operations

The MIDI Note Editor offers a handful of further editing moves: carving notes into a couple or many segments via the Split and Chop operations, and merging distinct same-pitch notes through the Join operation.

#### 10.5.8.1 Split

Split cuts a note into two pieces. To invoke it, keep the E key down and trace a line over the notes you want cut. Alternatively, hold E while clicking and dragging sideways within a note, which lets you split it and fine-tune where the cut lands at the same moment.

Throw in the Ctrl (Win) / Cmd (Mac) modifier to lock the split point onto the current grid.

Splitting Notes with a Mouse.

With nothing selected, the CtrlE (Win) / CmdE (Mac) keyboard shortcut splits every note that crosses the insert marker or reaches past the time selection. The Split Note(s) command in the Edit menu or in the MIDI Note Editor’s context menu does the same thing. Keep in mind this command stays available only while at least one note touches the insert marker or extends beyond the time selection.

#### 10.5.8.2 Chop

Chop lets you break notes into multiple segments according to whatever the grid settings are.

Chopping Notes.

How you chop notes varies according to whether you reach for the computer keyboard or the mouse.

Chop notes using the keyboard: - Pick your notes and hit the CtrlE (Win) / CmdE (Mac) key combination to slice the selected notes into segments that follow the current grid settings. The Chop Note(s) on Grid command in the Edit menu or the MIDI Note Editor’s context menu works as well. - With notes selected, press the Chop shortcut, keep the Ctrl (Win) / Cmd (Mac) modifier held, and tap the up and down arrow keys to raise or lower how many segments the notes get cut into. Throwing in the Shift modifier scales that segment count up or down by a power of two.

Chop notes using the mouse: - Select your notes, hit the ECtrl (Win) / EOption (Mac) key combination, then hover over any of the selected notes and drag up or down to raise or lower how many segments the notes are cut into. Throwing in the Shift modifier scales that segment count up or down by a power of two.

Increasing the Number of Parts Into Which Notes Are Chopped.

#### 10.5.8.3 Join

Join fuses every selected note that shares a pitch into a single note, holding onto the MPE contents and stitching the MPE envelopes together right alongside the MIDI notes.

To merge notes, pick out notes sitting in the same key track, then hit the CtrlJ (Win) / CmdJ (Mac) keyboard shortcut or reach for the Join Notes command in the Edit menu or the MIDI Note Editor’s context menu.

The Join Notes Context Menu Command.

### 10.5.9 Pitch and Time Utilities

[The Pitch and Time Utilities panel](https://www.ableton.com/en/live-manual/12/clip-view/#pitch-and-time-utilities-panel) gathers tools that give you several fast ways to reshape the notes inside a MIDI clip. Whatever you do here lands on the notes you have selected, or on a time range. With nothing selected, edits made through button controls reach across the entire clip.

#### 10.5.9.1 Transpose

The Transpose slider shows the pitch span of the notes, and it doubles as a way to transpose a note or several notes inside a time selection. Drag the slider upward or downward, or punch a number into it, to shift notes by however many semitones or scale degrees you choose (the latter applying when a clip scale is active).

The Transpose Slider.

Selected notes can likewise be transposed straight inside the MIDI Note Editor using the up and down arrow keys. For octave jumps, keep Shift held as you tap the up or down arrow keys.

#### 10.5.9.2 Fit to Scale

The Fit to Scale button nudges the pitches of notes in the clip or selection so they land inside the scale assigned to that clip. Each note moves to the nearest scale degree of the chosen scale, defaulting to the lower scale degree whenever two are equidistant. Should no scale be active for the clip, the button appears greyed out.

The Fit to Scale Button.

#### 10.5.9.3 Invert

Invert is a pitch move in which the topmost note trades places with the bottommost one, while the remaining notes get mirrored vertically, so the whole selection ends up flipped “upside-down”.

The Invert Button.

Whenever a scale is active for the clip, Invert works out each note’s mirrored position with respect to the prevailing scale degrees.

Note: don’t mix up Invert with the Invert Selection option covered in the [Selecting Notes and Timespan](https://www.ableton.com/en/live-manual/12/editing-midi/#selecting-notes-and-timespan) section earlier on: the first is a _pitch_ alteration applied to a note selection, while the second alters _what_ happens to be selected.

#### 10.5.9.4 Intervals

With the Interval Size slider together with the Add Interval button, you decide how many semitones or scale degrees (when a clip scale is active) the pitches of fresh notes will sit away from those in your original note selection. It’s a handy route to building chords in a hurry.

When a note selection already exists, changing the Interval Size slider value drops new notes in and selects them at once inside the MIDI Note Editor. If nothing is selected, the slider only stores the interval size, which you then commit with the Add Interval button. Pressing that button while no notes are selected adds new notes at the given interval for every note the clip already holds.

The Interval Size Slider and the Add Interval Button.

#### 10.5.9.5 Stretch

The note length of selected notes can be reshaped fast through a trio of controls in the Pitch and Time Utilities panel: the Stretch Factor control plus the Double (×2) and Halve (/2) buttons.

Stretch dictates the multiplier applied to a note’s length. Sitting to the right of the Stretch control, the ×2 and /2 buttons respectively lengthen or shorten — by a factor of 2 — a note’s duration, a time selection, or the loop region.

Note Stretching Options.

Bear in mind the Stretch control leaves the loop region’s length untouched.

#### 10.5.9.6 Note Duration

A single note duration, or length, can be assigned to every selected note. You may fit note lengths into a time range, lean on the current grid setting to drive note duration, or pick a particular length out of the choices in the Duration drop-down menu.

After settling on the length you want, push it onto the selected notes with the Set Length button. When nothing is selected, clicking that button hands the chosen note length to all of the clip’s notes.

Note Duration Options.

#### 10.5.9.7 Humanize

Humanize introduces some wobble into note start times so the piece sheds any robotic stiffness. You dial in the variation percentage with the Humanize Amount slider, reaching as far as a quarter of a grid division ahead of or behind where the note originally sat, and you commit it through the Humanize button.

Humanize Options.

#### 10.5.9.8 Reverse

The Reverse button reshuffles the selection so the final note swaps places with the opening one while everything sitting between them is mirrored horizontally. With no notes selected, the whole clip gets reversed.

The Reverse Button.

#### 10.5.9.9 Legato

Hitting the Legato button stretches (or trims) each selected note’s duration so that it runs right up to where the following note begins. The final note is carried out to the loop’s end.

The Legato Button.

Legato note lengths can also be produced with the [Span MIDI Tool](https://www.ableton.com/en/live-manual/12/midi-tools/#span).

### 10.5.10 MIDI Tools

Housed in the Transform and Generate panels, the MIDI Tools open up further avenues for editing MIDI notes. You can rework existing notes through such things as articulation, interpolation, or ornamentation, or you can have brand-new note patterns spun up on the spot from parameters you specify.

A dedicated [MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#midi-tools) chapter walks through every option on hand for transforming and generating notes.

### 10.5.11 Quantizing Notes

Live gives you four routes to quantizing MIDI notes:

1. Quantize notes right as you [record them](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-quantized-midi-notes).
2. Quantize notes by nudging them until they latch onto the grid lines on screen.
3. Quantize notes via the [Quantize MIDI Tool](https://www.ableton.com/en/live-manual/12/midi-tools/#quantize) found in Clip View’s Transform panel, which hands you finer command over how notes are quantized. This transformation lets you pin down an exact value to quantize notes to (note starts and ends can both be quantized). The Amount control even lets you quantize while sidestepping that rigid “quantized” feel, since it shifts notes by only a fraction of the chosen quantization value.
   The Quantize MIDI Tool.
4. Quantize by picking a note or several and reaching for the Quantize command in the Edit menu, or by pressing the CtrlU (Win) / CmdU (Mac) keyboard shortcut. This route relies on the quantization settings laid out in the Quantize MIDI Tool covered just above. Those same settings open up through the CtrlShiftU (Win) / CmdShiftU (Mac) keyboard shortcut.

### 10.5.12 Editing Velocities

Note velocity gets captured whenever a MIDI note sounds because you struck a key or pad on a controller, and you can think of it as the note’s loudness. Within the MIDI Note Editor, velocity reveals itself through how saturated the note’s color is — paler notes sound quiet, while richer ones sound loud. The Velocity Editor is where you tune the velocity values of a clip’s notes.

To alter a MIDI note’s velocity, click and drag its corresponding marker in the Velocity Editor. The numeric velocity reading appears in the Velocity Editor’s lane header. So you can pinpoint the velocity marker tied to a MIDI note that might be stacked atop others, Live lights up the velocity marker of whichever note your pointer is resting on.

Note Velocity Marker.

Several velocity markers can be picked at once for editing by clicking while you keep the Shift modifier down. To make a batch of notes share one velocity, grab their markers in the Velocity Editor, pull them all the way up or down to peak or floor velocity, and then settle on the value you’re after.

If you’d rather not open the Velocity Editor at all, click any selected note and drag straight up or down while holding the Alt (Win) / Cmd (Mac) modifier.

You can also key in velocity values by hand: select the velocity marker first, type the figure on the computer keyboard, then press Enter.

With Ctrl (Win) / Cmd (Mac) held, the up or down arrow keys bump the values of the selected velocity markers by +/-10. Add Shift to that and you can nudge those selected velocity markers in finer steps.

Beyond editing velocities by hand, you can also define a velocity range or scatter the note velocity values at random through the Velocity Controls that sit beneath the Editor lanes whenever the Velocity Editor is active.

Velocity Controls.

Clicking the Randomize button scatters the velocity values of the selected notes (or notes whose markers are selected). When nothing is selected at all, the values of every note get randomized.

The Randomize Button.

Positioned to the right of the Randomize button, the Randomization Amount slider lets you bound how far the randomized velocities can swing. Each velocity is bumped up or down at random by some amount falling between zero and whatever figure the slider reads. You may also type that slider figure on the keyboard, at which point confirming the new value with Enter sets the randomization off.

The Randomization Amount Slider.

The Ramp sliders let you build a velocity ramp spanning several notes. You fix the velocity of the selection’s opening note with the Ramp Start Value slider, and the Ramp End Value slider does the same for the closing note. Every note in between gets spaced out uniformly across the range the Ramp sliders define.

The Ramp Sliders.

With the Velocity Deviation slider you assign each note a velocity range. From then on, whenever that note sounds, a velocity is picked at random out of the range you named. The values can run positive or negative, raising or lowering velocity in turn. Say you set a velocity range of +20 on a selected note whose velocity value is 60: every time it plays, a random value somewhere between 60 and 80 gets chosen.

The Velocity Deviation Slider.

A shaded patch sitting above or below the velocity markers, together with a dot placed inside them, signals the velocity range. Double-click a velocity marker that carries a range and the range snaps back to 0.

Velocity Markers with Deviation Set.

When more than one note is selected, the range shown in the Velocity Deviation slider adapts to the velocity values already in place. Picture pushing the velocity range up while one note sits at a velocity value of 50 and another at 25: the first note’s velocity range tops out at +77, whereas the second’s can climb to +102. The slider then surfaces both figures to mirror this.

The Velocity Deviation Slider with Varied Ranges of Deviation.

Another way to set the velocity range is to hold Ctrl (Win) / Cmd (Mac) and drag upward or downward from a velocity marker. That works equally for a lone note and for a whole note selection.

#### 10.5.12.1 Drawing Velocities

Draw Mode lets you paint inside the Velocity Editor to assign velocity values rather than tweaking them one at a time. Flip Draw Mode on either by toggling the Control Bar’s Draw Mode button or by tapping the B key.

Drawing velocity reaches the notes that fall inside a particular grid division. Where notes are selected, your drawing touches only those, even if more notes share the grid division. Where none are selected, all of them are touched. Hovering over the Velocity Editor lights up in blue exactly which notes will be affected.

When you want markers drawn one by one (handy for a crescendo, say), switch off grid snapping using the Ctrl4 (Win) / Cmd4 (Mac) shortcut, or just keep the Alt (Win) / Cmd (Mac) modifier held. For markers laid out along a straight line, hold Alt (Win) / Option (Mac) and drag the cursor; tack on Shift to force that line horizontal.

Drawing Identical Velocities (Left) and a Crescendo (Right).

To sketch a velocity ramp across notes that all sit in one key track, click a key on the piano ruler to grab every note in that key track, then draw the ramp into the Velocity Editor.

#### 10.5.12.2 Note Off Velocity

The Velocity Editor handles Note On velocities, but you can bring up the Release Velocity Editor to work with Note Off velocities as well.

Select the Release Velocity Editor via the Lane Selector.

Note Off (or “release”) velocity is a fairly obscure parameter. If velocity stands for how fast you push a key down, then release velocity stands for how fast you let that depressed key back up. Only some devices recognize release velocity. Live’s [Sampler instrument](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sampler), to take one case, exposes Note Off velocity as a modulation source for many parameters.

### 10.5.13 Editing Probabilities

Note probability governs how likely a MIDI note is to fire while the clip plays back. The Chance Editor is where you assign probability to notes.

The Chance Editor.

Keep in mind the Chance Editor lane stays hidden out of the box; reveal it by clicking the triangular Lane Selector drop-down menu, which sits to the right of the Show/Hide All Expression Editors toggle over on the left side of the Clip Content Toolbar.

To shift a MIDI note’s probability value anywhere from 0-100%, click and drag the note’s probability marker within the Chance Editor. So you can find the probability marker tied to a MIDI note that might be stacked among others, Live highlights the probability marker of whichever note your pointer hovers over. While you drag the marker, the running probability value turns up in the Chance Editor’s lane and in the Status Bar alike. Select several notes whose probability values differ and a range of probability values is shown instead.

You may also type note probability values in by hand with a computer keyboard: first select a probability marker, then enter the figure and press Enter. The up or down arrow keys shift the selected probability markers by +/-10%, and holding Shift alongside the arrow keys lets you nudge those selected probability markers in finer increments.

Notes whose probability sits below 100% carry a small triangle in their upper-left corner. That triangle only shows once the key track height has been stretched far enough; otherwise it stays hidden. Widen the key track height by clicking and dragging rightward in the note ruler, which makes the MIDI Note Editor zoom in.

Note probability values can be randomized inside a stated range, measured against the starting probability value. You set that range with the Randomization Amount slider on the Clip Content Toolbar, which is useful for spinning up fresh variations on every loop or for lending the piece a more human feel.

The Randomize Amount Slider.

Each note probability gets shuffled away from its original figure, with the fresh value landing on either side of the starting probability inside the span fixed by the Randomization Amount slider. Take an original probability value of 50% paired with a Randomization Amount of 25%: the randomized probability values then span 25-75%. With notes selected, dialing the slider percentage randomizes their probability values straight away. You may instead type the randomization range on the keyboard and confirm it with Enter. While nothing is selected, moving the slider does nothing until you press Enter or click the Randomize button, and at that moment the randomization sweeps across every note probability.

The Randomize Button.

#### 10.5.13.1 Probability Groups

On top of giving each note its own probability value, you can hand a single probability value to a whole group of notes, so that either every note in the group plays by that value or just one note from the group sounds at any given moment. The two probability group types on offer are:

_Play All_ — every note plays at the probability value fixed by a probability marker. _Play One_ — at any moment only one note from the group sounds, following the set probability, and which note that is gets picked at random.

To build a note probability group, select the notes you want bundled together and click either the Play All or Play One button on the Clip Content Toolbar, according to which probability group type you mean to make.

Play All and Play One Buttons.

After grouping, the Chance Editor shows the notes a lone probability marker: it sports a diamond handle when the group is a Play All type and a triangle handle when it’s a Play One type. Right-click a group probability marker to switch the probability group type. The Play All or Play One buttons on the Clip Content Toolbar flip the group type just as well.

Beyond those dedicated buttons, a few other routes build note probability groups: - Reach for the Group Notes (Play All) or Group Notes (Play One) context menu options in the MIDI Note Editor. - Use the Group Notes (Play All) or Group Notes (Play One) command on the Edit menu. - Hit the CtrlG (Win) / CmdG (Mac) keyboard shortcut, which produces a group matching the type of the one you most recently built through either the dedicated buttons or the context menu.

Hover over a note that sits in a group and all of that group’s notes light up. Whenever the selected notes belong to a probability group, the Status Bar reports the group’s type — spelled out plainly if every note shares one group, or flagged with an asterisk when they don’t.

That small triangle in the upper-left corner of notes whose probability falls under 100% always appears once a note joins a probability group, even where the group’s probability stands at 100%.

To pull a note out of a probability group, select it and click the Ungroup button on the Clip Content Toolbar. Folding a note into a different group likewise strips it from its first group automatically. To dismantle a probability group entirely, select all of its notes and then click Ungroup.

The Ungroup Button.

The same thing happens through the Edit menu’s Ungroup Notes command, the CtrlShiftG (Win) / CmdShiftG (Mac) shortcut, or a right-click on a grouped note marker followed by choosing the Ungroup Notes option. Once notes are ungrouped, the Chance Editor goes back to showing a separate probability marker for each note.

### 10.6 Folding and Scales

The MIDI Note Editor comes with folding options that let you tuck away chosen rows, or key tracks, within the editor. Because these options reach every MIDI clip in the Set, the rows on hand vary from clip to clip across your Set according to which notes each clip actually contains.
