# Live Audio Effect Reference (part 7)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Every band is equipped with both an activator and a solo button. When the activator button is switched off for a particular band, that band's gain controls along with its compression/expansion are skipped. Putting one band into solo silences all the rest. Ahead of dynamics processing, the Input knobs raise or lower each band's level, whereas the Output knobs sitting to the right of the display set the band levels once processing has occurred.

The display area lets you both watch your dynamics processing in action and tune the compression and expansion behavior that applies. Within each band, large bars stand in for the output level, whereas small bars stand in for the input level prior to processing. When nothing is being processed, the input meters sit flush with the top edge of the output meters. Along the lower edge of the display, the scale is marked in dB. While you tweak a band's gain or dynamics processing, the display lets you observe how its output shifts relative to its input.

When you drag your mouse across the display, the pointer turns into a bracket whenever it crosses the edges of the blocks at either the left or right side. Those blocks stand for the signal levels falling under the Below threshold and rising over the Above threshold, in that order. Pulling left or right at the edges of these blocks changes the threshold level. Keeping Ctrl (Win) / Cmd (Mac) held during a threshold drag applies the same threshold across every band. Keep Alt (Win) / Option (Mac) held to tune the Above and Below thresholds together for one band. Keeping Shift held while you drag left or right lets you set a single band's threshold with greater precision.

When you hover the pointer over the central part of the block, it becomes an up-down arrow. Drag it up or down to raise or lower the loudness of the signal that falls inside the chosen volume range. Keeping Ctrl (Win) / Cmd (Mac) held while you drag up or down sets that same block's volume on every band. Keep Alt (Win) / Option (Mac) held to tune the Above and Below volumes together for one band. Keeping Shift held while dragging up or down lets you tune a single band's volume with greater precision. A double-click inside the region returns the volume to its default value.

Speaking technically, dropping the volume in the block sitting above the Above threshold yields downward compression, whereas lifting it yields upward expansion. In the same way, dropping the volume in the block sitting below the Below threshold yields downward expansion, whereas lifting it yields upward compression. Across every one of these cases, what you are changing is the compressor or expander ratio.

You can likewise tweak the thresholds and ratios for all bands through the column placed to the right of the display. Per band, the ”T,” ”B” and ”A” buttons in the lower-right corner of the display area cycle the readout through three sets: Time, holding attack plus release; Below, holding threshold plus ratio; and Above, again holding threshold plus ratio.

When dealing with the Above thresholds, Attack determines the time required to hit full compression or expansion after a signal climbs past the threshold, whereas Release determines the time the device needs to come back to normal once the signal sinks beneath the threshold.

When dealing with the Below thresholds, Attack determines the time required to hit full compression or expansion after a signal sinks beneath the threshold, whereas Release determines the time the device needs to come back to normal once the signal climbs past the threshold.

When Soft Knee is switched on, compression or expansion sets in slowly as the signal nears the threshold.

How rapidly Multiband Dynamics tracks level changes is likewise shaped by the RMS/Peak switch. When Peak is chosen, the device responds to brief peaks inside a signal. Choosing RMS mode makes it less reactive to extremely brief peaks and holds off processing until the incoming level has stayed past the threshold for a somewhat longer stretch.

Overall output gain for the device is governed by the global Output knob.

The Time control rescales the lengths of every one of the Attack and Release controls. With this, you can keep the same proportional envelope timing while speeding them all up or slowing them all down together.

Across all bands, the Amount knob controls how strong the applied compression or expansion is. When set to 0%, every compressor/expander runs at an effective ratio of 1, so it leaves the signal untouched.

### 28.26.3 Sidechain Parameters

The Multiband Dynamics Device With Sidechain Section.

Under typical conditions, the signal under processing and the input that fires the device are one and the same. However, with _sidechaining_, you can drive dynamics processing on one signal according to the level of a different signal or a particular frequency component. You reach the Sidechain parameters by unfolding the Multiband Dynamics window through the button in its title bar.

Switching on the Sidechain button lets you pick any of Live’s internal routing points using the choosers underneath. With this, the chosen source becomes the device’s trigger rather than the signal that is genuinely under processing.

The level of the external sidechain’s input is governed by the Gain knob, while the Dry/Wet knob lets you blend the sidechain together with the original signal to form the trigger. When Dry/Wet sits at 100%, the sidechain source fully drives the device. When it sits at 0%, the sidechain is essentially turned off. Keep in mind that raising the gain does _not_ lift the source signal's level inside the mix. That sidechain audio serves purely as a trigger for the device and you never actually hear it.

Using the headphones button, you can monitor the sidechain input by itself while bypassing what the device puts out. Because that sidechain audio never reaches the output and works only as a device trigger, this short-term monitoring choice makes setting sidechain parameters and hearing what truly drives the device far simpler.

