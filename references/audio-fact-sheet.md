# Audio Fact Sheet

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 38. Audio Fact Sheet

A large share of the engineering work at Ableton goes into rigorous, dispassionate measurement of how Live handles audio at its core. That ongoing testing has prompted us to roll out many small refinements to the audio engine over time. This document exists so that people can see precisely whether — and how — their signal gets altered by particular Live features that frequently get misread, and it also collects pointers for getting the cleanest possible output.

Our investigations concentrate on behavior that can be quantified and measured objectively. We avoid asserting anything about what you might _hear_, since there is no way for us to anticipate factors such as your room, your gear, the sensitivity of your ears, and so on. On top of that, none of this work attempts to rank Live against rival audio applications. Instead, it gathers verifiable facts describing what Live genuinely _does_ in a range of situations.

### 38.1 Testing and Methodology

At the time of writing, each Live build runs through an extensive battery of automated checks spanning the full range of Live‘s capabilities. Every new feature brings new checks along with it, and no update ships unless it clears the entire suite.

### 38.2 Neutral Operations

We call any Live procedure that produces zero alteration in audio quality a _neutral operation_. Relying on these functions guarantees that the signal stays intact. Use a neutral operation on material captured into Live and the result matches the signal exactly as it stood right after analog-to-digital conversion. Use one on files brought into Live and what you get is bit-identical to the versions sitting on disk. Use one while exporting from Live and the rendered file lands at quality no worse than what reached your ears during playback.

Treat the catalog of neutral operations that follows mainly as a theoretical reference. Each entry truly is neutral on its own, yet keep in mind that in practice it nearly always sits inside a chain that also includes non-neutral steps. Take an effects device, for instance: passing a signal through it is non-neutral. Whatever neutral operations come afterward will therefore still hand you audio that has been changed in some respect. Strictly speaking, even nudging the gain counts as non-neutral.

Neutral operations include:

### 38.2.1 Undithered Rendering

The [Export Audio/Video](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video) command writes Live’s audio output to a disk file. Provided certain criteria hold, this rendering counts as a neutral operation:

- The rendered file carries the same sample rate that the audio hardware uses in Live‘s Settings.
- Nothing non-neutral has been applied along the way.

To gauge Live‘s rendering, we feed it three categories of unprocessed material — white noise, fixed-frequency sine waves and sine sweeps — at 16-, 24- and 32-bit word lengths, then render each one out, again at assorted bit resolutions. Running phase cancellation between the source material and the rendered results yields this:

- Render at the same bit depth as the source, and the two cancel completely.
- Render at a bit depth above the source, and you again get complete cancellation.
- Render at a bit depth beneath the source, and the distortion introduced is as small as a 32-bit system can manage.

### 38.2.2 Matching Sample Rate/No Transposition

When Live plays an unstretched audio file, that playback is neutral as long as the file‘s sample rate matches what Live‘s Settings specify and no transposition is applied during playback. Cancellation tests on rendered output confirm this. Bear in mind that “playback“ here means strictly the audio inside Live, before it ever arrives at your audio hardware.

### 38.2.3 Unstretched Beats/Tones/Texture/Re-Pitch Warping

A clip whose tempo equals the tempo of the Set plays back without stretching. Under those conditions, as long as the clip‘s [Warp mode](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes) is Beats, Tones, Texture, or Re-Pitch — and not Complex or Complex Pro — its playback comes out neutral.

Whatever Warping results from altering the Set’s tempo is reversible: material that sounds unwarped at one tempo will keep sounding unwarped at that same tempo, even after the tempo is moved away and then brought back. Suppose you laid down several tracks at 120 BPM and later chose to drop the tempo to capture a tricky solo — once you restore the tempo to 120 BPM, those earlier tracks again play neutrally. The stretching applies solely to whatever you tracked at the reduced tempo.

