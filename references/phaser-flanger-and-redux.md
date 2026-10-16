# Phaser Flanger And Redux

Open when you need guidance on Phaser Flanger And Redux in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2829-phaser-flanger"></a>
### 28.29 Phaser-Flanger

The Phaser-Flanger Effect.

Phaser-Flanger merges flanger and phaser effects into a single device that has separate modes, and adds an extra Doubler mode on top. Each mode can be used to build lush, expressive sounds, backed by a broad selection of tools and fine-grained options. A pair of LFOs together with an envelope follower supply abundant modulation options.

In the display, you have three modes to pick from:

- Phaser, covering a broad span of frequency and modulation ranges, builds roaming notch filters by routing a phase-shifted copy of the input signal back into the input. That phase shifting comes from modulated all-pass filters and carries a lush sound.
- Flanger builds a constantly shifting comb filter effect by mixing a time-modulated delayed signal with feedback into the input.
- Doubler builds the impression of doubled tracks (several stacked versions of comparable recording takes) by mixing time-modulated delayed signals into the input.

Within the display sit a visualization plus the mode selector buttons. What the visualization shows varies with the mode you pick and the settings of the LFO Stereo Mode (covered in greater detail further down).

While in Phaser mode, the visualization displays how many notches there are along with their spectral placements.

You tune Phaser’s parameters in the display's lower section.

Notches raises or lowers how many all-pass filters are in use. Center selects the notches' center frequency. Spread widens or narrows the gap between notches by changing the Q factor of the all-pass filters. Blend balances the modulation routing across Center Frequency and Spread, where Center Frequency sits at 0.0 and Spread at 1.0.

While in Flanger mode, the visualization displays the way the modulation signal alters the delay time, with the left-most position matching the value set in the Time parameter. When the visualization travels rightward, the delay time shrinks; when it travels leftward, it grows. Time tunes the delay time of the Flanger delay lines.

While in Doubler mode, the visualization behaves unlike it does in Flanger mode. Modulation in Doubler mode is bipolar, so as the visualization travels rightward, the delay time grows; as it travels leftward, it shrinks. Time tunes the delay time of the Doubler delay lines.

To gain finer control over the sound, unfold the device through the button in Phaser-Flanger’s title bar, which exposes more options for the main LFO, along with a second LFO, an envelope follower, plus a high-pass filter labeled Safe Bass. A visualization for the main LFO is shown as well, presenting its rate, waveform and the phase relationships between the stereo channels.

The Phaser-Flanger Effect’s Unfolded View.

The Freq/Rate parameter governs the main LFO’s speed, which may be either tempo-synced or free-running. The Modulation Sync buttons sitting to the left of the dial let you flip between Frequency and Sync Rate. While set to Hz, the matching Freq dial governs the LFO rate measured in Hertz; if not, the Rate dial locks the LFO to the song tempo.

Several waveforms exist for the main LFO and reside in the LFO Waveform chooser. The default among them is Triangle, while the rest comprise Sine, plus the pair Saw Up and Saw Down, then Rectangle, then Random along with its companion Random S&H (Sample and Hold). On top of those you'll find Triangle Analog, Triangle 8, Triangle 16, detailed here:

- Triangle Analog is a low-pass filtered rectangular waveform that shifts its shape and amplitude sharply across different LFO rates.
- Triangle 8 splits one period of an ordinary triangular wave into eight discrete steps.
- Triangle 16 splits one period of an ordinary triangular wave into 16 discrete steps.

The LFO Stereo Mode button toggles between Phase and Spin modes, each of which lets you modulate every stereo channel on its own.

While Phase is selected, changing the Phase value alters the phase relationship across the left and right channels. At 180°, the left and right channels' phase is entirely inverted. You can observe this within the LFOs visualization.

While Spin is selected, changing the Spin value detunes the pair of LFO rates against one another. You can observe this within the main display’s visualization.

Duty Cycle shifts the time scale of the waveform’s period, compressing it toward the cycle's start (100%) or, alternatively, toward its end (-100%). With a 0% setting, that period's time scale spreads uniformly across the entire cycle, leaving the waveform unchanged. The behavior resembles the way Pulse Width acts on rectangular waveforms, and you can observe its effects in the main LFO's waveform view. This parameter has no impact on the noise-based Random and Random S&H modulation waveforms.

The second LFO is always set to a triangular waveform, and you steer it with the LFO2 Mix and LFO2 Freq/Rate parameters.

LFO2 Mix governs how much of the LFO2 gets blended with the main LFO. At 0%, the main LFO alone is active; at 100% LFO2 alone is active.

You can set the second LFO’s speed to be either free-running or tempo-synced through the Modulation Sync 2 toggle buttons. While free-running, the sync frequencies appear in Hertz and you tune them with the LFO2 Freq parameter. While tempo-synced, beat divisions appear in their place and you set them with the LFO2 Rate parameter.

The global parameters on offer are Amount, Feedback, Output, Warmth and Dry/Wet. The extra envelope follower along with the Safe Bass high-pass filter become reachable once the device is unfolded.

Amount governs how much delay modulation gets applied to incoming signals and acts on both the main LFO and LFO2.

Feedback governs how much of each channel’s output is routed back to its input. Raising it sounds more extreme and tends to produce a pronounced comb filtering effect, boosting some frequencies while cutting others. In Doubler Mode, it will additionally produce audible delays once playback halts. You can invert the feedback signal with the Ø button, which yields a “hollow” sound once paired with high feedback values.

Caution: high feedback values combined with particular settings can produce sudden jumps in volume levels. Make sure you protect your ears and equipment!

Underneath the main LFO you'll come across an envelope follower. An envelope follower takes the amplitude of an incoming audio signal and converts it into a modulation source.

To put the envelope follower to use, switch on the Env Fol button and give the Envelope Amount a value that isn't zero. Envelope Amount governs how strong the modulation produced by the envelope follower is. Negative values flip the envelope's phase.

Within the envelope follower’s own envelope, its rising and falling segments are governed by Attack and Release. A shorter Attack value makes the envelope follower react more quickly, while a longer one delays the point at which it kicks in. Shorter Release times make the envelope follower end its effect sooner than longer Release times do.

Safe Bass is a high-pass filter that, in effect, trims the effect on signal components beneath the chosen frequency. Its usable range runs from 5 Hz to 3000 Hz. It can ease the mixing of certain bass-heavy material.

Output governs how much gain is applied to the processed signal. The Warmth control brings in slight distortion and filtering to give a warmer tone. The balance between the dry and processed signals is set by the Dry/Wet control. Put it at 100% when you run Phaser-Flanger on a return track.

<a id="source-2830-redux"></a>
### 28.30 Redux

The Redux Effect.

The Redux effect offers a range of parameters for producing a broad spread of jagged, edgy sounds. You can drastically mangle any source material, with results that span harsh distortion and digital aliasing artifacts through to warm, fat 8-bit grit. You can fold extra noise and stereo width into the downsampling process, while filtering reshapes the sound even further. The quantizer’s amplitude curve is also adjustable, enabling both gentle and severe bitcrushing.

Redux relies on a pair of distinct digital signal manipulation methods: downsampling and bit reduction.
