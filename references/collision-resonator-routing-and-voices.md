# Collision Resonator Routing And Voices

Open when you need guidance on Collision Resonator Routing And Voices in Ableton Live.

Context: [MIDI/MPE Tab](collision-and-drift-routes.md#3026-midimpe-tab).

<a id="source-30261-the-global-section"></a>
#### 30.2.6.1 The Global Section

Collision’s Global Section.

Parameters tied to how Collision behaves and performs as a whole live in the global section.

How many notes are allowed to ring at once is set by the Voices drop-down.

With Retrig. enabled, a note already sounding is retriggered instead of spawning one more voice. Doing so can conserve CPU.

How signal travels among the resonators is decided by Structure.

Under serial routing 1 > 2, both resonators feed Resonator 1. That output is then summed to mono and passed along to Resonator 2, while also reaching its own mixer (kept in stereo).

Resonators in 1 > 2 (Serial) Configuration.

Under parallel routing 1 + 2, the combined output of the Mallet and Noise sections goes straight to each resonator.

Resonators in 1 + 2 (Parallel) Configuration.

Overall output level is set by Volume.