### 28.26.4 Multiband Dynamics Tips

Multiband Dynamics is a powerful, feature-packed device that can run as many as six separate kinds of processing at once. For that reason, the first steps with it may feel a little overwhelming. Below are a few practical uses to spark some ideas.

#### 28.26.4.1 Basic Multiband Compression

If you rely only on the upper thresholds, Multiband Dynamics works as a conventional ”downward” compressor. Tune the crossover points to fit your audio material, then bring in downward compression (either by pulling down on the upper blocks in the display or by entering numerical ratios greater than 1.)

#### 28.26.4.2 De-essing

If you want to clear out ”harshness” coming from excessively loud high frequency content, try switching on only the upper band and putting its crossover frequency near 5 kHz. After that, slowly tune the threshold and ratio so you bring in gentle downward compression. Soloing the band can make it easier to pick out the effect of your adjustments. As a rule, de-essing performs best when attack and release times are reasonably fast.

#### 28.26.4.3 Uncompression

Mastering engineers are frequently expected to work wonders, such as injecting punch and energy into a mix that has already taken heavy compression and consequently retains almost no transients. In most cases, these mixes have also been heavily maximized, which means they keep no headroom either. Fortunately, upward expansion can occasionally breathe some life back into material that has been over-squashed in this way. Here's the procedure:

1. Lower the Input knob so you create a bit of extra headroom.
2. Set the Above thresholds for each band so they fall below the loudest peaks.
3. Apply a modest amount of upward expansion to every band. Take care — too much upward expansion can push transients to extreme loudness.
4. Tune the attack and release times for every band with care. Be aware that, in contrast to ordinary downward compression, extremely fast attack times will _increase_ the impact of transients, whereas slower ones produce a more muffled result.

_Note_: Placing a maximizer or limiter after you've brought some peaks back to your material in order to boost gain may just wipe them out once more.

### 28.27 Overdrive

The Overdrive Effect.

Overdrive is a distortion effect that tips its hat to certain vintage pedal units that guitarists have long favored. In contrast to plenty of distortion devices, you can push it remarkably hard while keeping its dynamic range intact.

A band-pass filter, adjustable through an X-Y controller, comes ahead of the distortion stage. Set the filter bandwidth by clicking and dragging along the vertical axis. Place the frequency band by clicking and dragging along the horizontal axis. You can also dial in these parameters through the slider boxes beneath the X-Y display.

How much distortion you get is set by the Drive control. Keep in mind that 0% is not the same as no distortion at all!

Tone behaves as an EQ control after the distortion stage. The higher you push it, the more high-frequency content the signal carries.

With the Dynamics slider, you control the degree of compression brought in as distortion grows. At lower settings, pushing distortion higher brings about greater internal compression along with make-up gain. At higher settings, the amount of compression applied is reduced.

The balance between the dry and processed signals is set by the Dry/Wet control. Put it at 100 percent when you run Overdrive on a return track.

### 28.28 Pedal

The Pedal Effect.

