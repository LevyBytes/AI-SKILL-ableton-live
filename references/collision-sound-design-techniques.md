# Collision Sound Design Techniques

Open when you need guidance on Collision Sound Design Techniques in Ableton Live.

Context: [Collision](analog-and-collision-routes.md#302-collision).

<a id="source-3027-sound-design-tips"></a>
### 30.2.7 Sound Design Tips

Even though Collision was built to emulate how real-world objects behave, keep in mind that these emulations permit far greater latitude than the physical originals ever could. Collision is capable of strikingly lifelike renderings of standard mallet instruments — marimbas, vibraphones, and glockenspiels — yet it is equally simple to “misuse“ its controls to conjure tones no acoustic instrument could ever yield.

When aiming for lifelike instrument emulations, it pays to picture the sequence of happenings that creates a sound on a mallet instrument (take a marimba), then map each happening onto a corresponding part of Collision:

- A striker (Mallet) makes contact with a pitched bar (Resonator 1).
- That bar’s resonance gets boosted through a resonating tube (Resonator 2).

So the standard arrangement pairs the Mallet Exciter with the two resonators wired serially (1 > 2).

And naturally, when chasing _unrealistic_ tones, all bets are off:

- Reach for the Noise Exciter, especially alongside drawn-out envelopes, to build washy, near-granular textures. The same controls can mimic unusual acoustic phenomena such as bowed vibraphones or singing crystal glasses.
- Try wiring the resonators in the parallel (1 + 2) arrangement.
- Bring in the LFOs and MIDI controllers (MPE-capable ones included) to drive Collision’s controls.

_A word of caution_: in numerous respects Collision’s models are idealized stand-ins for real objects. As a result, it is all too simple to dial in resonances far touchier to input than any real-world resonator. Some parameter pairings can trigger sharp swings in loudness. Keep output low while you audition fresh sounds.
