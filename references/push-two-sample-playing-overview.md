# Push 2 Sample Playing Overview

Open when you need guidance on Push 2 Sample Playing Overview in Ableton Live.

Context: [Using Push 2](push-two-setup-and-playing-routes.md#35-using-push-2).

<a id="source-358-working-with-samples"></a>
### 35.8 Working with Samples

There are many ways to trigger samples from the pads on Push 2, with thorough yet approachable command over sample parameters straight from the encoders and display. Simpler is the instrument behind Push 2’s sample playback, and it's worth working through the in-depth [Simpler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#simpler) chapter to get the full picture of what it does.

You can begin with a sample by either creating a fresh MIDI track or pressing Browse to drop into Browse Mode on a MIDI track you already have. An empty Simpler can be loaded onto a track, but nothing plays until a sample is present. Push 2’s display lets you know the Simpler holds no sample and nudges you to go browse for one:

Press Browse to Load a Sample in an Empty Simpler.

Once a sample is loaded and you flip to Device View, the sample’s waveform appears on Push 2’s display next to several parameters for rapidly tuning how playback behaves. This is Simpler’s main control bank.

Simpler’s Main Parameter Bank in the Display.

Out of the box, Simpler picks certain parameter settings on its own according to how long the loaded sample is. Short samples, for instance, fire once per trigger, whereas long ones are set to loop and _warp_. A warped sample plays at your Set's tempo no matter which note you hit. Drag a warped clip into Simpler — out of an audio track, from the browser, or off your desktop — and it retains whatever warp settings and markers the source clip carried. The [Audio Clips, Tempo, and Warping](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#audio-clips-tempo-and-warping) chapter goes deeper on warping.

The Mode control is the key parameter steering how Simpler handles samples, since it picks which of Simpler’s three playback modes is in effect.

Simpler’s Mode Parameter.

- _Classic Playback Mode_ is Simpler's out-of-the-box choice, tuned toward building “conventional” melodic and harmonic instruments from pitched samples. A full ADSR envelope is on board and looping is supported, letting a sample hold for as long as the note stays down. Classic Mode runs polyphonic by default, and its pad grid follows the same layout used for other pitched instruments.
- _One-Shot Playback Mode_ plays back monophonically only and is geared toward one-shot drum hits or brief sampled phrases. Its envelope controls are pared down and looping isn't supported. By default a triggered note plays the whole sample no matter how briefly the note is held. One-Shot Mode's pad grid sticks with the melodic layout too.
- _Slicing Playback Mode_ cuts the sample into pieces non-destructively so each slice becomes playable from the pads. Slices can be made and shifted by hand, or you can pick from several schemes that have Simpler generate them automatically. This mode suits rhythmic drum breaks especially well.
