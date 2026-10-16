# Collision LFO MIDI And MPE

Open when you need guidance on Collision LFO MIDI And MPE in Ableton Live.

Context: [Collision](analog-and-collision-routes.md#302-collision).

<a id="source-3025-lfo-tab"></a>
### 30.2.5 LFO Tab

Collision’s LFOs.

Serving as modulators for an array of mallet, noise, and resonator parameters — picked in the Destination choosers — are Collision’s two standalone LFOs. They are also able to modulate one another.

Flipping each LFO on or off are the LFO 1 and LFO 2 switches, with the wave shape itself picked through the waveform chooser. On offer are sine, square, triangle, sawtooth up, sawtooth down and a couple of noise variants. One noise variant jumps between random levels; the other glides smoothly between them.

Phase offset for the LFO is set by the Offs. slider. With Retrigger active, playing a note relaunches the LFO at the waveform phase fixed by the Offset parameter.

Two targets per LFO can be modulated, each chosen in the Destination choosers. How intense each modulation is gets set with the LFO Destination Amount sliders. Bear in mind these depths are scaled relative to the LFO’s own Amount value.

Speed of the LFO is governed by Rate, expressed either in Hertz or as tempo-synced beat divisions. Overall LFO intensity comes from the Amount knob. On the MIDI tab, note pitch can drive Rate and velocity can drive Amount.

<a id="source-3026-midimpe-tab"></a>
### 30.2.6 MIDI/MPE Tab

Collision’s MIDI/MPE Tab.

A broad set of internal MIDI assignments is opened up by the MIDI/MPE tab, serving both ordinary and MPE-capable MIDI controllers. The pitch bend (per-note pitch bend included), modulation wheel, pressure, and slide from a MIDI controller can each feed two destinations, with separate depths fixed by the Amount sliders.

Pitch or velocity, by way of the Key and Vel sliders, can drive further mallet, noise, resonator, and LFO parameters.
