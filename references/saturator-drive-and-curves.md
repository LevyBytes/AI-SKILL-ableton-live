# Saturator Drive And Curves

Open when you need guidance on Saturator Drive And Curves in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2834-saturator"></a>
### 28.34 Saturator

The Saturator Effect.

As a waveshaping effect, Saturator lends your sound the grit, punch, or warmth it might be lacking. It achieves this by subjecting the input signal to non-linear shaping, producing anything from gentle saturation through to heavy coloration.

The way Saturator works is by remapping every single sample value in the incoming signal to a fresh value, guided by whichever shaping curve you pick. Since that mapping is generally non-linear, the signal ends up being reshaped on the fly according to how loud it is from one instant to the next.

The Curve Type chooser is where you pick which curve handles the input shaping. Eight options are offered. The first four are Analog Clip, Soft Sine, Bass Shaper, and Medium Curve; the remaining four are Hard Curve, Sinoid Fold, Digital Clip, and Waveshaper.

Each curve type carries its own shaping behavior. Once the clipping point is crossed, Digital Clip clips abruptly and hard, whereas Analog Clip eases through that point more gently. Below the clipping point, both of these curves stay linear. Saturation with distinct tonal flavors is provided by the Soft Sine, Medium Curve, and Hard Curve options. As a wavefolding curve, Sinoid Fold makes the output fold back on itself as the input grows louder, yielding strange textures.

Although the Bass Shaper curve resembles Analog Clip in some respects, it delivers a cleaner harmonic spectrum when low frequency signals are pushed with high gain. That trait makes it well suited to low-end material such as 808 kick drums and synth basslines.

A separate Bass Shaper Threshold control comes with Bass Shaper and defines the curve’s threshold across a range of 0 to -50 dB. As long as the input stays under the threshold the curve stays linear, but it begins clipping gradually once the signal rises past that point. This lets you transition smoothly from one clipping style into another: lower threshold settings yield soft clipping while higher ones yield hard clipping. For bass material the lower threshold settings are most effective, particularly alongside high Drive values.

If you want the boldest shaping of all, choose the Waveshaper curve. It comes with a dedicated control set of its own that you open by clicking the Toggle Expanded View button on the device title bar; further detail on how those parameters shape the signal appears in [the dedicated section below](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#saturators-waveshaper-controls).

Serving two purposes at once, the Shaper Curve display visualizes Saturator’s shaping curve and, in real time, plots the input signal against the chosen curve type. Saturation kicks in wherever the input reaches the curve’s non-linear regions.

A post-clipping stage applicable to every curve type can be chosen from the Post Clip Mode chooser sitting beneath the Shaper Curve display. With either Soft Clip or Hard Clip engaged, Saturator’s output stays at or below the ceiling defined by the Output control. That proves especially handy for taming any extra boost introduced by negative Color values.

Engaging the Color toggle activates the device’s pair of color filters, which draw a color curve shown in the device’s expanded view. These filters impose an EQ curve once before the shaper and then once more, inverted, after it. As a result you could, for instance, strip out bass frequencies ahead of the shaper so that only the mid and high range gets saturated while the bass energy is preserved in the output.

The Amt Lo slider lets you set how much saturation reaches the low frequencies. Going negative pulls back the total saturation on the lows, whereas going positive boosts it.

Before Saturator processes the signal, the Drive control raises its input gain. The extent of that effect on the input is visible inside the device’s Shaper Curve display.

Saturator’s final output level is reduced by the Output control. Whenever Soft Clip is engaged in the Post Clip Mode chooser, Saturator additionally runs an Analog Clip curve across the device’s output.

How the dry and processed signals are balanced at Saturator’s output is governed by the Dry/Wet control. When Saturator sits on a return track, set this to 100%.

Found in the expanded view, the Color Curve display renders a picture of the curve produced by the device’s two color filters.

The Color Curve Display and Color Filter Parameters.

Three further controls for sculpting Saturator’s color filters sit underneath the display. The Amt Hi slider governs how much saturation the second filter applies across the chosen frequency range. Going positive piles on more saturation while going negative pulls it back. With the Frequency slider you set the center frequency that the second color filter targets, and Width sets how broad a span of frequencies it touches.

These color filter settings can also be edited by dragging the handles within the Color Curve display — moving the first handle controls the Amt Lo parameter, while moving the second handle controls either the Amt Hi or the Frequency parameter, according to whether you drag it horizontally or vertically.
