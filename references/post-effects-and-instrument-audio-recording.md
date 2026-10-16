# Post Effects And Instrument Audio Recording

Open when you need guidance on Post Effects And Instrument Audio Recording in Ableton Live.

Context: [Making Use of Internal Routing](routing-and-i-o.md#1752-making-use-of-internal-routing).

<a id="source-17521-post-effects-recording"></a>
#### 17.5.2.1 Post-Effects Recording

Picture yourself sending a guitar into Live, assembling a song one track at a time, stacking take upon take. Granted, keeping a distinct effects chain on each track — so you can apply different effects to different takes after the fact — is powerful. Even so, you may prefer to pass the guitar signal through effects (a noise gate or an amp model, perhaps) _before_ it ever gets recorded, then capture the post-effects signal.

An Example Setup for Post-Effects Recording.

Pulling this off is simple: set aside a dedicated audio track that processes and monitors the arriving guitar signal. We name that track “Guitar“ and drop the effects we want into its device chain. Rather than record straight into the Guitar track, we spin up a couple of extra tracks for recording. Each of those is configured to take its input Post FX from the Guitar track. Note that tapping the Guitar track Post Mixer would be an option too, should we want to capture any of its level or panning.

On the monitoring side, the Guitar track’s Monitor radio button goes to In, since we always want our guitar audible through this track regardless of whatever else Live is doing. The remaining tracks’ Monitor radio buttons go to Off.

<a id="source-17522-recording-midi-as-audio"></a>
#### 17.5.2.2 Recording MIDI as Audio

While dealing with MIDI alongside elaborate software instruments, capturing the audio that results can sometimes beat capturing the MIDI going in. One lone MIDI note might, for instance, drive Native Instruments’ _Absynth_ to generate something closer to a passage of music than to a single tone. Such output suits depiction as an audio waveform far better than a solitary note in a MIDI clip, all the more so once you weigh the editing options.

Recording the Output of a Complex Instrument in Audio Tracks.

An arrangement much like the one [described above](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#post-effects-recording) gets the job done. A single MIDI track holds the virtual instrument, and one more audio track captures the audio output while the instrument plays.
