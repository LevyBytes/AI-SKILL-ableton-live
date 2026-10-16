# MIDI Pitch Time Transformations

Open when you need guidance on MIDI Pitch Time Transformations in Ableton Live.

Context: [Pitch and Time Utilities](midi-note-operations-routes.md#1059-pitch-and-time-utilities).

<a id="source-10591-transpose"></a>
#### 10.5.9.1 Transpose

The Transpose slider shows the pitch span of the notes, and it doubles as a way to transpose a note or several notes inside a time selection. Drag the slider upward or downward, or punch a number into it, to shift notes by however many semitones or scale degrees you choose (the latter applying when a clip scale is active).

The Transpose Slider.

Selected notes can likewise be transposed straight inside the MIDI Note Editor using the up and down arrow keys. For octave jumps, keep Shift held as you tap the up or down arrow keys.

<a id="source-10592-fit-to-scale"></a>
#### 10.5.9.2 Fit to Scale

The Fit to Scale button nudges the pitches of notes in the clip or selection so they land inside the scale assigned to that clip. Each note moves to the nearest scale degree of the chosen scale, defaulting to the lower scale degree whenever two are equidistant. Should no scale be active for the clip, the button appears greyed out.

The Fit to Scale Button.

<a id="source-10593-invert"></a>
#### 10.5.9.3 Invert

Invert is a pitch move in which the topmost note trades places with the bottommost one, while the remaining notes get mirrored vertically, so the whole selection ends up flipped “upside-down”.

The Invert Button.

Whenever a scale is active for the clip, Invert works out each note’s mirrored position with respect to the prevailing scale degrees.

Note: don’t mix up Invert with the Invert Selection option covered in the [Selecting Notes and Timespan](https://www.ableton.com/en/live-manual/12/editing-midi/#selecting-notes-and-timespan) section earlier on: the first is a _pitch_ alteration applied to a note selection, while the second alters _what_ happens to be selected.

<a id="source-10594-intervals"></a>
#### 10.5.9.4 Intervals

With the Interval Size slider together with the Add Interval button, you decide how many semitones or scale degrees (when a clip scale is active) the pitches of fresh notes will sit away from those in your original note selection. It’s a handy route to building chords in a hurry.

When a note selection already exists, changing the Interval Size slider value drops new notes in and selects them at once inside the MIDI Note Editor. If nothing is selected, the slider only stores the interval size, which you then commit with the Add Interval button. Pressing that button while no notes are selected adds new notes at the given interval for every note the clip already holds.

The Interval Size Slider and the Add Interval Button.

<a id="source-10595-stretch"></a>
#### 10.5.9.5 Stretch

The note length of selected notes can be reshaped fast through a trio of controls in the Pitch and Time Utilities panel: the Stretch Factor control plus the Double (×2) and Halve (/2) buttons.

Stretch dictates the multiplier applied to a note’s length. Sitting to the right of the Stretch control, the ×2 and /2 buttons respectively lengthen or shorten — by a factor of 2 — a note’s duration, a time selection, or the loop region.

Note Stretching Options.

Bear in mind the Stretch control leaves the loop region’s length untouched.

<a id="source-10596-note-duration"></a>
#### 10.5.9.6 Note Duration

A single note duration, or length, can be assigned to every selected note. You may fit note lengths into a time range, lean on the current grid setting to drive note duration, or pick a particular length out of the choices in the Duration drop-down menu.

After settling on the length you want, push it onto the selected notes with the Set Length button. When nothing is selected, clicking that button hands the chosen note length to all of the clip’s notes.

Note Duration Options.

<a id="source-10597-humanize"></a>
#### 10.5.9.7 Humanize

Humanize introduces some wobble into note start times so the piece sheds any robotic stiffness. You dial in the variation percentage with the Humanize Amount slider, reaching as far as a quarter of a grid division ahead of or behind where the note originally sat, and you commit it through the Humanize button.

Humanize Options.

<a id="source-10598-reverse"></a>
#### 10.5.9.8 Reverse

The Reverse button reshuffles the selection so the final note swaps places with the opening one while everything sitting between them is mirrored horizontally. With no notes selected, the whole clip gets reversed.

The Reverse Button.

<a id="source-10599-legato"></a>
#### 10.5.9.9 Legato

Hitting the Legato button stretches (or trims) each selected note’s duration so that it runs right up to where the following note begins. The final note is carried out to the loop’s end.

The Legato Button.

Legato note lengths can also be produced with the [Span MIDI Tool](https://www.ableton.com/en/live-manual/12/midi-tools/#span).
