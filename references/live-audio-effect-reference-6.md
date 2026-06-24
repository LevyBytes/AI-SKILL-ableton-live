# Live Audio Effect Reference (part 6)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

- Damping sets how much treble gets rolled off inside the reverb algorithms; turn it up and the resulting reverberation grows darker in tone.
- Lo Damp governs how much of the bottom end is filtered out by the reverb algorithms; raising it yields brighter-sounding reverberation.
- Mod determines how much motion occurs within the tail produced by the algorithm. Dialing modulation down quiets that motion, whereas raising it introduces a chorus-like sweep and simultaneously softens any resonant buildup.
- Diffusion sets how thick the algorithm’s tail becomes. Lower settings thin the tail out, and as you raise the value the tail grows progressively denser.
- Distance places the reflections at a simulated remove. Pull it down and the reflections sit nearer the listener, packed more tightly together; push it up and they retreat into the distance, spacing the echoes farther apart in time.

#### 28.23.4.3 Shimmer

A tight stack of diffuse delays feeding a pitch shifter in the loop forms the basis of the Shimmer reverb algorithm. At low diffusion you hear a clean delay, whereas cranking diffusion high yields a thick, rich synthetic reverb. By blending the pitch-shifted output back into the feedback path, the Shimmer effect produces tails that drift upward or downward in pitch.

Alongside the common parameters described earlier, Shimmer adds these controls:

- Damping sets how much treble gets rolled off inside the reverb algorithms; turn it up and the resulting reverberation grows darker in tone.
- Mod determines how much motion occurs within the tail produced by the algorithm. Dialing modulation down quiets that motion, whereas raising it introduces a chorus-like sweep and simultaneously softens any resonant buildup.
- Pitch sets, in semitones, how far the feedback signal is shifted up or down.
- Diffusion sets how thick the algorithm’s tail becomes. Lower settings thin the tail out, and as you raise the value the tail grows progressively denser. Drop it under 10% for dub-style delay textures. It’s a blast on drums!
- Shimmer governs how strong the Shimmer effect is. At 0% there is no pitch shifting at all, and the pitched layer grows steadily louder as you push the percentage higher. On melodic parts, dialing Shimmer up to 100% gives you striking harmonized pitches.

When Shimmer mode is active, the Size knob controls the spacing between the separate echoes heard on percussive sources.

#### 28.23.4.4 Tides

By pairing a smooth reverb with a multiband filter that sweeps across the output spectrum, the Tides algorithm conjures up rippling, frequency-banded textures.

Beyond the common parameters covered above, Tides offers the following:

- Damping sets how much treble gets rolled off inside the reverb algorithms; turn it up and the resulting reverberation grows darker in tone.
- Wave reshapes the modulation curve of the filter, sweeping it from noise (0%) through sine (50%) and on to square (100%).
- Tide controls how pronounced the texture from the tail’s modulation becomes.
- Phase sets how far apart the left and right modulation waveforms are offset from one another. Dial in 180° and the two channels sit completely out of phase.
- Rate fixes how fast the modulation oscillator runs, expressed in beat divisions that include Triplet, 16th, and Dotted note value variants.

#### 28.23.4.5 Prism

Built on velvet (spectrally flat) noise, the Prism algorithm delivers a distinctive, brilliant, synthetic-sounding diffuse reverb. You can readily deploy it as a “ghost” reverb that lends depth without stepping on the original material. It shines on short, non-linear decays for drums and transients, yet it works just as well on sustained sources with longer decays where you want a tidy but clearly digital character.

On top of the common parameters listed earlier, Prism contributes these:

- Low Mult stretches or shrinks how long the low end of the reverb tail takes to decay.
- High Mult stretches or shrinks how long the top end of the reverb tail takes to decay.
- X over sets where the split between the tail’s low- and high-frequency regions falls, thereby determining which frequencies the Low Mult and High Mult parameters act upon.

