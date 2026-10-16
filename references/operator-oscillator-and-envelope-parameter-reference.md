# Operator Oscillator And Envelope Parameter Reference

Open when you need guidance on Operator Oscillator And Envelope Parameter Reference in Ableton Live.

Context: [The Complete Parameter List](operator-and-sampler-routes.md#30910-the-complete-parameter-list).

<a id="source-309106-oscillators-a-d-shell-and-display"></a>
#### 30.9.10.6 Oscillators A-D Shell and Display

Osc On — Switches the oscillator on or off.

Osc Coarse Frequency (Coarse) — How oscillator frequency relates to note pitch is governed by the Coarse and Fine parameters. Coarse fixes that ratio in whole numbers, yielding a harmonic relationship.

Osc Fine Frequency (Fine) — How oscillator frequency relates to note pitch is governed by the Coarse and Fine parameters. Fine fixes that ratio in fractions of whole numbers, yielding an inharmonic relationship.

Osc Fixed Frequency On (Fixed) — Under Fixed Mode, oscillators ignore note pitch and hold a fixed frequency instead.

Osc Fixed Frequency (Freq) — The oscillator's frequency expressed in Hertz. It stays constant no matter the note pitch.

Osc Fixed Multiplier (Multi) — Serves to scale the range of the fixed frequency. Take this value times the oscillator’s Freq knob value to arrive at the true frequency in Hz.

Osc Output Level (Level) — Sets the oscillator's output level. When that oscillator modulates another, its level weighs heavily on the resulting timbre. Higher levels tend to yield bright and/or noisy sounds.

Envelope / Oscillator Switches — These switches flip the display between the oscillator’s envelope and its harmonics editor.

16/32/64 — These switches determine how many partials are open to user editing.

Osc Waveform (Wave) — Pick from an assortment of thoughtfully chosen waveforms. They can then be edited through the harmonics editor.

Osc Feedback (Feedback) — An oscillator is able to modulate itself provided no other oscillator is modulating it. That modulation hinges not only on the feedback control's setting but also on the oscillator level and the envelope. More feedback yields a more intricate resulting waveform.

Osc Phase (Phase) — Fixes the oscillator's starting phase. The available span covers one complete cycle.

Retrigger (R) — With this on, the oscillator jumps back to the identical phase position whenever a note fires. With R off, the oscillator keeps running freely.

Repeat — Repeating the drawn partials with a progressive fadeout can manufacture higher harmonics, governed by what's chosen in the Repeat chooser. Low Repeat settings yield a brighter tone, while higher ones bring more high-end roll-off and a stronger fundamental. With Repeat off, any partials beyond the 16th, 32nd or 64th harmonic get cut.

Osc Frequency < Velocity (Osc < Vel) — Note velocity can modulate an oscillator's frequency. Positive values push the oscillator’s pitch up as velocity grows, and negative values pull it down.

Osc Freq < Vel Quantized (Q) — Lets you quantize the result of the Frequency < Velocity parameter. When active, the audible outcome equals manually altering the Coarse parameter for every note.

Volume Envelope Rates < Velocity (Time < Vel) — This control is present for the filter, pitch, LFO and volume envelopes alike. For that reason it is documented in the section on envelopes.

Osc Output Level < Velocity (Vel) — Sets the degree to which note velocity governs the oscillator’s level. Applied to modulating oscillators, this produces velocity-dependent timbres.

Osc Output Level < Key (Key) — Sets the degree to which note pitch governs the oscillator’s level. C3 serves as the center point for this function.

<a id="source-309107-envelope-display"></a>
#### 30.9.10.7 Envelope Display

Envelope Attack Time (Attack) — Sets how long a note takes to climb from the initial level up to the peak level. With the oscillator envelopes, this envelope segment is linear in shape. With the filter and pitch envelopes, the segment's shape is adjustable.

Envelope Decay Time (Decay) — Sets how long a note takes to fall from the peak level to the sustain level. With the oscillator envelopes, this envelope segment is exponential in shape. With the filter and pitch envelopes, the segment's shape is adjustable.

Envelope Release Time (Release) — How long a note takes to arrive at the end level once a Note Off message comes in. For the oscillator envelopes this level is fixed at -inf dB and the segment is exponential in shape. For the filter and pitch envelopes the End Level parameter sets the end level and the segment's shape is adjustable. Whatever segment happens to be running, this release segment commences from the envelope's value at the instant the Note Off message arrives.

Envelope Initial Level (Initial) — Sets the envelope's starting value.

Envelope Peak Level (Peak) — The high point reached when the note attack finishes.

Envelope Sustain Level (Sustain) — The level held once the note decay finishes. The envelope rests here until note release, except when it is in Loop, Sync or Beat Mode.

Envelope End Level (End) — (LFO, Filter and pitch envelopes only) The level arrived at when the Release stage ends.

Envelope Loop Mode (Loop) — Set to Loop, the envelope restarts once the decay segment ends. Set to Beat or Sync, it restarts after a specified beat-time. Under Sync Mode this restart is quantized to song time. Under Trigger mode the envelope disregards Note Off.

Envelope Beat/Sync Rate (Repeat) — As long as it remains on, the envelope is retriggered after this span of beat-time. On retriggering, the envelope climbs at the chosen attack rate from wherever it is up to the peak level.

Envelope Loop Time (Time) — Should a note linger past the close of the decay/sustain segment, the envelope restarts from its initial value. This parameter sets how long the journey from the sustain level back to the initial value takes.

Envelope Rates < Velocity (Time < Vel) — This setting determines how much note velocity modulates the envelope segments. It becomes particularly intriguing when the envelopes loop. Note that this modulation leaves the beat-time in Beat or Sync Modes untouched, acting instead on the envelope segments themselves.

The filter and pitch envelopes additionally supply controls for tilting the slope of their envelope segments. With positive slope values the envelope dashes ahead at the start and eases off afterward. With negative slope values the envelope holds flat for a stretch and then accelerates toward the close. At a slope of zero the response is linear, the envelope advancing at a steady rate across the whole segment.

Attack Slope (A.Slope) — Shapes the Attack envelope segment.

Decay Slope (D.Slope) — Shapes the Decay envelope segment.

Release Slope (R.Slope) — Shapes the Release envelope segment.

<a id="source-309108-context-menu-options-for-operator"></a>
#### 30.9.10.8 Context Menu Options for Operator

A few of Operator's operations and parameters can be reached solely through the context menu. They comprise:

Copy commands for Oscillators — Within the context menu of the oscillator’s shell and envelope display you'll find options for copying parameters from one oscillator to another.

Envelope commands — Within the context menu of every envelope display you'll find options that swiftly drive all envelope levels to their maximum, minimum, or middle values.

Harmonics editor commands — The harmonics editor's context menu can confine partial drawing to even or odd harmonics and switch normalization of an oscillator’s output level on or off. A command for exporting the waveform as an .ams file is present as well.

Play By Key — Found in the context menu of the filter’s Freq control, this command tunes the filter for key tracking by placing the cutoff at 466 Hz and the Freq < Key at 100%.

Enable Per-Note Pitch Bend — This is switched on by default, letting Operator react to per-note pitch bend changes. Should you wish, you can turn the behaviour off by clearing the option in the context menu of the device title bar.
