# Live Midi Effect Reference

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 29. Live MIDI Effect Reference

Bundled with Live is an assortment of purpose-built MIDI effects. Each one can reshape the pitch, length, and velocity of incoming MIDI in different ways. A single MIDI effect can liven up a pattern on its own, or you can chain several of them together to build more intricate note sequences.

Scale awareness is available on every MIDI effect that exposes pitch controls. With the Use Current Scale toggle active in the device title bar, controls tied to pitch let you work in scale degrees rather than semitones. The benefit is that every note you shift remains inside a chosen harmonic range.

For a primer on how effects work in Live, see the [Working with Instruments and Effects](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects) chapter.

### 29.1 Arpeggiator

The Arpeggiator Effect.

Starting from a chord or even just one note, Arpeggiator builds rhythmic figures. It packs in the usual arpeggiator tools alongside a few distinctive ones.

You will hear arpeggiators all over 80s synth records, where they were a staple. The term traces back to the arpeggio, a musical idea in which a chord's notes sound one after another instead of together. The word itself comes from the Italian “arpeggiare,” meaning to play notes on a harp.

Which order the notes follow in the rhythm is governed by the Style chooser. Picking a style brings up a picture of its pattern in the display. To step through the available patterns, use the Previous Style Pattern and Next Style Pattern buttons shown there.

You'll find many familiar arpeggiator styles here, including Up, Down, Converge, and Diverge. A few less common ones are also on offer:

- Play Order sorts the notes by the sequence in which you played them. Because of this, the effect only becomes apparent once you've entered more than a single chord or note.
- Chord Trigger plays back the notes you fed in stacked together as a chord.

On top of those, three styles handle random arpeggios:

- Random keeps producing an ever-changing scramble of the MIDI notes coming in.
- Random Other builds random figures from the incoming MIDI notes, yet holds off on repeating any one note until every other incoming note has appeared.
- Random Once derives a single random figure from the incoming MIDI notes and loops it; once the incoming MIDI shifts, it draws up a fresh pattern.

How fast the arpeggiated figure runs is governed by the Rate control, which counts in either milliseconds or tempo-synced beat divisions, depending on the Sync/Free Rate toggle setting.

The Distance and Steps controls let you transpose the figure. Distance fixes the amount of transposition in semitones or scale degrees, and Steps decides how often the figure gets transposed. It first sounds at its starting pitch, then climbs through higher transpositions for positive Distance settings or descends for negative ones. As an example, with Distance at +12 st and Steps at 2, a figure beginning on C3 sounds first at C3, next at C4, and lastly at C5.

If you'd rather transpose inside a chosen scale, dial in the Root and Scale choosers. The figure can also follow the clip's scale once you switch on the Use Current Scale toggle in the device title bar. Doing so greys out the Root and Scale choosers, since the clip now governs those values.

Note length within the figure, expressed as a share of the Rate value, is set by the Gate control. Push Gate past 100% and the notes start to overlap, giving a legato result.

If you're feeding notes from a MIDI controller, flipping on the Hold switch keeps the figure looping even after you let go of the keys. It repeats until you strike another key. You can grab a starting batch of keys and then add notes to the running figure by pressing more. Playing a note again removes it. That lets you slowly grow and reshuffle the figure as it plays.

By shifting the note sequence a chosen number of steps, the Pattern Offset control rearranges where the figure begins. Picture the notes laid out on a circle played clockwise from a fixed point — Pattern Offset spins that circle counterclockwise one note per increment, moving the starting note. With the offset at 1, for instance, the figure's second note now leads and what used to be first is pushed to the end.