Whether tempo automation captured in the Arrangement replays neutrally hinges on the Warp Mode. Turning on transient preservation with Beats mode can introduce artifacts; switching to preserve 16ths rather than transients, or moving to the Repitch Warp Mode, gets rid of them.

Keep in mind that [grooves](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves) operate by shifting where Warp Markers sit. As a consequence, any audio clip carrying a groove plays back non-neutrally, even at its native tempo.

Cancellation tests on rendered output establish that unstretched clip playback is neutral.

### 38.2.4 Summing at Single Mix Points

Wherever Live combines signals — clip and return track inputs, the Main track, Racks — it sums them in double precision (64-bit). So at any individual summing point, the act of mixing in Live is neutral. We verify this by loading pairs of 24-bit files (white noise plus fixed-frequency sine waves alongside their phase-inverted counterparts), summing each pair together eight successive times, and rendering the result as 32-bit files. Every one of those tests produces flawless phase cancellation.

Note, though, that even though 64-bit summing covers each _single_ mix point, the rest of Live‘s internal processing remains at 32-bit. Because of that, a signal routed through several summing points may pick up a vanishingly small amount of degradation. Pairing 64-bit summing with a 32-bit architecture lands on an excellent compromise between sound quality and demands on CPU and memory.

### 38.2.5 Recording External Signals (Bit Depth >/= A/D Converter)

Capturing audio into Live qualifies as neutral so long as the bit depth chosen in Live‘s Settings window meets or exceeds the bit depth of the A/D converters feeding the recording. In this setting, “neutral“ amounts to a bit-perfect match with whatever the A/D converters handed to Live.

### 38.2.6 Recording Internal Sources at 32 Bit

Material captured through internal routing comes out identical to its source as long as you record at 32 bits. We advise recording internally at 32 bits whenever you want neutral captures of plug-in instruments or of any signal flowing through effects plug-ins. That said, when the source is already at a lower bit depth, recording internally at that very depth stays neutral too (presuming no effects are in play) — taking an untouched 16 bit file and recording it internally at 32 bits does nothing to improve its fidelity.

Cancellation tests confirm that internal recording is neutral.

### 38.2.7 Freezing Tracks