Pedal is a guitar distortion effect. Paired with Live’s [Tuner](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#tuner), [Amp](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#amp) and [Cabinet](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#cabinet) effects, Pedal works wonderfully for shaping guitar tones. You can also put Pedal to work in more unusual ways, for instance as a standalone effect on vocals, synths or drums.

How much distortion is applied to the dry signal is set by the Gain control. Remember that 0% is not the same as no distortion. A good approach is to pull the Gain back down to 0% and raise it gradually until the output level you want appears. If you position it ahead of Pedal within a device chain, the Gain parameter of [Utility](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#utility) can drop the signal down further still.

Overall output gain for the device is governed by the global Output knob.

You have three distinct Pedal Types to pick from, each one modeled on distortion pedals carrying their own particular sonic character:

- Overdrive: warm and smooth
- Distortion: tight and aggressive
- Fuzz: unstable, with a “broken amp” sound

Pedal includes a three-band EQ that shapes the sound's timbre once distortion has been applied. That EQ is adaptive, meaning the resonance (or “Q”) grows as the EQ boost grows.

The Bass control acts as a peak EQ centered at 100 Hz. It comes in handy for adding “punch” to bass or drum sounds, or for trimming low frequencies out of guitars.

The Mid control functions as a three-way switchable boosting EQ. Both the center frequency and range of the Mid control are determined by the Mid Frequency switch. That center frequency marks the midpoint of the frequency range the Mid control acts upon. Around this center value, the frequency range is tighter at the lowest switch setting and broader at the higher one. Such behavior is typical of guitar pedals, where tight cuts and boosts are commonly made at low frequencies and broader ones at high frequencies.

These are the center frequencies for each switch setting:

- Lowest setting, positioned on the left side: 500 Hz
- Middle setting, positioned in the center: 1 kHz
- Highest setting, positioned on the right side: 2 kHz

The Treble control acts as a shelving EQ with its cutoff at 3.3 kHz. It comes in handy for taming harsh high frequencies (or for lifting them, if that suits your taste!).

Tip: When you want finer EQ control after the distortion, just keep these controls at their neutral position and reach instead for a separate EQ, for example [EQ Eight](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#eq-eight).

The Sub switch enables a low shelf filter that lifts frequencies under 250 Hz. You can pair it with the Bass control by switching Sub on and setting the Bass to -100%, or by switching Sub off and setting the Bass to 100%.

The balance between the dry and processed signals is set by the Dry/Wet slider.

You can cut down aliasing by switching on Hi-Quality mode, reachable through the context menu in the device title bar. This lifts the sound quality, especially where high frequency signals are concerned, though it does cost a small amount of additional CPU.

### 28.28.1 Pedal Tips

#### 28.28.1.1 Positioning Pedal in the Device Chain

How the distortion reacts is shaped by the signal arriving at it. As an example, putting a Compressor ahead of Pedal in the device chain produces a more even outcome. Conversely, placing an EQ or filter set to high gain and resonance ahead of Pedal can produce a screaming distortion effect.

#### 28.28.1.2 Techno Kick

Pick a fitting kick that has a long decay (for instance Kit-Core 909, with its decay raised). Next, select the Distort pedal, switch on the Sub switch, and tune the Gain however you like.

For extra “whack”, push the Mid Frequency switch over to the right-most position and raise the Mid control. To get more “thump”, you can raise the Bass control.

To pull back the “air”, lower the Treble control.

#### 28.28.1.3 Drum Group Fizzle

To bring “fizzle” into a drum group, pick the Fuzz pedal, raise the Gain to 50% and confirm the Sub switch is turned off.

Pull the Bass and Mid controls down to -100%, and set the Mid Frequency Switch however you like. Push the Treble up to 100%.

Put the Output at -20dB. After that, drop the Dry/Wet slider to 0% and raise it slowly until the drums fizzle the way you want.

#### 28.28.1.4 Broken Speaker

Pick the Fuzz pedal, and confirm the Sub switch is turned off. Bring the Bass control all the way down, and put the Treble at 25%.

Put the Mid control at 100% and push the Mid Frequency switch to the right-most position. Lastly, set the Gain control to 100%.

#### 28.28.1.5 Sub Warmer

To layer upper harmonics and warmth onto a plain sub bass, pick the OD pedal, switch on the Sub switch and raise the Bass control. After that, push the Gain up slowly until you reach the effect you want. You can then trim or lift the mid frequencies with the Mid control.

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

### 28.30 Redux

The Redux Effect.

The Redux effect offers a range of parameters for producing a broad spread of jagged, edgy sounds. You can drastically mangle any source material, with results that span harsh distortion and digital aliasing artifacts through to warm, fat 8-bit grit. You can fold extra noise and stereo width into the downsampling process, while filtering reshapes the sound even further. The quantizer’s amplitude curve is also adjustable, enabling both gentle and severe bitcrushing.

Redux relies on a pair of distinct digital signal manipulation methods: downsampling and bit reduction.

### 28.30.1 Downsampling

You'll find the downsampling controls on the device's left side. Running Redux’s downsampler with no filters engaged brings inharmonic frequency content into the spectrum. How wide that added content's frequency range is depends on the interplay between the material's frequency content and the sample rate set in the device.

Rate sets the sample rate down to which the signal is degraded. Lower values bring about greater imaging along with more inharmonic tones.

Jitter feeds noise into the downsampler’s clock signal, which adds randomness to the downsampling process. The outcome is a noisier tone plus broader stereo width.

The Filter section offers both a Pre and a Post setting. Switching on the Pre button brings in a filter ahead of downsampling, which narrows the bandwidth of the signal that downsampling processes. With Jitter in play, it additionally narrows the signal's stereo width.

The Post button brings in a low-pass filter following the downsampling process, which trims imaging. You can tune the Post filter frequency with the Post-Filter Octave slider. The displayed number stands for how many octaves sit above or below half of the frequency given in the Rate parameter.

### 28.30.2 Bit Reduction

You'll find the bit reduction controls on the device's right side. Bit reduction cuts the number of bits used to depict the digital signal, trimming dynamic range while introducing distortion and noise. Under extreme settings, every bit of the original dynamics vanishes and sounds collapse into jagged square waves.

The Bits control cuts how many bits are in use. The displayed value stands for how many bits encode the output signal. Lowering this value raises noise and distortion while cutting dynamic range.

Shape alters the contour of the quantizer’s characteristic curve. Higher values yield a finer resolution at smaller amplitudes, which means subtle signal components take less of a hit than louder ones do. How much total distortion arises across different Shape settings will hinge on the input signal's dynamic range.