Tip: To nail that vintage ‘80s gated-snare-reverb sound, keep the Decay and Size values on the small side.

### 28.23.5 EQ Section

Hybrid Reverb’s EQ Section.

You’ll find Hybrid Reverb’s EQ section on the device display’s second tab. A single click on the tab’s toggle button turns it on or off in an instant.

Out of the box, the EQ sits downstream of both reverb engines in the chain; flip the Pre Algo button, though, and it moves ahead of the algorithmic reverb no matter which reverb routing you’ve selected.

You get four control bands for sculpting the reverb signal further. Each of the low and high bands can switch between a pass filter and a shelving EQ. In low-pass or high-pass mode, those filters offer slopes spanning anything from a mild 6 dB/octave up to an aggressive 96 dB/octave. The pair of peak EQs in the middle reach across the whole spectrum, handling everything from broad boosts to fairly tight cuts.

### 28.23.6 Output Section

A closing group of parameters in Hybrid Reverb’s output section lets you fine-tune how the device sounds as a whole.

Stereo dials in the stereo width of the wet signal. At 0% you get a mono output, while pushing past 100% spreads the panorama into a wider-than-stereo image.

Pushing the Vintage slider up progressively roughens Hybrid Reverb’s sound by mimicking the reduced sample rates and bit-depths typical of old-school digital reverb units. There are four presets that dramatically reshape the character: Subtle, Old, Older, and Extreme.

Bass Mono folds any of Hybrid Reverb’s output below 180 Hz down to mono, tightening up the low end.

The Dry/Wet control balances the wet, processed sound against the untreated signal. Push it to 100% whenever Hybrid Reverb sits on a return track.

### 28.24 Limiter

The Limiter Effect.