Whenever you [freeze](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#track-freeze) tracks, Live writes the resulting audio files at 32 bit, guaranteeing they won‘t fall below the quality you heard before freezing. A handful of Freeze scenarios, though, behave non-neutrally and deserve mention:

A frozen Arrangement View track may carry sound that runs past the clip‘s own end — reverb tails, delay echoes, and the like. A frozen Session View track, by contrast, always spans precisely two loop cycles, so whatever audio would have spilled past two loop cycles during unfrozen playback gets truncated once the track is frozen.

For unfrozen clips, time-based effects such as reverbs and delays compute in real-time, which is why halting playback mid-tail lets that reverb or delay tail ring on. Frozen tails, on the other hand, have been baked into audio, so they cut off sharply when playback stops.

With frozen Arrangement View clips, every parameter automation is baked into the audio file. Frozen Session View clips instead capture a “snapshot“ of all parameter values as they stand at the Arrangement‘s 1.1.1 position and hold those for the whole length of the frozen clip. That mirrors how unfrozen clips work: while normal Session View clips play, any Arrangement automations stay “punched out“ until you click the Back to Arrangement button.

Live always replays frozen clips with Warp engaged in Beats mode, so they inherit exactly the same non-neutral characteristics as any other warped audio file.

Devices driven by random parameters — for instance, the Chance control found in the Beat Repeat device — stop behaving randomly once frozen. As with time-based effects, the random values present at the instant of freezing become part of the rendered file, so they are no longer recomputed in real-time.

### 38.2.8 Bypassed Effects

When an effect in Live is bypassed, it drops out of the signal flow entirely. That holds equally for Live‘s own built-in effects devices and for outside VST and AU plug-ins. As a result, the audio leaving a bypassed effect is the same as the audio that entered it. Be aware, though, that effects devices whose parameters fundamentally demand delay — the Lookahead settings in Compressor are one example — keep imposing that delay even while bypassed, so automatic delay compensation across the rest of the project stays intact. Usually this has no audible consequence whatsoever.

To test that bypassed effects are neutral, we drop a single instance of every Live effects device onto an audio track, switch them all off, and render the track‘s output. We then set that render beside the render of the same track carrying no devices at all. Phase cancellation between the two files proves they are identical.

### 38.2.9 Routing

Moving signals around through Live‘s [routing](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) is a neutral operation. Whatever arrives at the routing destination matches what left the routing source exactly. Keep in mind, however, that Live‘s adaptable routing setup opens up many possibilities — pulling a signal from before or after a given track‘s effects or mixer, or tapping the output of separate sample slots inside the Impulse instrument, among others. Under those arrangements, the signal you hear at the destination will probably differ from what you‘d hear ahead of routing, because the tap was placed somewhere short of the end of its original signal chain.

### 38.2.10 Splitting Clips

A clip that is already neutral stays neutral once you [split](https://www.ableton.com/en/live-manual/12/arrangement-view/#splitting-clips) it. The split changes only where playback sits inside the sample; the underlying sample data is left untouched. Crossing a split boundary during playback is seamless and sample-accurate.

We put clip splitting through a range of conditions to confirm it stays neutral:

- Splitting unwarped clips with loop on and off.
- Splitting warped but unstretched clips with loop on and off.

For every one of these, the output is rendered and held up against the render of an unsplit copy of the same source. Phase cancellation between the two files shows they are identical.

### 38.3 Non-Neutral Operations

Any Live procedure that alters audio quality is called a _non-neutral operation_. Anyone using these can count on at least some modification to the signal. Run a non-neutral operation on files brought into Live and the imported audio will no longer match the versions stored on disk. Run one while exporting from Live and what reaches your ears during real-time playback will diverge from what lands in your new file.

The non-neutral operations are laid out below.

### 38.3.1 Playback in Complex and Complex Pro Mode

The [Complex](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#complex-and-complex-pro-mode) and [Complex Pro](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#complex-and-complex-pro-mode) Warp Modes rest on a completely separate technology from the algorithms driving Beats, Tones, Texture, and Re-Pitch modes. The Complex modes can deliver a better sound — especially on mixed sound files holding several types of audio material — yet they are never neutral, not even when the tempo is left unchanged. For that reason, together with the heavier CPU load these algorithms carry, we suggest reaching for them only when the other Warp Modes fail to give satisfactory results.

### 38.3.2 Sample Rate Conversion/Transposition

Converting the sample rate — whether in real-time playback or while rendering — is non-neutral. Playing back audio files whose sample rate differs from the figure set in Live‘s Settings window degrades the signal. Transposition is itself a kind of sample-rate conversion, so it likewise behaves non-neutrally.

To hold down any harm during real-time playback, the advice is to handle sample rate conversion offline instead of mixing files of varying sample rates inside one Set. After you‘ve exported the samples at whatever sample rate you intend to use in Live, you can import those files with no quality loss at all.

Rendering audio out of Live at a sampling rate other than the one you used throughout the project is also non-neutral. The sample rate conversion that happens during export relies on the outstanding [SoX Resampler](https://soxr.sourceforge.net) library, licensed under the [GNU LGPL v2.1](https://gnu.org/licenses), producing downsampled files with remarkably low distortion.

### 38.3.3 Volume Automation

Automating the volume level shifts the gain, which by definition makes it non-neutral. Some ways of implementing automation envelopes, however, can throw off audible artifacts — especially when those envelopes aren‘t recalculated quickly enough. In Live, the volume automation curves refresh once per audio sample, so the distortion stays extraordinarily low.

### 38.3.4 Dithering

Any time you render audio down to a lower bit depth, applying dithering is wise as a way to hold artifacts in check. Dithering — essentially a very faint layer of noise — is non-neutral by nature, but it‘s an unavoidable trade-off when you drop the bit resolution.

Bear in mind that Live processes every internal signal at 32-bit, so even one gain change turns the resulting audio into 32-bit material as well, regardless of whether the original was 16- or 24-bit. Because dither must never be applied to the same audio file more than once, the safest course — unless you‘re mastering and finalizing within Live — is to render at 32-bit every time and skip dithering completely.

### 38.3.5 Recording External Signals (Bit Depth < A/D Converter)

Capturing audio into Live turns non-neutral whenever the bit depth chosen in Live‘s Settings window sits below that of the A/D converters supplying the recording. We advise against doing this.

### 38.3.6 Recording Internal Sources Below 32 Bit

Whenever you capture material through internal routing at any bit depth under 32 bits, quality suffers. To keep captures of plug-in instruments — and of any signal moving through effects plug-ins — neutral, the recommendation is to record internally at 32 bits. Still, note that if the source is already at a lower bit depth, an internal recording at that same depth remains neutral as well (provided no effects are involved); pushing an untouched 16 bit file up to 32 bits during internal recording will not raise its sound quality.

### 38.3.7 Consolidate

[Consolidating clips](https://www.ableton.com/en/live-manual/12/arrangement-view/#consolidating-clips) in the Arrangement View produces fresh audio files that are non-neutral relative to the source audio data. In particular, those new files are normalized, and their clip volumes get trimmed so playback matches the loudness you heard before consolidating. Since normalization adjusts gain, it is a non-neutral operation. Beyond that, the new files take on whatever sample rate and bit depth Live‘s Settings window specifies, which can be different from the values in the original audio files.

### 38.3.8 Clip Fades

With Create Fades on Clip Edges switched on under the Record, Warp & Launch Settings, Live lays a brief fade — no longer than 4 ms — across the clip‘s start and end to head off clicks at those boundaries. You can also bring these “declicking“ fades to Session View clips through the [Clip Fade](https://www.ableton.com/en/live-manual/12/clip-view/#clip-start-and-end-fades) button. On top of that, Arrangement View clips offer [editable fades and crossfades](https://www.ableton.com/en/live-manual/12/arrangement-view/#audio-clip-fades-and-crossfades). Any of these fade options is non-neutral once applied.

### 38.3.9 Panning

Panning in Live follows a constant power scheme built on sinusoidal gain curves. At the center position the output sits at 0 dB, while a signal panned hard left or right gains +3 dB. To keep that level shift in check, it can help to tighten the overall stereo width ahead of any extreme panning, which you accomplish through the Width control in the Utility device.

### 38.3.10 Grooves

In the majority of cases, playing a warped clip whose tempo lines up with the Set is neutral. Add a [groove](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves), though, and the playback turns non-neutral at every tempo.

### 38.4 Tips for Achieving Optimal Sound Quality in Live

If you‘re aiming for the best possible audio quality in Live, here is a set of suggested habits and program settings to follow.

- Settle on a project‘s sample rate before you start working, instead of switching it partway through the project.
- Track audio into Live with top-tier hardware — a good audio interface, quality cables, and so on — and at the steepest sample rate and bit depth your interface and machine can handle.
- Steer clear of mixing samples of differing sample rates inside one project. Should you need such files, convert them first to the sample rate your audio interface is set to, using an offline tool built for the job.
- Switch off both the Warp and Fade options in the Clip View for every audio clip.
- Leave the Transpose and Detune controls alone on all clips.
- Always render at 32-bit.

Keep in mind that while these habits secure the cleanest audio, they also turn off parts of Live‘s functionality — stretching and synchronization in particular.

### 38.5 Conclusion

Our hope is that this gives people a clear picture of precisely how their audio changes as they carry out the various procedures in Live. We‘ve concentrated on the functions that over the years have most often sown confusion or doubt, and the rosters of neutral and non-neutral operations shown here are, by their nature, far from exhaustive.