To add swing, pick a groove from the Groove chooser. The way grooves behave in Arpeggiator mirrors how they work on clips. How strongly the groove bites is governed by the Global Groove Amount slider, found in the [Groove Pool](https://www.ableton.com/en/live-manual/12/using-grooves/#groove-pool) or the Control Bar.

Depending on which Retrigger option you pick, the figure can restart at chosen points:

- Off — The figure never restarts.
- Note — A fresh incoming note restarts the figure.
- Beat — The figure restarts on a chosen bar or beat, governed by the Interval control.

Each restart of the figure is signaled by the LED beside the Retrigger controls flashing.

How many passes the figure makes is set by the Repeats control. Out of the box, Repeats sits at ∞, so the figure loops without stopping. Dropping Repeats to 1 or 2 can mimic a guitar strum, for instance. Pairing assorted Repeats amounts with different Retrigger choices also lets you build rhythm-driven arpeggios broken up by gaps.

Switching on the Velocity toggle opens the figure's velocity controls. Decay fixes how long it takes to arrive at the velocity set by the Target control. A lengthy Decay paired with Target at 0, for example, yields a slow fade-out.

With the Retrigger switch on, the velocity slope restarts every time the figure does. Pairing velocity with Beat retriggering injects rhythmic movement into the figure's velocity slope.

### 29.2 CC Control

The CC Control Effect.

With CC Control you can dispatch MIDI CC messages out to hardware. It offers three fixed control knobs (Mod Wheel, Pitch Bend, Pressure), a single customizable button for firing off on/off or minimum/maximum values (Custom A), plus twelve customizable control dials (Custom B - M).

Here is what each of the device's fixed control knobs does:

_Mod Wheel_ – Fixes how much modulation the receiving device applies.

_Pitch Bend_ – Pushes pitch bend data out to the receiving device. The range moves downward for negative values and upward for positive ones.

_Pressure_ – Fixes how much channel pressure/aftertouch the receiving device applies.

Toggling the Custom A button on or off switches it between on/off or minimum/maximum values. Although it's meant for sustain/hold pedal messages (CC 64), you can point it at any other MIDI parameter through its CC Type Chooser drop-down menu.

Each of the Custom B - M controls can be given a new name and pointed at any MIDI parameter via that control's CC Type Chooser drop-down menu. The custom names and routings show up on Push and can be stored as presets, which makes them quick to browse and reuse. You can write parameter values into automation lanes or move them live with the device's control dials — handy both when arranging and when improvising in performance.

The device's title bar holds two toggles that flip between controls 1 - 8 and controls 9 - 16, plus a Send button that, when clicked, pushes out every current MIDI CC value. Turning on the Learn toggle lets an incoming MIDI source feed CC data into any customizable control. It's a fast way to tailor the device to your setup. Learn also makes it simple to spot which CC message an outboard controller is transmitting.

Keep in mind that when CC automation is already present for a CC message that CC Control sends to a receiving device, the MIDI data from both sides gets combined.

### 29.3 Chord

The Chord Effect.

True to its name, this effect stacks a chord by taking each incoming note's pitch and layering up to six more pitches on top.

The Shift 1-6 controls let you choose which pitches join the chord, anywhere within ±36 semitones of the original note. Setting Shift 1 to +4 semitones and Shift 2 to +7 semitones, for example, produces a major chord with the incoming note as its root. Order doesn't matter — it's irrelevant which Shift control carries which pitch. Whenever a given note sounds, the LED beside its Shift knob flashes.

Bear in mind that you can't put the same pitch on more than one Shift control. You couldn't, for instance, set both Shift 2 and Shift 3 to +8 st. When a pitch already lives on a Shift control, repeating that pitch elsewhere just switches the extra one off.

Beyond entering pitches by hand, you can switch on the Learn toggle in the device title bar and assign pitches by playing a chord on an outboard MIDI controller. Just hold down the keys you'd like in the chord. The first key you hold sets the root and stays off the Shift controls; everything held after that fills the Shift controls in sequence. Hold extra keys while keeping the first ones down to bring in more pitches. When you've got the pitches you want, switch the Learn toggle off.

With the Velocity or Chance toggle active, the slider beneath each Shift control lets you shape the generated note's dynamics:

- Velocity fixes the velocity of a generated note. It works relatively, spanning 1% to 200%. At 100%, the generated note carries the same velocity as the incoming note. Differing velocities across notes can lend faint overtones or sharply reshape how a chord is balanced.
- Chance fixes how probable it is that a generated note sounds when an incoming note fires. The probability is adjustable anywhere from 0% to 100%. At 100%, every incoming note spawns a note.

Pairing Velocity with Chance is a solid approach for working dynamic movement into a generated chord.

Within a generated chord, the Strum control spaces the notes apart by as much as 400 ms. With positive settings, the strum leads with the original note and then runs through Shift 1 to Shift 6. Negative settings flip that ordering. To stack duplicate notes, head to the context menu of the device title bar and enable its _Play Duplicate Notes When Strumming_ option.

Two further controls are on hand to refine the strumming:

- Tension governs the strum's pace. Positive settings begin the strum slowly and speed it up with every added note, whereas negative settings start it fast and ease it down.
- Crescendo lays a velocity ramp over the strummed notes. An upward ramp comes from positive settings and a downward ramp from negative ones.

Pitches default to semitones, but switching on the Use Current Scale toggle in the device title bar lets you enter them as scale degrees instead.

To push MPE data out to the notes of a generated chord, open the context menu of the device title bar and switch on its _Send Per Note Events to Generated Notes_ option. With scale awareness also active, per-note pitch bend messages track the clip's scale, keeping bent chords inside the intended harmonic range.

### 29.4 Note Length

The Note Length Effect.

Note Length reshapes how long incoming MIDI notes last. It can also fire notes off MIDI Note Off messages rather than the customary Note On messages.

Whether the device fires on Note On or Note Off messages is decided by the Trigger Source toggle. With Note On selected, the Gate and Length controls govern how long incoming notes run. The Gate control sets how the Length control's value gets applied. At 100%, notes run for the full span the Length control specifies. Gate at 200% doubles that span, while 50% cuts it in half. The Time Mode toggles let you express the length in milliseconds or tempo-synced beat divisions.

When the device fires from a Note Off event (the instant a note is let go), an incoming note's timing is pushed back by its own length — so it begins right when it would have ended under Note On triggering. After that opening delay passes, the Gate and Length controls take over the timing.

Working with Note Off messages unlocks three extra parameters:

- Release Velocity — Sets the output note's velocity. The percentage strikes a balance between the incoming note's Note On and Note Off velocities. Should your keyboard lack MIDI Note Off velocity, this can stay at 0%.
- Decay Time — Sets how long an incoming note's velocity needs to fall to zero. Decay kicks off the moment the device gets a Note On message. Whatever value stands at the Note Off point becomes the output note's velocity.
- Key Scale — Changes output-note length according to the incoming notes' pitch. With positive settings, notes under C3 grow gradually longer while notes over C3 shorten. Negative settings flip that around.

Switching on the Latch toggle turns on note latching. Under Note On messages, a triggered note keeps sounding until the next Note On arrives. Under Note Off messages, notes fire once every key (or a connected sustain pedal) is released and a new Note Off message comes in. Either way, the Gate and Length controls go inactive, because the Note On/Off messages now dictate triggered-note length. On top of that, the Release Velocity, Decay Time, and Key Scale controls switch off for Note Off messages.

### 29.5 Pitch

The Pitch Effect.

Pitch shifts incoming MIDI notes by as much as ±128 semitones or ±30 scale degrees.

Use the Pitch control to dial in how far incoming pitches move. Notes shift in semitones by default. Switch on the Use Current Scale toggle in the device's title bar to move them by scale degrees instead.

The Step Up and Step Down buttons nudge the Pitch control value up or down by the amount the Step Width slider specifies. That Step Width amount spans 1 to 48 semitones, or 1 to 30 scale degrees with Use Current Scale on. Every one of these controls accepts [Key and/or MIDI mappings](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) for adjustment on the fly.

The span of pitches permitted through the effect is set by the Lowest and Range controls.

Pick an option from the Mode chooser to decide how notes falling outside the chosen span are handled:

- With Block mode, notes beyond the span can't get through. The LED next to the Range control flashes whenever that occurs.
- With Fold mode, notes beyond the span are shifted to land inside it.
- With Limit mode, notes are held to the span. So any note below the span's lowest note climbs up to it, and any note above the span's highest note drops down to fit.

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

### 29.7 Scale

The Scale Effect.

Scale rewrites notes according to a chosen scale. A matrix gives each incoming note an outgoing counterpart. So you could, say, turn every incoming C into a D.

A 13x13 grid forms the Note Matrix, with each row and column standing for the 12 notes of a full octave. Columns hold incoming note values, and rows display the outgoing counterparts.

Keys colored black on a keyboard match the black squares. How each note maps under the chosen scale is shown by the highlighted squares. Mapping starts at the root note, which sits in the Note Matrix's lower-left corner. The Base chooser sets the root note, and the Scale Name chooser picks the scale. You can instead switch on the Use Current Scale toggle in the device title bar to adopt the clip's root note and scale. With that on, the Base and Scale Name choosers go inactive, since the clip now sets those.

Pick User from the Scale Name chooser to build a scale of your own. To begin with, each highlighted square maps to its matching note inside an octave — C gives C, C# gives C#, and so forth. Drag highlighted squares with the mouse, or remove them by clicking, to shape which notes the scale keeps. Drop a note from the Note Matrix and it stops sounding, even when played.

The Transpose slider lifts or lowers incoming MIDI notes by up to ±36 semitones. You might, say, move a tune in C major into G major by putting Transpose at +7 st.

Once the Scale Name is on User, you can switch on the Fold switch to fold notes automatically when they sit more than six semitones from the original. If an incoming C3 maps out to an A3, for instance, turning on Fold sends C3 to A2 instead.

The reach of the scale mapping is set by the Lowest and Range controls. Every octave is covered by default, but you can narrow the reach to creatively rework a few notes while sparing the others. Say Lowest is C2 and Range is +36: under a C major scale, only C2 through B4 get remapped. Combine these with the Transpose parameter to confine transposition to one stretch of notes. Keeping the same settings as the example, you could put the Transpose control at +7 st so only the notes from C2 to B4 shift while the rest sit untouched.

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
