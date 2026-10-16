# MIDI Ornament Quantize Recombine And Span

Open when you need guidance on MIDI Ornament Quantize Recombine And Span in Ableton Live.

Context: [Transformation Tools](midi-tools.md#112-transformation-tools).

<a id="source-1126-ornament"></a>
### 11.2.6 Ornament

Through its Flam and Grace Notes options, the Ornament Transformation lets you tack ornamental notes onto the front of selected notes. Run the Transformation over the same selection a second time and yet more flam or grace notes get slipped in.

The Ornament MIDI Tool.

Choose which kind of ornamental notes to layer on by flipping on either the Flam or the Grace Notes toggle.

The Flam and Grace Notes Toggles.

With Flam, one lone note is tacked onto the front of every selected note.

Where that flam note sits is set by the Flam Position parameter: positive values have the flam note overwrite the front of the original note, whereas negative values slot the flam note ahead of the selected note’s start. Since the parameter’s value is a percentage of the current grid setting, the flam note’s length keys off the grid size rather than the original note’s length. As a result, at 100% / -100% the flam note spans one grid division — sitting at the original note’s start or just before it — and shrinks proportionally as Flam Position drifts toward 0%.

The velocity of the flam notes, measured against the velocity of the original notes, is what the Flam Velocity parameter sets.

Notes Before and After Adding Flam.

With Grace Notes, several notes of matching length are tacked onto the front of each original note.

Using the Grace Notes Pitch buttons you decide the pitch of the added grace notes relative to the original note. Choose High and every other grace note lands one semitone (or scale degree, where a scale is active) above the original notes; choose Low and every other grace note sits one semitone or scale degree under the existing notes. Pick Same and the grace notes share the original notes’ pitch.

Whether the added grace notes overwrite the front of the selected notes (with the parameter at positive values) or sit ahead of the original notes (at negative values) is decided by the Grace Notes Position parameter. Expressed as a share of whatever grid size is active, its value works like this: at 100% / -100% the inserted graces notes span a single grid division, landing either at the original note’s start or right before it.

How loud the grace notes are relative to the velocity of the original notes is set by the Grace Notes Velocity parameter.

The Grace Notes Chance control fixes the odds that each grace note sounds, gauged against the original note’s Chance values.

With the Grace Notes Amount parameter you state how many grace notes to attach to each selected note. Every individual grace note always comes out the same size.

Note Selection Before and After Adding Grace Notes.

<a id="source-1127-quantize"></a>
### 11.2.7 Quantize

By shifting or stretching the selected notes to match the quantization settings you specify, the Quantize MIDI Tool tightens their timing. Be aware that a matching Quantize tool is available for [audio clips](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#quantizing-audio) too.

The Quantize Transformation.

You may quantize notes to the current grid size or instead name a particular meter value (triplets included). It’s open to you to quantize the note start time, the note end time, or both at once. Quantizing a note’s end stretches it until it terminates on the meter subdivision you chose. The Amount control even lets you quantize notes while sidestepping that fully “quantized” feel, since it shifts notes by only a fraction of the set quantization value.

Notes Before and After Applying Quantization.

Besides reaching the Transformation through Clip View’s tabs/panels, you can call up the Quantize MIDI Tool to adjust its parameters via the Quantize Settings… command in the Edit menu, or fire the Ctrl+Shift+U (Win) / Cmd+Shift+U (Mac) shortcut to quantize the selected notes without ever opening the Transform tab/panel.

<a id="source-1128-recombine"></a>
### 11.2.8 Recombine

For a chosen group of notes, the Recombine MIDI Tool reshuffles the position, pitch, duration, or velocity so that a parameter value belonging to one note in the group ends up applied to another note.

The Recombine Transformation.

The Dimension chooser is where you settle on which one of four note parameters Recombine will permute: Position, Pitch, Duration, or Velocity.

The Dimension Chooser.

Recombine offers three approaches to reordering note parameters: 1. Shuffle, in which note parameters are permuted at random. 2. Mirror, in which note parameters are permuted so they run opposite to the note selection. 3. Rotate, in which note parameters are permuted in a circular fashion.

You flip on the Shuffle and Mirror permutation types with their own toggles, while Rotate only kicks in once you give Rotation Steps a value other than 0.

To set Rotation Steps, drag your mouse across the columns inside Recombine’s display, or use the Rotate Step Down/Up buttons beneath the display. The count of available steps always sits one below the number of selected notes. Positive numbers spin parameter values clockwise; negative numbers spin them counter-clockwise.

Pick Position in the Dimension chooser and the Rotate on Grid toggle becomes available. Switched on, it has Recombine count grid cells in the selection — rather than notes — to figure how many Rotation Steps exist. Exactly how many Rotation Steps are available then hinges on the current grid settings.

You can call on each permutation type on its own or stack several together. They run in a fixed order: first Shuffle, then Mirror, then Rotate. Bear in mind that with Shuffle on, a fresh parameter permutation is born every time you hit the Apply button.

Note Velocities Before and After Applying the Shuffle Transformation Mode.

<a id="source-1129-span"></a>
### 11.2.9 Span

Drawing on three articulation types — legato, tenuto and staccato — the Span MIDI Tool reshapes the durations of selected notes.

The Span Transformation.

A couple of extra parameters let you bring some variety to how the notes are transformed:

- Offset shifts note end times by up to a grid step. Positive values lengthen the note; negative values shorten it.
- Variation sprinkles random spread across note lengths. Positive values shorten the note, while negative values lengthen it. Set to anything other than 0%, it brews up fresh note length variation each time you reapply the Transformation.

With Legato, each selected note grows until it reaches the start time of the note that follows. The final selected note runs to the close of the time selection or, where there is none, to the end of the loop.

Notes Before and After Applying Legato.

Tenuto leaves the original note length intact unless you touch the Offset and Variation parameters.

Under the Staccato articulation type, note length follows from the spacing between the selected notes’ start times. The tightest gap between start times is cut in half, and that span becomes the new note length for the transformed notes. From there, the Offset and Variation parameters let you tweak note length further.
