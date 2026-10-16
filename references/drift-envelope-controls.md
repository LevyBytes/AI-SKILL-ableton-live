# Drift Envelope Controls

Open when you need guidance on Drift Envelope Controls in Ableton Live.

Context: [Envelopes Section](collision-and-drift-routes.md#3034-envelopes-section).

<a id="source-30341-envelope-1"></a>
#### 30.3.4.1 Envelope 1

How the Oscillator section’s output amplitude (taking in both oscillators plus the Noise generator when active) starts and evolves once a note begins and then ends is governed by Envelope 1.

The Attack, Decay, Sustain, and Release controls can be set via their knobs or by reshaping the envelope right in the display.

_Attack_ fixes the span needed to climb from the starting value up to the peak value.

_Decay_ fixes the span needed to fall from the peak value down to the Sustain level.

_Sustain_ fixes the level held once the Decay stage closes; the envelope stays there until the note finishes.

_Release_ fixes the span needed to drop back to zero after the note ends.

Switching between Envelope 1 and Envelope 2 happens by clicking the matching section in the UI or by using the _1_ and _2_ toggles within the display. Whichever envelope is active appears in the display ready to edit.

<a id="source-30342-envelope-2"></a>
#### 30.3.4.2 Envelope 2

Attack, Decay, Sustain, and Release controls belong to Envelope 2 as well; unlike Envelope 1 though, Envelope 2 is not tied to amplitude by default and can serve as a source for every modulation source slot inside Drift.

Flipping the switch to the left of the Attack control converts Envelope 2 from an ADSR envelope into a Cycling Envelope.

Cycling Envelope.

What the Cycling Envelope behaves like is an LFO modulation that relaunches with every arriving MIDI note.

The envelope’s midpoint is shifted by the Tilt knob, and at very low or very high settings it can also reshape the envelope’s slopes. How long the envelope sits at its peak is fixed by the Hold control.

Out of the box, the Cycling Envelope shows the Rate control, one of four available time modes alongside Ratio, Time, and Sync. Click the switches beside the control to choose another. According to the time mode, the cycle rate is set in Hz, ratio, milliseconds, or tempo-synced beat divisions.
