# Arpeggiator And CC Control

Open when you need guidance on Arpeggiator And CC Control in Ableton Live.

Context: [Live MIDI Effect Reference](live-midi-effect-reference.md#29-live-midi-effect-reference).

<a id="source-291-arpeggiator"></a>
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

<a id="source-292-cc-control"></a>
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
