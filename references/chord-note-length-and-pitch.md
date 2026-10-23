# Chord Note Length And Pitch

Open when you need guidance on Chord Note Length And Pitch in Ableton Live.

Context: [Live MIDI Effect Reference](live-midi-effect-reference.md#29-live-midi-effect-reference).

<a id="source-293-chord"></a>
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

<a id="source-294-note-length"></a>
### 29.4 Note Length

The Note Length Effect.

Note Length reshapes how long incoming MIDI notes last. It can also fire notes off MIDI Note Off messages rather than the customary Note On messages.

Whether the device fires on Note On or Note Off messages is decided by the Trigger Source toggle. With Note On selected, the Gate and Length controls govern how long incoming notes run. The Gate control sets how the Length control's value gets applied. At 100%, notes run for the full span the Length control specifies. Gate at 200% doubles that span, while 50% cuts it in half. The Time Mode toggles let you express the length in milliseconds or tempo-synced beat divisions.

When the device fires from a Note Off event (the instant a note is let go), an incoming note's timing is pushed back by its own length — so it begins right when it would have ended under Note On triggering. After that opening delay passes, the Gate and Length controls take over the timing.

Working with Note Off messages unlocks three extra parameters:

- Release Velocity: Sets the output note's velocity. The percentage strikes a balance between the incoming note's Note On and Note Off velocities. Should your keyboard lack MIDI Note Off velocity, this can stay at 0%.
- Decay Time: Sets how long an incoming note's velocity needs to fall to zero. Decay kicks off the moment the device gets a Note On message. Whatever value stands at the Note Off point becomes the output note's velocity.
- Key Scale: Changes output-note length according to the incoming notes' pitch. With positive settings, notes under C3 grow gradually longer while notes over C3 shorten. Negative settings flip that around.

Switching on the Latch toggle turns on note latching. Under Note On messages, a triggered note keeps sounding until the next Note On arrives. Under Note Off messages, notes fire once every key (or a connected sustain pedal) is released and a new Note Off message comes in. Either way, the Gate and Length controls go inactive, because the Note On/Off messages now dictate triggered-note length. On top of that, the Release Velocity, Decay Time, and Key Scale controls switch off for Note Off messages.

<a id="source-295-pitch"></a>
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
