# Random Scale And Velocity

Open when you need guidance on Random Scale And Velocity in Ableton Live.

Context: [Live MIDI Effect Reference](live-midi-effect-reference.md#29-live-midi-effect-reference).

<a id="source-296-random"></a>
### 29.6 Random

The Random Effect.

Random injects an element of surprise into note sequences by scrambling the pitch of incoming notes.

How probable it is that an incoming note's pitch gets randomly shifted is governed by the Chance control. Think of it as a dry/wet knob for randomness.

Two settings — the Choices and Interval controls — together produce the random number that drives the pitch shift. The Choices control sets how many pitches are possible, from 1 to 24. The Interval control sets how many intervals can sit between those pitches. Multiply the two values together to get the full span of possible pitches measured against the incoming note.

Take Chance at 50%, Choices at 1, and Interval at 12: hitting C3 over and over sends half the notes to C3 and half to C4, in no set order. Flip the Choices and Interval figures so Choices is 12 and Interval is 1, and half the notes land on C3 while the rest land on anything from C#3 up to C4. Both examples assume Mode is on Random and Sign is on Add, which are the defaults.

Mode dictates how the scrambling plays out: Random hands out pitches in no set order, whereas Alt walks through them in a fixed round-robin sequence. Chance acts differently here: at 100%, the upcoming output note is always the next one in line, and at 0%, the upcoming output note is always the incoming note.

For instance, with Chance at 100%, Choices at 12, and Interval at 1, your first C3 sounds as C3, and each C3 after climbs another semitone up to C4, where it loops back to C3. With Chance at 100% and both Choices and Interval at 2, repeated C3s flip between C3 and D3. That's perfect for mimicking upbow and downbow on strings, or trading off right- and left-hand drum hits.

How random pitches sit against the incoming note is set by Sign:

- Add yields random pitches above the original note.
- Sub yields random pitches below the original note.
- Bi yields random pitches that may sit above or below the original note.

To the right of the Chance control, a set of LEDs reports how random pitches are being placed:

- The + LED flashes when a pitch over the original note appears.
- The 0 LED flashes when the pitch is left as is.
- The - LED flashes when a pitch under the original note appears.

Switch on the Use Current Scale toggle in the device title bar to lock randomly generated pitches to the clip's scale. That keeps the outputs inside a chosen harmonic range. Pairing Random's Alt mode with a set scale lets you build something like a basic but surprising step sequencer.

<a id="source-297-scale"></a>
### 29.7 Scale

The Scale Effect.

Scale rewrites notes according to a chosen scale. A matrix gives each incoming note an outgoing counterpart. So you could, say, turn every incoming C into a D.

A 13x13 grid forms the Note Matrix, with each row and column standing for the 12 notes of a full octave. Columns hold incoming note values, and rows display the outgoing counterparts.

Keys colored black on a keyboard match the black squares. How each note maps under the chosen scale is shown by the highlighted squares. Mapping starts at the root note, which sits in the Note Matrix's lower-left corner. The Base chooser sets the root note, and the Scale Name chooser picks the scale. You can instead switch on the Use Current Scale toggle in the device title bar to adopt the clip's root note and scale. With that on, the Base and Scale Name choosers go inactive, since the clip now sets those.

Pick User from the Scale Name chooser to build a scale of your own. To begin with, each highlighted square maps to its matching note inside an octave — C gives C, C# gives C#, and so forth. Drag highlighted squares with the mouse, or remove them by clicking, to shape which notes the scale keeps. Drop a note from the Note Matrix and it stops sounding, even when played.

The Transpose slider lifts or lowers incoming MIDI notes by up to ±36 semitones. You might, say, move a tune in C major into G major by putting Transpose at +7 st.

Once the Scale Name is on User, you can switch on the Fold switch to fold notes automatically when they sit more than six semitones from the original. If an incoming C3 maps out to an A3, for instance, turning on Fold sends C3 to A2 instead.

The reach of the scale mapping is set by the Lowest and Range controls. Every octave is covered by default, but you can narrow the reach to creatively rework a few notes while sparing the others. Say Lowest is C2 and Range is +36: under a C major scale, only C2 through B4 get remapped. Combine these with the Transpose parameter to confine transposition to one stretch of notes. Keeping the same settings as the example, you could put the Transpose control at +7 st so only the notes from C2 to B4 shift while the rest sit untouched.

<a id="source-298-velocity"></a>
### 29.8 Velocity

The Velocity Effect.

Velocity reshapes the velocity values (1-127) of incoming MIDI notes so their outgoing values land inside a chosen range.

The Velocity Curve grid plots how incoming velocities sitting inside the range fixed by the Range and Lowest controls (X-axis) get remapped onto the range fixed by the Out Hi and Out Low controls (Y-axis). How the velocity values change is defined by the resulting curve.

You might, say, put Out Low at 80 and Out High at 127 to force every outgoing velocity into a louder range, even where the originals were played gently. Be aware that with Lowest and Out Low at zero plus Range and Out Hi at 127, the effect basically passes through, since all incoming velocity values come out in much the same range.

Through the Operation chooser you can remap velocity for MIDI Note On (Velocity), Note Off (Rel. Vel.), or both at once.

To decide how incoming velocities outside the range fixed by the Range and Lowest controls get handled, pick one of the Mode toggles:

- With Clip mode, incoming velocities are pinned so they stay inside the range.
- With Gate mode, incoming velocities beyond the range are dropped entirely. The LED under the Velocity Curve grid flashes whenever the gate blocks a note.
- With Fixed mode, the Out Hi value becomes every outgoing velocity, no matter what came in.

Random lays random modulation across all incoming velocities. How wide that modulation runs depends on the value you set and is shaped by the Output Range controls. With Out Hi at 127 and Out Low at 60, for example, a Random value of 50 nudges velocities up or down by as much as 50 inside the 60-127 range.

Set Random to a positive value and a grey-shaded zone shows up around the velocity curve, signaling that the velocities fall under the chosen random spread.

A more elaborate velocity curve can be sculpted with the Drive and Compand controls. Drive drives every value in the curve toward the far extremes; Compand can stretch out or pull in the values within the curve's bounds.

Positive Drive settings push velocities into the top of the range so most notes hit hard, while negative settings push them into the bottom so most notes play quietly.

Positive Compand settings stretch incoming velocities toward the curve's outer edge, driving the outgoing values toward the high or low extremes. Negative Compand settings pull outgoing velocities in toward the middle.

These two can be worked on their own or in tandem to further carve the velocity curve, yielding a more shaped result inside the broad range.
