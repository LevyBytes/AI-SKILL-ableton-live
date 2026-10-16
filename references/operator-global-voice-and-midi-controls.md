# Operator Global Voice And MIDI Controls

Open when you need guidance on Operator Global Voice And MIDI Controls in Ableton Live.

Context: [Global Controls](meld-and-operator-routes.md#3096-global-controls).

<a id="source-3096-global-controls"></a>
### 30.9.6 Global Controls

Operator’s Global Display and Shell Parameters.

Housed in the global section are the parameters that steer Operator’s overall behavior. On top of that, the global display area lays out a full complement of modulation routing controls.

<a id="source-live-instrument-reference-part-6"></a>

How many Operator voices (notes) may sound at once is governed by the Voices parameter, found in the global display. In an ideal world you would keep this value high enough that nothing ever gets cut while you perform, yet for the sake of CPU headroom a range from 6 to 12 tends to be more practical. Up to 32 voices of polyphony are available in Operator.

Tip: Certain timbres are inherently monophonic and ought to occupy just one voice — a flute being the classic illustration. For such patches, dial Voices down to 1. Choosing a value of 1 for Voices brings a second consequence as well: voices that overlap will sound legato, so the envelopes carry over from one note to the next without retriggering, and pitch alone shifts.

The shell's global section houses a master Volume control for the instrument, while the display within that global section holds a Pan control. Note pitch or a random amount can modulate Pan, by way of the neighbouring Pan < Key and Pan < Rnd controls, in turn.

A broad assortment of internal MIDI mappings is offered from the middle of the global display. Each of the MIDI controllers Velocity, Key, Aftertouch, Pitch Bend and Mod Wheel may drive two destinations, and the Amount sliders set a separate modulation depth for each. Keep in mind that Time < Key and pitch bend range come with fixed assignments, even though both of those sources can additionally feed a further target. To read more about the modulation choices on offer, consult the [complete parameter list](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#the-complete-parameter-list).
