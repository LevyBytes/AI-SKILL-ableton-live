# Collision Resonator Tuning And Mixer

Open when you need guidance on Collision Resonator Tuning And Mixer in Ableton Live.

Context: [Resonator Tabs](collision-and-drift-routes.md#3024-resonator-tabs).

<a id="source-30241-tuning-section"></a>
#### 30.2.4.1 Tuning Section

Resonator Tuning Parameters.

Coarse and fine tuning are handled respectively by the Tune knob and Fine slider. Tune steps in semitones either direction, while Fine works in one-cent steps (reaching at most a quarter tone, or 50 cents, in either direction).

The Key slider on the MIDI tab can also drive the Tune knob. That Key slider governs how strongly shifts in MIDI note pitch retune the resonator. Its 100% default keeps the resonator on a standard equal-tempered scale. Raise it to 200% and each keyboard semitone produces a whole-step tuning shift. Push it negative and the resonator falls in pitch as you ascend the keyboard.

A ramp that sweeps the resonator’s pitch across time is supplied by the Pitch Envelope parameters (Pitch Env and Time). Pitch Env fixes the initial pitch and Time controls how long the glide to the destination pitch lasts. Velocity, by way of the matching Vel slider on the MIDI tab, can drive that initial pitch.

<a id="source-30242-mixer-section"></a>
#### 30.2.4.2 Mixer Section

Resonator Mixer.

A dedicated Gain and Pan control belongs to each resonator. Note pitch, through the Key slider on the MIDI tab, can also drive Pan.

A share of the unprocessed oscillator signal is blended in alongside the resonated signal by the Bleed control. Turn it up and more of that raw signal comes through. It comes in handy for bringing back high frequencies, which low tuning or quality settings tend to dampen.

Output level for the chosen resonator is set by Gain.
