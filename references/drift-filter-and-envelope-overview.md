# Drift Filter And Envelope Overview

Open when you need guidance on Drift Filter And Envelope Overview in Ableton Live.

Context: [Drift](collision-and-drift-routes.md#303-drift).

<a id="source-3033-filter-section"></a>
### 30.3.3 Filter Section

Drift’s Filter Section.

A major part of carving the oscillators’ timbres falls to filtering.

Drift’s Filter section provides a low-pass filter switchable between two types, filter key tracking, a resonance control, a high-pass filter, and a pair of frequency modulation controls.

Cutoff for the low-pass filter is set by the Freq knob. The Type toggle moves between a couple of separate low–pass options: Type I (12 dB/octave) alongside Type II (24 dB/octave).

Type I relies on a DFM-1 filter that recirculates more of its own distortion, spanning a wide tonal range from gentle filter sweeps to warm drive.

Type II carries the Cytomic MS2 filter, built on a Sallen-Key topology with soft clipping to rein in resonance.

How strongly the pitch of arriving MIDI notes steers the low-pass filter’s frequency is set by the Key slider. At a value of 0.00, MIDI notes leave filter frequency untouched. At 1.00, low notes pull the filter frequency down and high notes push it up.

Resonance of the low-pass filter is set by the Res knob, and cutoff for the high-pass filter is set by the HP knob.

You may also click anywhere within the Filter section to reach and edit the envelope through the Envelopes section display via an X-Y controller. Drag the left filter dot side to side to fix the high-pass frequency. Drag the right filter dot side to side for the low-pass frequency or up and down for the resonance amount.

For the low-pass filter cutoff, up to two modulation sources are pickable through the Low-pass Modulation Source drop-downs inside the Freq Mod section. How strongly each source drives the frequency, anywhere from -100% to 100%, is fixed by the Low-pass Modulation Amount sliders.

<a id="source-3034-envelopes-section"></a>
### 30.3.4 Envelopes Section

Drift’s Envelopes Section.

In general, envelopes dictate the way a sound’s amplitude evolves from the instant a note begins until it stops.

A pair of standalone envelopes lives in Drift’s Envelopes section: one governing how amplitude changes and a second meant purely for modulation.
