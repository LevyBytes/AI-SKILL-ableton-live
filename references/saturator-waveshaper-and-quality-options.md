# Saturator Waveshaper And Quality Options

Open when you need guidance on Saturator Waveshaper And Quality Options in Ableton Live.

Context: [Saturator](roar-saturator-shifter-spectral-resonator-routes.md#2834-saturator).

<a id="source-283401-saturators-waveshaper-controls"></a>
#### 28.34.0.1 Saturator’s Waveshaper Controls

Choosing the Waveshaper curve type brings six extra parameters to life in the expanded view.

The Waveshaper Controls.

Here is how the Waveshaper controls shape the device’s signal-processing behavior:

- _Drive_ sets the degree to which the Waveshaper curve’s parameters act on the input signal. At 0%, those parameters leave the Waveshaper curve untouched, while at 100% they shape the curve completely.
- _Curve_ contributes primarily third-order harmonics to the input signal.
- _Depth_ governs how tall a sine wave is laid over the top of the Waveshaper curve. Raising the value lifts that sine wave’s amplitude so it bends the shaping curve more strongly. At 0%, the sine wave exerts no effect.
- _Linear_ operates together with the Curve and Depth parameters to reshape the linear region of the Waveshaper curve.
- _Damp_ levels off any signals sitting close to the waveform’s center. Its behavior resembles an extremely fast noise gate.
- _Period_ sets how tightly the ripples in the overlaid sine wave are packed, relative to the Depth control.

<a id="source-283402-context-menu-options-for-saturator"></a>
#### 28.34.0.2 Context Menu Options for Saturator

Saturator’s context menu exposes two further modes you can switch on: Hi-Quality and Pre-DC Filter. Engaging Hi-Quality mode cuts down aliasing and raises audio fidelity (most noticeably on high frequency signals), though it draws a little extra CPU. Turning on Pre-DC Filter mode inserts a DC filter at Saturator’s input stage, handy for stripping DC offsets out of audio that carries them.
