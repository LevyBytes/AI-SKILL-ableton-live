# Redux Downsampling Bit Depth And Mix

Open when you need guidance on Redux Downsampling Bit Depth And Mix in Ableton Live.

Context: [Redux](multiband-distortion-and-modulation-routes.md#2830-redux).

<a id="source-28301-downsampling"></a>
### 28.30.1 Downsampling

You'll find the downsampling controls on the device's left side. Running Redux’s downsampler with no filters engaged brings inharmonic frequency content into the spectrum. How wide that added content's frequency range is depends on the interplay between the material's frequency content and the sample rate set in the device.

Rate sets the sample rate down to which the signal is degraded. Lower values bring about greater imaging along with more inharmonic tones.

Jitter feeds noise into the downsampler’s clock signal, which adds randomness to the downsampling process. The outcome is a noisier tone plus broader stereo width.

The Filter section offers both a Pre and a Post setting. Switching on the Pre button brings in a filter ahead of downsampling, which narrows the bandwidth of the signal that downsampling processes. With Jitter in play, it additionally narrows the signal's stereo width.

The Post button brings in a low-pass filter following the downsampling process, which trims imaging. You can tune the Post filter frequency with the Post-Filter Octave slider. The displayed number stands for how many octaves sit above or below half of the frequency given in the Rate parameter.

<a id="source-28302-bit-reduction"></a>
### 28.30.2 Bit Reduction

You'll find the bit reduction controls on the device's right side. Bit reduction cuts the number of bits used to depict the digital signal, trimming dynamic range while introducing distortion and noise. Under extreme settings, every bit of the original dynamics vanishes and sounds collapse into jagged square waves.

The Bits control cuts how many bits are in use. The displayed value stands for how many bits encode the output signal. Lowering this value raises noise and distortion while cutting dynamic range.

Shape alters the contour of the quantizer’s characteristic curve. Higher values yield a finer resolution at smaller amplitudes, which means subtle signal components take less of a hit than louder ones do. How much total distortion arises across different Shape settings will hinge on the input signal's dynamic range.

<a id="source-live-audio-effect-reference-part-8"></a>

Switching on the DC Shift button introduces an amplitude offset ahead of quantization. The character of the quantization distortion shifts noticeably as a result — most audibly when Bits sits at lower values, where the level rises and extra crunch appears!

Use the Dry/Wet control to balance how much processed versus dry signal you hear. When Redux runs in a return track, dial this to 100%.
