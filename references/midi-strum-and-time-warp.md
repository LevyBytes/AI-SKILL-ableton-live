# MIDI Strum And Time Warp

Open when you need guidance on MIDI Strum And Time Warp in Ableton Live.

Context: [Transformation Tools](midi-tools.md#112-transformation-tools).

<a id="source-11210-strum"></a>
### 11.2.10 Strum

Following a shape laid out by the Strum Low, Strum High and Tension parameters, the Strum MIDI Tool nudges the start times of the notes within a chord.

The Strum Transformation.

Working from the lowest note upward, the Strum Low parameter sets how far the successive notes are offset. Positive values push the note start times earlier, while negative values pull them back. At 100% / -100% the lowest note’s start time shifts by as much as one grid step. The remaining notes follow proportionally, tracing the shape shown in the Strum Position display. Should the Tension parameter sit at 0.0%, the notes spread out at equal spacing from one another.

Starting instead from the highest note, the Strum High parameter governs the offset across the original chord. Positive values move the note start times earlier, and negative values move them back. At 100% / -100% the highest note shifts by up to a grid step. The other notes spread proportionally to mirror the shape in the display. With the Tension parameter at 0.0%, the notes land at even spacing between each other.

For the Transformation to do anything, the Strum Low and/or Strum High parameters have to hold a value other than 0.0%. You can alter either parameter by dragging its breakpoint in the Strum Position display, or by typing a value for each on your computer keyboard.

What the Tension parameter does is reshape the offset of note start times so they stop sitting at uniform spacing and instead trace a curve, with the gaps between notes widening or narrowing according to the setting. Positive Tension values make the gap between notes widest at the start of the sequence before it tapers off exponentially. Negative values make the gap narrow at the start of the sequence and then grow exponentially.

Notes Before and After Applying the Strum Transformation.

<a id="source-11211-time-warp"></a>
### 11.2.11 Time Warp

A time-stretching MIDI Tool, Time Warp reworks selected notes by following a speed curve, which opens the door to tempo shifts like accelerando or ritardando.

The Time Warp Transformation.

The speed curve is something you build inside the Breakpoints display, where the curve’s time range lines up with the time selection. Using their individual toggles, you can turn on anywhere from one to three breakpoints along the speed curve. To position a breakpoint, either drag it in the display or select it and reach for the Breakpoint Time and Breakpoint Speed sliders, which set its timeline position and speed in turn. Whatever the sliders read always mirrors the breakpoint you currently have selected.

<a id="source-midi-tools-part-2"></a>

Sitting beneath the Breakpoints display, the toggles give you extra control over how the time-warping behaves. With Quantize active, notes that have been warped snap to the current grid settings. Switching on Preserve Time Range keeps the output of the Transformation confined to the span occupied by the notes you originally selected. Turning on Include Note End factors each original note's ending position into the speed curve calculation, so the lengths of those notes can change as a result.

How notes look once Time Warp has been applied, compared with before.
