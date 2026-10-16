# Overdrive And Pedal

Open when you need guidance on Overdrive And Pedal in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2827-overdrive"></a>
### 28.27 Overdrive

The Overdrive Effect.

Overdrive is a distortion effect that tips its hat to certain vintage pedal units that guitarists have long favored. In contrast to plenty of distortion devices, you can push it remarkably hard while keeping its dynamic range intact.

A band-pass filter, adjustable through an X-Y controller, comes ahead of the distortion stage. Set the filter bandwidth by clicking and dragging along the vertical axis. Place the frequency band by clicking and dragging along the horizontal axis. You can also dial in these parameters through the slider boxes beneath the X-Y display.

How much distortion you get is set by the Drive control. Keep in mind that 0% is not the same as no distortion at all!

Tone behaves as an EQ control after the distortion stage. The higher you push it, the more high-frequency content the signal carries.

With the Dynamics slider, you control the degree of compression brought in as distortion grows. At lower settings, pushing distortion higher brings about greater internal compression along with make-up gain. At higher settings, the amount of compression applied is reduced.

The balance between the dry and processed signals is set by the Dry/Wet control. Put it at 100 percent when you run Overdrive on a return track.

<a id="source-2828-pedal"></a>
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
