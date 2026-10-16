# MIDI Tools Quantization And Velocity

Open when you need guidance on MIDI Tools Quantization And Velocity in Ableton Live.

Context: [Editing MIDI Notes](editing-midi.md#105-editing-midi-notes).

<a id="source-10510-midi-tools"></a>
### 10.5.10 MIDI Tools

Housed in the Transform and Generate panels, the MIDI Tools open up further avenues for editing MIDI notes. You can rework existing notes through such things as articulation, interpolation, or ornamentation, or you can have brand-new note patterns spun up on the spot from parameters you specify.

A dedicated [MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#midi-tools) chapter walks through every option on hand for transforming and generating notes.

<a id="source-10511-quantizing-notes"></a>
### 10.5.11 Quantizing Notes

Live gives you four routes to quantizing MIDI notes:

1. Quantize notes right as you [record them](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-quantized-midi-notes).
2. Quantize notes by nudging them until they latch onto the grid lines on screen.
3. Quantize notes via the [Quantize MIDI Tool](https://www.ableton.com/en/live-manual/12/midi-tools/#quantize) found in Clip View’s Transform panel, which hands you finer command over how notes are quantized. This transformation lets you pin down an exact value to quantize notes to (note starts and ends can both be quantized). The Amount control even lets you quantize while sidestepping that rigid “quantized” feel, since it shifts notes by only a fraction of the chosen quantization value.
   The Quantize MIDI Tool.
4. Quantize by picking a note or several and reaching for the Quantize command in the Edit menu, or by pressing the Ctrl+U (Win) / Cmd+U (Mac) keyboard shortcut. This route relies on the quantization settings laid out in the Quantize MIDI Tool covered just above. Those same settings open up through the Ctrl+Shift+U (Win) / Cmd+Shift+U (Mac) keyboard shortcut.

<a id="source-10512-editing-velocities"></a>
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
