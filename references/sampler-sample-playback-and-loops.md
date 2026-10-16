# Sampler Sample Playback And Loops

Open when you need guidance on Sampler Sample Playback And Loops in Ableton Live.

Context: [The Sample Tab](sampler-zones-and-playback-routes.md#30106-the-sample-tab).

<a id="source-301061-sample-playback"></a>
#### 30.10.6.1 Sample Playback

Every parameter below operates together with the global volume envelope (located in the Filter/Global tab) to shape Sampler's fundamental voicing. Among other things, these envelopes rely on the familiar ADSR (Attack, Decay, Sustain, Release) parameters:

Envelope Attack Time (Attack) — Determines how long an envelope takes to climb from its initial level up to the peak level. You can reshape that climb with the Attack Slope (A. Slope) parameter.

Envelope Decay Time (Decay) — Determines how long an envelope takes to fall from the peak level down to the sustain level. You can reshape that fall with the Decay Slope (D. Slope) parameter.

Envelope Sustain Level (Sustain) — The level held once the envelope decay concludes. The envelope holds here right up until note release, unless it happens to be running in Loop, Sync or Beat Mode.

Envelope Release Time (Release) — How long an envelope takes to arrive at the end level once a Note Off message comes in. The Release Slope (R. Slope) value dictates the contour of this portion of the envelope.

Envelope Initial Level (Initial) — Determines where the envelope begins.

Envelope Peak Level (Peak) — The high point reached as the envelope attack finishes and the Decay stage gets underway.

Envelope End Level (End) — (LFO, Filter and pitch envelopes only) The level arrived at once the Release stage wraps up.

Envelope Rates < Velocity (Time < Vel) — This setting governs how much note velocity modulates the envelope segments. It becomes particularly engaging when the envelopes loop. Bear in mind it doesn't touch the beat-time under Beat or Sync Modes — only the envelope segments themselves.

Envelope Loop Mode (Loop) — Set to Loop and the envelope restarts once the decay segment finishes. Set to Beat or Sync and it restarts after a specified beat-time. Under Sync Mode that restart locks to song time. Under Trigger mode the envelope pays no attention to Note Off.

Envelope Beat/Sync Rate (Repeat) — So long as it remains on, the envelope re-fires after this span of beat-time. On each re-fire it climbs at the set attack rate from wherever it currently sits up to the peak level.

Envelope Loop Time (Time) — Should a note still be held after the decay/sustain segment ends, the envelope restarts from its initial value. This parameter sets how long the trip from sustain level back to the initial value takes.

As noted earlier, Sampler’s envelopes additionally offer parameters for tuning the slope of each envelope segment. A positive slope value makes the envelope race ahead at first and then ease off. A negative slope value keeps the envelope flat for a stretch before accelerating toward the finish. At a slope of zero the motion is linear, holding one constant rate across the whole segment.

This tab presents every time-based value in either samples or minutes:seconds:milliseconds, a choice you flip via the context menu on any of the parameter boxes. Here, "samples" denotes the tiniest measurable increment of digital audio rather than the audio files themselves, which are what we usually call “samples.“

_Sample Start_ — The time position at which playback kicks off. Should the volume envelope’s Attack parameter be cranked high (a slow attack), what you actually hear might commence somewhat after the point indicated here.

_Sample End_ — The time position at which playback stops (assuming no loop is enabled), regardless of whether the volume envelope has finished.

_Sustain Mode_ — The optional Sustain Loop marks out a portion of the sample that repeats for as long as the note sits in the sustain stage of its envelope. Switching on the Sustain Loop additionally makes the Release Loop available. That opens up a handful of playback choices:

_No Sustain Loop_ — Playback runs straight through until it hits the Sample End or until the volume envelope finishes its release stage, whichever comes first.

_Sustain Loop Enabled_ — Playback runs straight through to Loop End, then leaps at once to Loop Start and keeps looping. With Release Mode OFF, that looping persists within the Sustain Loop right up until the volume envelope finishes its release stage.

_Back-and-Forth Sustain Loop Enabled_ — Playback advances to Loop End, then runs backward to Loop Start, then heads forward toward Loop End once more. With Release Mode OFF, the cycle keeps repeating until the volume envelope finishes its release stage.

_Link_ — Flipping the Link switch makes Sample Start match Loop Start. Note that the Sample Start parameter box keeps its original value — it merely grays out, ready to be restored with one click.

_Loop Start_ — Where the Sustain Loop begins, expressed in samples.

_Loop End_ — Where the Sustain Loop ends, expressed in samples.

_Release Mode_ — Release Mode becomes available to enable any time the Sustain Loop is active.

— The volume envelope’s release stage runs, but stays confined to the Sustain Loop, and playback never moves past Loop End.

_Release Enabled_ — Once the volume envelope hits its release stage, playback runs straight ahead toward Sample End.

_Release Loop Enabled_ — Once the volume envelope hits its release stage, playback runs straight ahead to Sample End, then leaps at once to Release Loop and keeps looping until the volume envelope finishes its release stage.

_Back-and-Forth Release Loop Enabled_ — Once the volume envelope hits its release stage, playback runs straight ahead to Sample End, then reverses back to Release Loop, then heads forward toward Sample End again. The cycle repeats until the volume envelope finishes its release stage.

_Release Loop_ — fixes where the Release Loop begins. Sample End marks where the Release Loop ends.

_Sustain- and Release-Loop Crossfade (Crossfade)_ — Crossfading the loops helps strip clicks out of loop transitions. By default Sampler applies constant-power fades at loop boundaries, but switching off “Use Constant Power Fade for Loops“ in the context menu enables linear crossfades instead.

_Sustain- and Release-Loop Detune (Detune)_ — Because a loop is really just an oscillation, a sample's pitch can drift inside the loop in proportion to the loop’s length. Tip: very short loops make this most apparent. Detune lets you bring the pitch of those regions back in line with the rest of the sample.

_Interpolation (Interpol)_ — A global setting that controls how precisely transposed samples are rendered. Be warned that pushing the quality past “Normal“ to “Good” or “Best” taxes your CPU heavily.

_RAM Mode (RAM)_ — Another global control, this one pulls the full multisample into RAM. Doing so can improve performance while you modulate start and end points, yet loading sizable multisamples into RAM rapidly eats up the RAM your computer needs elsewhere. Either way, fitting your computer with as much RAM as you can is always advisable, since it can deliver meaningful performance benefits.

Right-clicking on the waveform to open its context menu offers several editing and viewing choices. Just as in the Sample Layer List context menu, Show in Browser, Manage Samples, Normalize Volumes and Normalize Pan all appear. You can also zoom in toward or out from the playing or looping regions, depending on the Sustain and Loop Modes currently in effect.

To close out, a few more controls sit at the far-right edge of the Sample tab:

_Vertical Zoom (slider)_ — Stretches the waveform's height within the sample display. This affects appearance only and leaves the audio untouched.

_B, M, L and R Buttons_ — Standing for Both, Mono, Left and Right, these buttons let you decide which channels of the sample get shown.
