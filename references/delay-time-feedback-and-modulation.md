# Delay Time Feedback And Modulation

Open when you need guidance on Delay Time Feedback And Modulation in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2811-delay"></a>
### 28.11 Delay

The Delay Effect.

Each stereo channel in Delay gets its own separate delay line, and the device adds a band-pass filter plus LFO modulation features.

You may dial the delay time in tempo-locked beat divisions (Sync) or in milliseconds (Time). The Delay Time Mode toggles let you flip between the two.

Under Sync, the numbered buttons let you set the delay time in sixteenth notes. Pick 4, for instance, and the input is held back by four sixteenth notes, which works out to one beat — a quarter note — of delay. The Offset sliders nudge the sixteenth-note timing by fractional steps. Negative settings tighten the timing so the delay lands a little ahead of the sixteenth-note division, while positive settings loosen it so the delay arrives a touch later. Offset is a good way to fold gentle swing into the delay.

Under Time, you can hold the input back by anything from 1.00 millisecond out to 5.00 seconds.

Switch on the Stereo Link toggle to tie the delay settings of the left and right channels together. With the link active, any change you make to one channel’s delay time carries over to both. Offset still adjusts per channel on its own, even while Stereo Link is on.

How much of each channel’s output gets routed back into that channel’s delay line input is set by the Feedback control. These feedback loops stay separate per channel, so the left channel’s signal never crosses into the right channel and the reverse holds true as well.

Hit the Freeze button and the audio sitting in the device’s buffer at that instant loops forever. Fresh input gets disregarded until you switch Freeze back off.

Ahead of the delay signal sits a band-pass filter you can turn on or off with the Filter toggle. Within the display, drag along the X-axis to move the filter’s center frequency and drag along the Y-axis to set its bandwidth. The Freq and Width sliders adjust these same values too.

An LFO can modulate the delay time and the filter frequency, opening up everything from chorus-style textures to chopped-up glitches.

Out of the box, the full LFO section stays folded away and only the delay-time and filter modulation controls appear under the band-pass display. The LFO Controls toggle unfolds the LFO section to reveal the extra modulation options.

Expanding the LFO Section via the LFO Controls Toggle.Delay’s LFO Modulation Options.

How much LFO modulation reaches the delay time is set by the Delay slider, while the modulation depth for the filter frequency is set by the Filter slider.

The Rate drop-down menu offers these LFO rate modes: Rate, Time, Synced, Triplet, Dotted, and Sixteenth. As playback runs, the LED beside the LFO Controls toggle blinks in step with the active LFO rate.

The Wave drop-down holds these LFO waveform choices: Sine, Triangle, Ramp Up, and Ramp Down, plus Square, S&H (Sample and Hold), or Wander. The Morph slider lets you reshape whichever waveform you chose.

Changing the delay time while Delay is working on audio — during playback, say — can throw sudden shifts into the delayed sound. To control how Delay manages those timing transitions, you can pick among three smoothing modes:

- _Repitch_ shifts the pitch when you alter the delay time, much like vintage tape delay units behave. It is the default mode.
- _Fade_ crossfades from the old delay time to the new one. The effect can resemble granular synthesis, particularly when you move the delay time slowly.
- _Jump_ snaps straight to the new delay time. That can throw audible clicks if you change the delay time while an earlier delay is still ringing out.

Which smoothing mode you select also changes how the LFO modulation of delay time and filter colors the end result. Try tweaking the modulation under each mode to hear the delay’s sound shift.

Switch on the Ping Pong toggle and the delayed signal bounces back and forth across the left and right channels.

The Dry/Wet control sets how the dry and processed signals balance out. If you run Delay on a return track, push this control to 100% so the return track passes along only the processed signal.
