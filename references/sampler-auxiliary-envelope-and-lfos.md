# Sampler Auxiliary Envelope And LFOs

Open when you need guidance on Sampler Auxiliary Envelope And LFOs in Ableton Live.

Context: [Sampler](operator-and-sampler-routes.md#3010-sampler).

<a id="source-30109-the-modulation-tab"></a>
### 30.10.9 The Modulation Tab

The Modulation Tab.

Within the Modulation tab you get one more loopable envelope alongside three LFOs, every one of them able to modulate several parameters and even one another. An LFO may run freely or lock to the Live Set’s tempo, and stereo modulation effects are possible with LFOs 2 and 3.

<a id="source-301091-the-auxiliary-envelope"></a>
#### 30.10.9.1 The Auxiliary Envelope

Over on the left, the Auxiliary (Aux) envelope behaves a great deal like the Pitch/Osc tab envelopes, supplying Initial, Peak, Sustain and End levels together with ADSR, Loop mode and slope points. You can send this envelope to any of 29 destinations via both the A and B choosers. The depth with which the Auxiliary envelope modulates destinations A and B is dialed in with the pair of sliders to the right.

<a id="source-301092-lfos-1-2-and-3"></a>
#### 30.10.9.2 LFOs 1, 2 and 3

Whatever room is left on the Modulation tab holds three Low Frequency Oscillators (LFOs). True to their name, Sampler’s LFOs work by feeding a low frequency (under 30 Hz) into a parameter so as to modulate it. Activate any oscillator by clicking the LFO 1, LFO 2 or LFO 3 switches.

_Type_: Six waveshapes are on offer for Sampler’s LFOs: Sine, Square, Triangle, Sawtooth Down, Sawtooth Up, and Sample and Hold.

_Rate_: When Hz is chosen, the Freq slider on the right governs the LFO’s speed. When the note head is chosen instead, the LFO locks to beat-time, which you adjust on the Beats slider to the right.

_Freq_: The LFO’s speed expressed in Hertz (cycles per second), tunable from 0.01 to 30 Hz.

_Beats_: Specifies the LFO’s speed in beat-time (64th notes to 8 bars).

_LFO Attack (Attack)_: The interval the LFO requires to climb to full intensity. It lets you, say, ease vibrato in gradually while a note sustains.

_LFO Retrigger (Retrig)_: Switching on Retrigger for an LFO resets it to its origin, the initial phase, with every fresh MIDI note. Retriggering the LFO before it finishes a cycle can yield hybrid LFO contours.

_LFO Offset (Offset)_: This shifts an LFO’s origin, or initial phase, so the oscillator launches from somewhere else in its cycle. Retriggering the LFO before it finishes a cycle can yield hybrid LFO contours.

_LFO Rate < Key (Key)_: Commonly called keyboard tracking, any non-zero setting makes an LFO speed up in line with the pitch of incoming MIDI notes.

LFO 1 carries four sliders for swiftly modulating global parameters:

_Volume (Vol)_: LFO 1 is able to modulate the global volume level. This slider sets the modulation depth across a 0-100 scale.

_Pan (Pan)_: LFO 1 is able to modulate the global pan placement. This slider sets the modulation depth across a 0-100 scale.

_Filter_: LFO 1 is able to modulate the filter cutoff frequency (Freq in the Filter/Global tab). This slider sets the modulation depth across a 0-24 scale.

_Pitch_: LFO 1 is able to modulate the pitch of samples. This slider sets the modulation depth across a 0-100 scale.

_LFO Stereo Mode (Stereo)_: Two flavors of stereo modulation are available from LFOs 2 and 3: _Phase_ or _Spin_. Under phase mode, the left and right LFO channels move at the same speed, and the Phase parameter shifts the right channel away from the left. Under spin mode, the Spin parameter lets the right LFO channel run as much as 50% quicker than the left.

As with the Auxiliary envelope, LFOs 2 and 3 provide A and B choosers through which you can direct the LFOs toward numerous destinations.
