# Hybrid Reverb Shimmer Tides And Prism

Open when you need guidance on Hybrid Reverb Shimmer Tides And Prism in Ableton Live.

Context: [Algorithmic Reverb Engine](gate-glue-grain-hybrid-reverb-routes.md#28234-algorithmic-reverb-engine).

<a id="source-282343-shimmer"></a>
#### 28.23.4.3 Shimmer

A tight stack of diffuse delays feeding a pitch shifter in the loop forms the basis of the Shimmer reverb algorithm. At low diffusion you hear a clean delay, whereas cranking diffusion high yields a thick, rich synthetic reverb. By blending the pitch-shifted output back into the feedback path, the Shimmer effect produces tails that drift upward or downward in pitch.

Alongside the common parameters described earlier, Shimmer adds these controls:

- Damping sets how much treble gets rolled off inside the reverb algorithms; turn it up and the resulting reverberation grows darker in tone.
- Mod determines how much motion occurs within the tail produced by the algorithm. Dialing modulation down quiets that motion, whereas raising it introduces a chorus-like sweep and simultaneously softens any resonant buildup.
- Pitch sets, in semitones, how far the feedback signal is shifted up or down.
- Diffusion sets how thick the algorithm’s tail becomes. Lower settings thin the tail out, and as you raise the value the tail grows progressively denser. Drop it under 10% for dub-style delay textures. It’s a blast on drums!
- Shimmer governs how strong the Shimmer effect is. At 0% there is no pitch shifting at all, and the pitched layer grows steadily louder as you push the percentage higher. On melodic parts, dialing Shimmer up to 100% gives you striking harmonized pitches.

When Shimmer mode is active, the Size knob controls the spacing between the separate echoes heard on percussive sources.

<a id="source-282344-tides"></a>
#### 28.23.4.4 Tides

By pairing a smooth reverb with a multiband filter that sweeps across the output spectrum, the Tides algorithm conjures up rippling, frequency-banded textures.

Beyond the common parameters covered above, Tides offers the following:

- Damping sets how much treble gets rolled off inside the reverb algorithms; turn it up and the resulting reverberation grows darker in tone.
- Wave reshapes the modulation curve of the filter, sweeping it from noise (0%) through sine (50%) and on to square (100%).
- Tide controls how pronounced the texture from the tail’s modulation becomes.
- Phase sets how far apart the left and right modulation waveforms are offset from one another. Dial in 180° and the two channels sit completely out of phase.
- Rate fixes how fast the modulation oscillator runs, expressed in beat divisions that include Triplet, 16th, and Dotted note value variants.

<a id="source-282345-prism"></a>
#### 28.23.4.5 Prism

Built on velvet (spectrally flat) noise, the Prism algorithm delivers a distinctive, brilliant, synthetic-sounding diffuse reverb. You can readily deploy it as a “ghost” reverb that lends depth without stepping on the original material. It shines on short, non-linear decays for drums and transients, yet it works just as well on sustained sources with longer decays where you want a tidy but clearly digital character.

On top of the common parameters listed earlier, Prism contributes these:

- Low Mult stretches or shrinks how long the low end of the reverb tail takes to decay.
- High Mult stretches or shrinks how long the top end of the reverb tail takes to decay.
- X over sets where the split between the tail’s low- and high-frequency regions falls, thereby determining which frequencies the Low Mult and High Mult parameters act upon.

Tip: To nail that vintage ‘80s gated-snare-reverb sound, keep the Decay and Size values on the small side.
