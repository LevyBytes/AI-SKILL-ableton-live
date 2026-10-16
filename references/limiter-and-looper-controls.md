# Limiter And Looper Controls

Open when you need guidance on Limiter And Looper Controls in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2824-limiter"></a>
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

<a id="source-2825-looper"></a>
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
