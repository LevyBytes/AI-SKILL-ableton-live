# Audio Envelope Pitch Volume And Rhythm

Open when you need guidance on Audio Envelope Pitch Volume And Rhythm in Ableton Live.

Context: [Audio Clip Envelopes](clip-envelopes.md#262-audio-clip-envelopes).

<a id="source-2621-clip-envelopes-are-non-destructive"></a>
### 26.2.1 Clip Envelopes are Non-Destructive

Clip envelopes let you sculpt fresh sounds out of a sample while leaving the file on disk untouched. Since Live works out the envelope modulations as it plays, a single Live Set can hold hundreds of clips that each sound distinct yet all draw on one shared sample.

Naturally, a sound you've just built can be saved out by [rendering](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video) or through [resampling](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips). Within the Arrangement View, the [Consolidate command](https://www.ableton.com/en/live-manual/12/arrangement-view/#consolidating-clips) lets you generate new samples.

<a id="source-2622-changing-pitch-and-tuning-per-note"></a>
### 26.2.2 Changing Pitch and Tuning per Note

Pull a sample loop out of the browser and drop it into Live, confirm the [Warp switch](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping) is on, then start the clip playing. Pick “Clip” in the Device chooser along with “Transposition” in the Control chooser. From here you're free to shift the pitch transposition of single notes within the sample while it plays back.

The quickest route is to switch on [Draw Mode](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-envelopes) and lay down steps that follow the grid. Turn Draw Mode back off whenever you need to tweak breakpoints and line segments — handy for softening the blocky steps by shifting breakpoints sideways.

The Transposition Envelope with Steps (Top) and Ramps (Bottom).

Keep in mind that your warp settings govern how faithfully Live's time-warping engine follows the contour of the envelope. For snappier tracking, lower the Grain Size value when in Tones or Texture Mode, or set a smaller Granulation Resolution while in Beats Mode.

When fine-tuning the pitch of single notes in the sample, hold the Shift modifier as you draw or reposition breakpoints to gain a finer resolution.

To move the display around, keep the Ctrl+Alt (Win) / Cmd+Option (Mac) modifier held while you drag.

The modulation applied to pitch works _additively_: the transposition envelope's output is just summed onto the value of the Transpose control. Whatever the modulation produces is then clamped so it remains within the permitted span (-48..48 semitones here).

<a id="source-2623-muting-or-attenuating-notes-in-a-sample"></a>
### 26.2.3 Muting or Attenuating Notes in a Sample

Choose “Clip” in the Device chooser together with “Gain” in the Control chooser. Whether you lay steps down in Draw Mode or sculpt contours using breakpoints, you can stamp any volume shape you like onto the sample.

Imposing a Volume Envelope on a Sample.

Live reads the volume envelope's output as a relative percentage of wherever the Clip Gain slider currently sits. For that reason the clip envelope's modulation is never able to climb past the absolute volume setting, though it can pull the audible level all the way down to silence.

<a id="source-2624-scrambling-beats"></a>
### 26.2.4 Scrambling Beats

A particularly inventive application of clip envelopes is modulating the sample offset. This kind of modulation is best suited to rhythmic material and is offered only for clips configured to play back in the Beats Warp Mode.

Give sample offset modulation a go using a one-bar drum loop: confirm Beats Mode is selected, then in the Envelopes tab pick “Clip“ from the Device chooser and “Sample Offset“ from the Control chooser. A vertical grid overlay shows up across the Envelope Editor. With the envelope's Draw Mode active, push steps to non-zero values and you'll hear the loop come apart. So what's actually happening?

Picture a tape head reading the audio, with the envelope steering where that head sits. As the envelope's value climbs, the head drifts further from its resting center. A positive envelope value pushes the head toward the “future,“ while a negative one pulls it back into the “past.“ Helpfully, Live measures this modulation in beats instead of centimeters: each vertical grid line stands for a sixteenth note of offset, and the modulation can swing from plus eight sixteenths down to minus eight sixteenths.

When you want to whip up engaging variations on beat loops in a hurry, sample offset modulation is the go-to. We'd steer you away from it for “analytical“ cut-and-splice jobs, though; those go far more smoothly in Live's Arrangement View, where the outcome can be consolidated into new clips without fuss.

Repeating Steps and Slowing Time with the Sample Offset Envelope.

Certain sample offset envelope gestures yield a signature result: a descending “escalator“ shape, say, essentially loops back the step found at the start of the envelope. In the same vein, a gentle downward-sloping ramp drags time out and yields pleasant smearing effects whenever the slope sits just shy of 45 degrees; give it a try at a 1/32 Granulation Resolution.

<a id="source-2625-using-clips-as-templates"></a>
### 26.2.5 Using Clips as Templates

The more creatively you employ clip envelopes, the more the host clips take on a character all their own, detached from whatever sample they began with. Sooner or later you may ask yourself: how would this clip sound built around some other sample? Finding out is simple — select the clip so it shows in the Clip View, then drag whichever sample you want from the browser, or from the Session or Arrangement View, onto that Clip View. Every clip setting, the envelopes included, stays exactly as it was; the only thing swapped out is the sample.