The Limiter effect is a mastering-grade dynamics processor that keeps your output from rising past a level you choose. It works especially well on the Main track, where it stops digital-to-analog converters from clipping. At its core, a limiter is just a compressor whose ratio is infinite. To read up on the theory behind compression, head to the [Compressor](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#compressor) section.

The Limiter display holds the Ceiling control plus the Gain Reduction meter. With the Ceiling control you set the highest level the device is ever allowed to put out. Should none of the incoming peaks rise above that ceiling, the device leaves the signal untouched.

How much gain reduction is taking place once the signal hits the ceiling or threshold is shown by the Gain Reduction meter.

The Link control governs the degree to which Limiter’s gain reduction is shared between its two channels, which may be left/right or mid/side depending on the Routing Mode you’ve chosen. At 100%, whenever either channel calls for compression both are reduced together, holding the stereo image steady. At 0%, each channel is handled on its own and can receive a different amount of reduction. That independence comes in handy with signals whose left and right sides are unrelated, or for creative tricks like a “wobble” across the stereo field.

To the left of the display, the Input Gain knob lets you raise or lower the level of the incoming signal before any limiting takes place.

Engaging the Maximize toggle beneath the Input Gain knob swaps the Ceiling control for Threshold, giving you a single knob to tune both the loudness and the dynamic range of the signal. Pulling the Threshold down boosts the limiter stage’s output by the negative of whatever Threshold value you set. Keep in mind that with Maximize active the Input Gain knob turns into the Output control, which fixes the device’s intended output level.

With the Release knob you set how quickly the device eases off limiting once the signal drops back under the ceiling or threshold. Quick release values produce a louder, more aggressive result, whereas longer ones sound smoother but may shrink the dynamic range. You can watch the Release control at work on the Gain Reduction meter: short releases send the meter snapping back to zero, while longer ones let it ease down gradually as Limiter holds the compression in place for a while longer.

Flip the Auto toggle under the Release knob to switch on auto-release. With it engaged, Limiter studies the incoming audio and keeps adapting its release time to whatever the signal is doing. Bear in mind that the Release control goes inactive while auto-release is running.

Sitting to the right of the display, the Lookahead control governs how fast Limiter reacts to peaks that need compressing. You can set the lookahead time to 1.5, 3, or 6 milliseconds. A briefer lookahead permits heavier compression but may add distortion, particularly on low-frequency material. Because lookahead feeds into Limiter’s attack time, longer settings are handy for snagging extremely fast peaks. Do note that lookahead adds latency, and the larger the value, the more latency you incur.

Three ceiling modes are available via the Ceiling Mode toggles: Standard, Soft Clip, and True Peak. Standard is what the device uses by default. Soft Clip applies gentle clipping as signals near the ceiling, lending transients a touch of warmth and punch. With Soft Clip engaged, an LED above the mode toggles lights up and blinks whenever the signal clips. True Peak, lastly, guards against inter-sample peaks.

The Routing Mode toggles control how Limiter handles peaks that land on just one side of the stereo signal. Under L/R mode, the left and right channels are limited separately, letting the device clamp down harder at the cost of some stereo-image smearing. Under M/S mode, Limiter converts the signal to mid/side ahead of limiting and then converts it back to stereo on the way out; this keeps the stereo image intact but adds latency.

Bear in mind that tacking on any further effects downstream of Limiter can reintroduce gain. To guarantee your finished mix never clips, make Limiter the final link in the Main track’s device chain and keep that track’s volume under 0 dB.

### 28.25 Looper

The Looper Effect.

Modeled on the classic real-time looping units, Looper is an audio effect that lets you capture and loop audio while stacking up endless overdubs locked to your Set. When the Set isn’t playing, Looper can study the audio coming in and snap Live’s tempo to it. You may also fix a loop length ahead of recording, and Live’s tempo will shift so the loop lands inside the bar count you asked for. On top of that, you can pull audio into Looper as a bed beneath fresh overdubs, or push the contents of Looper out as a brand-new clip.

A roomy display fills the upper portion of Looper’s interface, laid out for at-a-glance reading on stage. The whole display floods red while you’re recording. Once recording stops, it reports where you are in the loop along with the full loop length counted in bars and beats.

Looper’s transport buttons behave much like Live’s other transport controls. Pressing Record captures incoming audio until you hit another button, wiping out whatever Looper was holding. Overdub keeps piling on fresh layers of input, each matching the length of the first recorded pass. Play sounds out Looper’s buffer as it currently stands without laying down anything new, and Stop halts playback.

How the transport controls act hinges on whether Live is currently playing back. While the transport rolls, Looper acts like a clip and obeys launch quantization set by the [Quantization chooser](https://www.ableton.com/en/live-manual/12/live-concepts/#recording-new-clips). With Live’s playback halted, Looper’s transport fires the moment you trigger it, ignoring the Quantization value.

Hitting Clear wipes Looper’s buffer. Press it during Overdub while the transport is rolling and the buffer empties out, yet the tempo and length stay put. Press Clear in any other state and both tempo and length reset.

The Undo button removes everything overdubbed since the last time you switched Overdub on. Whatever you captured originally, together with anything overdubbed on an earlier pass, stays intact. Once you’ve hit Undo, the control flips to Redo, which restores the material the last undo took away.

Beneath the transport controls sits the larger Multi-Purpose Transport Button. Like the standard transport buttons, what it does shifts with Looper’s present playback state and with whether anything has been recorded yet. With an empty buffer, one click begins recording. While Looper is recording, overdubbing, or stopped, one click flips it into play mode. Mid-playback, a click drops you into overdub mode, and further single clicks let you bounce between overdub and playback at will.

A quick double-press of the button stops Looper from either play or overdub mode. Holding it down for two seconds during playback triggers Undo or Redo. Holding for two seconds while stopped wipes Looper’s buffer.

Diagram of Looper’s Multi-Purpose Transport Button Behavior.

The Multi-Purpose Transport Button is built with a MIDI footswitch in mind. To map a footswitch, switch into [MIDI Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#assigning-midi-remote-control), click the button, and step on your connected footswitch. After that, leave MIDI Map Mode.

How Looper works out the tempo of recorded material is governed by the Tempo Control chooser:

- _None_: Looper keeps its own internal tempo, unaffected by Live’s global tempo.
- _Follow song tempo_: Looper’s playback rate is shifted so the recording sounds at Live’s global tempo.
- _Set & Follow song tempo_: Live’s global tempo is nudged to match the tempo of whatever you recorded into Looper. From then on, any change you make to Live’s global tempo retimes Looper’s playback so the recording follows the new global tempo.

You set how long Looper records with the Record Length chooser. What it does varies with whether Live’s global transport is rolling and, subject to the Tempo Control chooser’s state, it can drive Live’s global tempo:

- _Song running_: With Looper’s Record Length chooser left at its default ”x bars,” recording continues until you tap another transport button. Pick a set bar count from the chooser instead, and Looper records for exactly that span before flipping to Play or Overdub, whichever the button beside the chooser specifies.
- _Song not running_: With the Record Length chooser sitting at the default ”x bars,” Looper estimates the tempo of your take the instant you press Overdub, Play, or Stop. That guess can land at double or half the speed you intended, though. Lock in a fixed bar count up front and Looper’s tempo bends so your recording fills that span.

What effect Looper’s transport controls have on Live’s global transport comes down to the Song Control chooser:

- _None_ leaves Live’s global transport untouched by Looper’s transport controls.
- _Start Song_ fires Live’s global transport every time Looper moves into Play or Overdub mode, while Looper’s Stop button does nothing to the global transport.
- _Start & Stop Song_ chains Live’s global transport to Looper’s transport controls. Stepping into Play or Overdub launches Live’s transport, and tapping Looper’s Stop button halts it.

Kicking off Live’s transport through Looper also realigns the playback position of any apps linked over [Ableton Link](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#setting-up-link). That keeps those apps locked to tempo and parked at the right spot in the musical phrase.

Pressing the ”×2” button doubles how long Looper’s recording buffer runs. Whatever you’ve already laid down is simply copied across. That lets you, say, capture a run of one-bar ideas and then layer a run of two-bar ones over them. Looper shows the buffer’s length and tempo in the display area.

In the same vein, the ”÷2” button halves the current buffer’s length, keeping the half that’s playing right now and throwing away the rest.

Through the ”Drag me!” spot in the display you can save Looper’s buffer out as a fresh audio file. Drag and drop it onto the browser or straight onto a track to spawn a new clip, whose Warp Mode defaults to [Re-Pitch](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#re-pitch-mode). You can equally drag audio files onto the ”Drag me!” spot to swap out whatever Looper currently holds, then build further overdubs on top of that bed.

The Speed knob changes how fast Looper plays back, and therefore its pitch. The up and down arrows on its left are quick ways to shift pitch by full octaves, which doubles or halves the playback rate. Those buttons obey the Quantization chooser setting.

Switch on the Reverse button and the material you recorded earlier plays in reverse. Anything you overdub once Reverse is on will play forward. Keep in mind that turning Reverse back off flips this around: the original take resumes playing forward, while whatever you overdubbed with Reverse engaged now plays backward. Toggling the Reverse button obeys the Quantization chooser setting.

Feedback determines how much of the already-recorded signal loops back into Looper as you overdub. At 100%, the earlier material holds its volume forever. At 50%, it drops to half its level on every pass. Tweaks to Feedback only kick in on the following repetition. Note too that Feedback does nothing in Play mode, where each pass stays at a constant volume.

For monitoring Looper’s input, the Input -> Output chooser gives you four choices:

- _Always_ lets the input be heard no matter whether Looper is playing or recording. Always is usually what you want with Looper as an insert effect on a single track.
- _Never_ keeps the input from ever being heard. Reach for Never when Looper sits on a return track that’s fed by sends from a range of other tracks.
- _Rec/OVR_ makes the input audible only while recording or overdubbing, never during Play mode or while stopped. That suits setups where you’re routing audio to several tracks, each holding its own Looper. Give each of those Loopers its own foot pedal and you can flip its record and playback states while playing, with no need to fuss over monitoring.
- _Rec/OVR/Stop_ lets the input through at all times except during play mode. It resembles the Insert mode of [Beat Repeat](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#beat-repeat) and works well for capturing parts that abruptly cut into your live performance.

### 28.25.1 Feedback Routing

For [internal routing](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#internal-routings) to other tracks, Looper can serve as both a source and a destination. With this you could, for instance, build Looper overdubs that keep cycling back through the devices on another track. Here’s how to wire it up:

1. Insert Looper on a track.
2. Record at least one pass of material into Looper.
3. Create another audio track.
4. Set the new track’s upper Audio From and Audio To choosers to the track that holds the Looper.
5. Set the new track’s lower Audio From and Audio To choosers to ”Insert-Looper.”
6. Flip the new track’s Monitoring to ”In.”
7. Drop further effects devices into that new track’s device chain.
8. Put Looper into Overdub mode.

From here, Looper’s signal travels out through the other track’s device chain and loops back into Looper itself, so each pass piles on more heavily processed overdub layers.

### 28.26 Multiband Dynamics

The Multiband Dynamics Effect.

The Multiband Dynamics device gives you a versatile way to reshape the dynamic range of your audio. Built first and foremost for mastering duties, it can apply both upward and downward compression as well as expansion across as many as three separate frequency bands, each with its own adjustable crossover points and envelope controls. Because every band carries both an upper and a lower threshold, you can run two different kinds of dynamics processing on it at once.

### 28.26.1 Dynamics Processing Theory

Getting the most out of the Multiband Dynamics device is easier once you grasp the four distinct ways dynamics can be shaped.

“Compression” usually refers to pulling down the level of any signal that climbs past a threshold. That’s exactly what Live’s [Compressor](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#compressor) does, and the more precise name for it is _downward compression_, since it pushes the loud parts down and so narrows the dynamic range. Yet you can shrink the dynamic range the other way too, by lifting the level of signals that sit _below_ a threshold. That far rarer variety goes by the name _upward compression_. The diagram makes it clear that whichever flavor you reach for, the result is a signal with a tighter dynamic range than you started with.

Downward and Upward Compression.

Expansion is compression’s mirror image. A standard expander drops the level of signals falling beneath a threshold. Live’s [Gate](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#gate) operates this way, and is more properly termed _downward expansion_, because it pushes the quiet bits down and thereby widens the dynamic range. You can also stretch the dynamic range by boosting signals that rise _above_ a threshold. Mirroring upward compression, this approach is called _upward expansion_ and shows up far less often. The diagram illustrates that either kind of expansion leaves you with a wider dynamic range.

Downward and Upward Expansion.

In short:

- Downward compression (common): make loud signals quieter
- Upward compression (uncommon): make quiet signals louder
- Downward expansion (common): make quiet signals quieter
- Upward expansion (uncommon): make loud signals louder

Every one of these processing types is on offer in the Multiband Dynamics device. Since it splits the incoming audio into three frequency bands and gives each band an upper plus a lower threshold, one instance of Multiband Dynamics can run six kinds of dynamics processing all at the same time.

### 28.26.2 Interface and Controls

Toggling the high and low bands on or off is done with the High and Low buttons. Switch both off and the device collapses to a single-band effect, where only the Mid controls touch the signal. Sitting under the High and Low buttons, the frequency sliders move the crossovers that mark out each band’s range. Say the low frequency reads 500 Hz and the high frequency reads 2000 Hz: the low band then spans 0 Hz to 500 Hz, the mid band 500 Hz to 2000 Hz, and the high band runs from 2000 Hz on up to whatever ceiling your soundcard or sample rate allows.
