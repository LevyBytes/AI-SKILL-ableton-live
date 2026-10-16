# Neutral Audio Operations

Open when you need guidance on Neutral Audio Operations in Ableton Live.

Context: [Neutral Operations](audio-fact-sheet.md#382-neutral-operations).

<a id="source-3821-undithered-rendering"></a>
### 38.2.1 Undithered Rendering

The [Export Audio/Video](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video) command writes Live’s audio output to a disk file. Provided certain criteria hold, this rendering counts as a neutral operation:

- The rendered file carries the same sample rate that the audio hardware uses in Live‘s Settings.
- Nothing non-neutral has been applied along the way.

To gauge Live‘s rendering, we feed it three categories of unprocessed material — white noise, fixed-frequency sine waves and sine sweeps — at 16-, 24- and 32-bit word lengths, then render each one out, again at assorted bit resolutions. Running phase cancellation between the source material and the rendered results yields this:

- Render at the same bit depth as the source, and the two cancel completely.
- Render at a bit depth above the source, and you again get complete cancellation.
- Render at a bit depth beneath the source, and the distortion introduced is as small as a 32-bit system can manage.

<a id="source-3822-matching-sample-rateno-transposition"></a>
### 38.2.2 Matching Sample Rate/No Transposition

When Live plays an unstretched audio file, that playback is neutral as long as the file‘s sample rate matches what Live‘s Settings specify and no transposition is applied during playback. Cancellation tests on rendered output confirm this. Bear in mind that “playback“ here means strictly the audio inside Live, before it ever arrives at your audio hardware.

<a id="source-3823-unstretched-beatstonestexturere-pitch-warping"></a>
### 38.2.3 Unstretched Beats/Tones/Texture/Re-Pitch Warping

A clip whose tempo equals the tempo of the Set plays back without stretching. Under those conditions, as long as the clip‘s [Warp mode](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes) is Beats, Tones, Texture, or Re-Pitch — and not Complex or Complex Pro — its playback comes out neutral.

Whatever Warping results from altering the Set’s tempo is reversible: material that sounds unwarped at one tempo will keep sounding unwarped at that same tempo, even after the tempo is moved away and then brought back. Suppose you laid down several tracks at 120 BPM and later chose to drop the tempo to capture a tricky solo — once you restore the tempo to 120 BPM, those earlier tracks again play neutrally. The stretching applies solely to whatever you tracked at the reduced tempo.

Whether tempo automation captured in the Arrangement replays neutrally hinges on the Warp Mode. Turning on transient preservation with Beats mode can introduce artifacts; switching to preserve 16ths rather than transients, or moving to the Repitch Warp Mode, gets rid of them.

Keep in mind that [grooves](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves) operate by shifting where Warp Markers sit. As a consequence, any audio clip carrying a groove plays back non-neutrally, even at its native tempo.

Cancellation tests on rendered output establish that unstretched clip playback is neutral.

<a id="source-3824-summing-at-single-mix-points"></a>
### 38.2.4 Summing at Single Mix Points

Wherever Live combines signals — clip and return track inputs, the Main track, Racks — it sums them in double precision (64-bit). So at any individual summing point, the act of mixing in Live is neutral. We verify this by loading pairs of 24-bit files (white noise plus fixed-frequency sine waves alongside their phase-inverted counterparts), summing each pair together eight successive times, and rendering the result as 32-bit files. Every one of those tests produces flawless phase cancellation.

Note, though, that even though 64-bit summing covers each _single_ mix point, the rest of Live‘s internal processing remains at 32-bit. Because of that, a signal routed through several summing points may pick up a vanishingly small amount of degradation. Pairing 64-bit summing with a 32-bit architecture lands on an excellent compromise between sound quality and demands on CPU and memory.

<a id="source-3825-recording-external-signals-bit-depth--ad-converter"></a>
### 38.2.5 Recording External Signals (Bit Depth >/= A/D Converter)

Capturing audio into Live qualifies as neutral so long as the bit depth chosen in Live‘s Settings window meets or exceeds the bit depth of the A/D converters feeding the recording. In this setting, “neutral“ amounts to a bit-perfect match with whatever the A/D converters handed to Live.

<a id="source-3826-recording-internal-sources-at-32-bit"></a>
### 38.2.6 Recording Internal Sources at 32 Bit

Material captured through internal routing comes out identical to its source as long as you record at 32 bits. We advise recording internally at 32 bits whenever you want neutral captures of plug-in instruments or of any signal flowing through effects plug-ins. That said, when the source is already at a lower bit depth, recording internally at that very depth stays neutral too (presuming no effects are in play) — taking an untouched 16 bit file and recording it internally at 32 bits does nothing to improve its fidelity.

Cancellation tests confirm that internal recording is neutral.

<a id="source-3827-freezing-tracks"></a>
### 38.2.7 Freezing Tracks

Whenever you [freeze](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#track-freeze) tracks, Live writes the resulting audio files at 32 bit, guaranteeing they won‘t fall below the quality you heard before freezing. A handful of Freeze scenarios, though, behave non-neutrally and deserve mention:

A frozen Arrangement View track may carry sound that runs past the clip‘s own end — reverb tails, delay echoes, and the like. A frozen Session View track, by contrast, always spans precisely two loop cycles, so whatever audio would have spilled past two loop cycles during unfrozen playback gets truncated once the track is frozen.

For unfrozen clips, time-based effects such as reverbs and delays compute in real-time, which is why halting playback mid-tail lets that reverb or delay tail ring on. Frozen tails, on the other hand, have been baked into audio, so they cut off sharply when playback stops.

With frozen Arrangement View clips, every parameter automation is baked into the audio file. Frozen Session View clips instead capture a “snapshot“ of all parameter values as they stand at the Arrangement‘s 1.1.1 position and hold those for the whole length of the frozen clip. That mirrors how unfrozen clips work: while normal Session View clips play, any Arrangement automations stay “punched out“ until you click the Back to Arrangement button.

Live always replays frozen clips with Warp engaged in Beats mode, so they inherit exactly the same non-neutral characteristics as any other warped audio file.

Devices driven by random parameters — for instance, the Chance control found in the Beat Repeat device — stop behaving randomly once frozen. As with time-based effects, the random values present at the instant of freezing become part of the rendered file, so they are no longer recomputed in real-time.

<a id="source-3828-bypassed-effects"></a>
### 38.2.8 Bypassed Effects

When an effect in Live is bypassed, it drops out of the signal flow entirely. That holds equally for Live‘s own built-in effects devices and for outside VST and AU plug-ins. As a result, the audio leaving a bypassed effect is the same as the audio that entered it. Be aware, though, that effects devices whose parameters fundamentally demand delay — the Lookahead settings in Compressor are one example — keep imposing that delay even while bypassed, so automatic delay compensation across the rest of the project stays intact. Usually this has no audible consequence whatsoever.

To test that bypassed effects are neutral, we drop a single instance of every Live effects device onto an audio track, switch them all off, and render the track‘s output. We then set that render beside the render of the same track carrying no devices at all. Phase cancellation between the two files proves they are identical.

<a id="source-3829-routing"></a>
### 38.2.9 Routing

Moving signals around through Live‘s [routing](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) is a neutral operation. Whatever arrives at the routing destination matches what left the routing source exactly. Keep in mind, however, that Live‘s adaptable routing setup opens up many possibilities — pulling a signal from before or after a given track‘s effects or mixer, or tapping the output of separate sample slots inside the Impulse instrument, among others. Under those arrangements, the signal you hear at the destination will probably differ from what you‘d hear ahead of routing, because the tap was placed somewhere short of the end of its original signal chain.

<a id="source-38210-splitting-clips"></a>
### 38.2.10 Splitting Clips

A clip that is already neutral stays neutral once you [split](https://www.ableton.com/en/live-manual/12/arrangement-view/#splitting-clips) it. The split changes only where playback sits inside the sample; the underlying sample data is left untouched. Crossing a split boundary during playback is seamless and sample-accurate.

We put clip splitting through a range of conditions to confirm it stays neutral:

- Splitting unwarped clips with loop on and off.
- Splitting warped but unstretched clips with loop on and off.

For every one of these, the output is rendered and held up against the render of an unsplit copy of the same source. Phase cancellation between the two files shows they are identical.
