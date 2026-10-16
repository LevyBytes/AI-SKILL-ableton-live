# MIDI Note Probability Editing

Open when you need guidance on MIDI Note Probability Editing in Ableton Live.

Context: [Editing MIDI Notes](editing-midi.md#105-editing-midi-notes).

<a id="source-10513-editing-probabilities"></a>
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
