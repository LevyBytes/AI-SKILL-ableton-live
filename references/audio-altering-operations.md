# Audio Altering Operations

Open when you need guidance on Audio Altering Operations in Ableton Live.

Context: [Non-Neutral Operations](audio-fact-sheet.md#383-non-neutral-operations).

<a id="source-3831-playback-in-complex-and-complex-pro-mode"></a>
### 38.3.1 Playback in Complex and Complex Pro Mode

The [Complex](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#complex-and-complex-pro-mode) and [Complex Pro](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#complex-and-complex-pro-mode) Warp Modes rest on a completely separate technology from the algorithms driving Beats, Tones, Texture, and Re-Pitch modes. The Complex modes can deliver a better sound — especially on mixed sound files holding several types of audio material — yet they are never neutral, not even when the tempo is left unchanged. For that reason, together with the heavier CPU load these algorithms carry, we suggest reaching for them only when the other Warp Modes fail to give satisfactory results.

<a id="source-3832-sample-rate-conversiontransposition"></a>
### 38.3.2 Sample Rate Conversion/Transposition

Converting the sample rate — whether in real-time playback or while rendering — is non-neutral. Playing back audio files whose sample rate differs from the figure set in Live‘s Settings window degrades the signal. Transposition is itself a kind of sample-rate conversion, so it likewise behaves non-neutrally.

To hold down any harm during real-time playback, the advice is to handle sample rate conversion offline instead of mixing files of varying sample rates inside one Set. After you‘ve exported the samples at whatever sample rate you intend to use in Live, you can import those files with no quality loss at all.

Rendering audio out of Live at a sampling rate other than the one you used throughout the project is also non-neutral. The sample rate conversion that happens during export relies on the outstanding [SoX Resampler](https://soxr.sourceforge.net) library, licensed under the [GNU LGPL v2.1](https://gnu.org/licenses), producing downsampled files with remarkably low distortion.

<a id="source-3833-volume-automation"></a>
### 38.3.3 Volume Automation

Automating the volume level shifts the gain, which by definition makes it non-neutral. Some ways of implementing automation envelopes, however, can throw off audible artifacts — especially when those envelopes aren‘t recalculated quickly enough. In Live, the volume automation curves refresh once per audio sample, so the distortion stays extraordinarily low.

<a id="source-3834-dithering"></a>
### 38.3.4 Dithering

Any time you render audio down to a lower bit depth, applying dithering is wise as a way to hold artifacts in check. Dithering — essentially a very faint layer of noise — is non-neutral by nature, but it‘s an unavoidable trade-off when you drop the bit resolution.

Bear in mind that Live processes every internal signal at 32-bit, so even one gain change turns the resulting audio into 32-bit material as well, regardless of whether the original was 16- or 24-bit. Because dither must never be applied to the same audio file more than once, the safest course — unless you‘re mastering and finalizing within Live — is to render at 32-bit every time and skip dithering completely.

<a id="source-3835-recording-external-signals-bit-depth--ad-converter"></a>
### 38.3.5 Recording External Signals (Bit Depth < A/D Converter)

Capturing audio into Live turns non-neutral whenever the bit depth chosen in Live‘s Settings window sits below that of the A/D converters supplying the recording. We advise against doing this.

<a id="source-3836-recording-internal-sources-below-32-bit"></a>
### 38.3.6 Recording Internal Sources Below 32 Bit

Whenever you capture material through internal routing at any bit depth under 32 bits, quality suffers. To keep captures of plug-in instruments — and of any signal moving through effects plug-ins — neutral, the recommendation is to record internally at 32 bits. Still, note that if the source is already at a lower bit depth, an internal recording at that same depth remains neutral as well (provided no effects are involved); pushing an untouched 16 bit file up to 32 bits during internal recording will not raise its sound quality.

<a id="source-3837-consolidate"></a>
### 38.3.7 Consolidate

[Consolidating clips](https://www.ableton.com/en/live-manual/12/arrangement-view/#consolidating-clips) in the Arrangement View produces fresh audio files that are non-neutral relative to the source audio data. In particular, those new files are normalized, and their clip volumes get trimmed so playback matches the loudness you heard before consolidating. Since normalization adjusts gain, it is a non-neutral operation. Beyond that, the new files take on whatever sample rate and bit depth Live‘s Settings window specifies, which can be different from the values in the original audio files.

<a id="source-3838-clip-fades"></a>
### 38.3.8 Clip Fades

With Create Fades on Clip Edges switched on under the Record, Warp & Launch Settings, Live lays a brief fade — no longer than 4 ms — across the clip‘s start and end to head off clicks at those boundaries. You can also bring these “declicking“ fades to Session View clips through the [Clip Fade](https://www.ableton.com/en/live-manual/12/clip-view/#clip-start-and-end-fades) button. On top of that, Arrangement View clips offer [editable fades and crossfades](https://www.ableton.com/en/live-manual/12/arrangement-view/#audio-clip-fades-and-crossfades). Any of these fade options is non-neutral once applied.

<a id="source-3839-panning"></a>
### 38.3.9 Panning

Panning in Live follows a constant power scheme built on sinusoidal gain curves. At the center position the output sits at 0 dB, while a signal panned hard left or right gains +3 dB. To keep that level shift in check, it can help to tighten the overall stereo width ahead of any extreme panning, which you accomplish through the Width control in the Utility device.

<a id="source-38310-grooves"></a>
### 38.3.10 Grooves

In the majority of cases, playing a warped clip whose tempo lines up with the Set is neutral. Add a [groove](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves), though, and the playback turns non-neutral at every tempo.
