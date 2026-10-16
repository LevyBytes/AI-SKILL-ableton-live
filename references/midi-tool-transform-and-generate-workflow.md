# MIDI Tool Transform And Generate Workflow

Open when you need guidance on MIDI Tool Transform And Generate Workflow in Ableton Live.

Context: [MIDI Tools](midi-tools.md#11-midi-tools).

<a id="source-111-using-midi-tools"></a>
### 11.1 Using MIDI Tools

To put a MIDI Tool to work transforming or generating notes, bring up the Transform or Generate panel, pick a tool from the Transformation/Generator Selector chooser, and adjust the controls inside the chosen MIDI Tool’s interface. Every MIDI Tool ships with the Auto Apply button switched on out of the box. With it active, your edits to a MIDI Tool’s settings transform or generate MIDI notes the moment you make them.

The Auto Apply Button.

From then on, every tweak you make to a MIDI Tool’s parameters shows up in the MIDI Note Editor without delay. Should you prefer that the Transformations and Generators not act right away, switch the Auto Apply button off. Bear in mind that flipping this button off returns the notes to how they started.

Once the Auto Apply button is off, take your time dialing in a MIDI Tool’s parameters; when the settings feel right, hit the Apply button so the changes are committed.

The Apply Button.

There’s also a way to apply whichever MIDI Tool is selected without stepping out of the MIDI Note Editor — just press Ctrl+Enter (Win) / Cmd+Enter (Mac).

Whenever you run a Transformation, it targets the time selection, the note selection, or the clip loop (in cases where neither a time nor a note selection exists). Running a Transformation swaps the original notes out for the transformed ones.

A Generator, meanwhile, targets the time selection or, lacking one, the clip loop. Should notes already be sitting in the MIDI Note Editor as a Generator runs, the new notes will either join the current material (when the old and new notes steer clear of each other) or take its place (when the existing and generated notes overlap).

Because MIDI Tools respect scale, enabling a scale on a clip causes every pitch-related parameter across the MIDI Tools to read in scale degrees rather than semitones.

Whatever transforming or generating you do to notes is reversible through the Undo and Redo commands in the Edit menu. Keep in mind that those commands touch only the edits made to MIDI notes, leaving any changes to a MIDI Tool’s parameters untouched. To send the parameters back to how they began, use the Reset button, which dims out the moment the MIDI Tool returns to default.

An Active Reset Button.

Bear in mind the Reset button reaches only the parameters of the chosen MIDI Tool; the MIDI notes themselves are left alone.
