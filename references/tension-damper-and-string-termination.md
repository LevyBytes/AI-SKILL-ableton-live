# Tension Damper And String Termination

Open when you need guidance on Tension Damper And String Termination in Ableton Live.

Context: [String Tab](simpler-and-tension-routes.md#30122-string-tab).

<a id="source-301224-the-damper-section"></a>
#### 30.12.2.4 The Damper Section

Tension’s Damper Section.

Every string instrument has some kind of damping device that silences the ringing string. On pianos it's a felt pad pressed to the string the moment the key comes up. With instruments like guitars and violins, the performer damps by halting the string's motion using their fingers. Beyond controlling string decay, dampers contribute a sound of their own, which forms an important part of a string instrument's tone. A switch beside its name turns the Damper section on or off.

Even though a damper exists to silence the string rather than excite it, it bears some resemblance to a hammer and carries a few of the same parameters.

How firmly the damper's surface bears down on the string is governed by the Mass knob. Raising the value mutes the string sooner.

You set how stiff the damper material is with the Stiffness control. Lower settings emulate pliable substances like felt, while higher settings imitate a metal damper.

Be aware that very large Mass and Stiffness settings can mimic dampers that grip the string firmly enough to alter its working length, which then shifts the tuning.

The Velocity control governs how quickly the damper lands on the string as the key is released, and likewise how quickly it leaves the string as the key is pressed. Use caution here — very large Velocity settings can make the damper strike the string so forcefully that a loud burst results when the key lifts. Bear in mind the Gated switch's position dictates whether the Velocity control does anything. With the Gated switch on, the damper meets the string upon key release. With Gated off, the damper stays on the string permanently, so the Velocity control has no bearing.

The Position knob does much the same job as its counterpart in the Exciter section, but here it sets where along the string the damper touches. At 0% the damper meets the string at its termination point, and at 50% it damps the string's midpoint. Things differ slightly once the Fix. Pos switch is engaged, though. Then the contact point stays anchored to one location instead of moving as the string's length changes.

Using the Key sliders beneath them, the Mass, Stiffness and Velocity, and Position parameters can be additionally modulated by note pitch.

How rigid the damper mechanism is gets set with the Damping knob, which determines the total vibration the damper soaks up. Lower settings mean less damping (and longer decays). This grows somewhat unpredictable, though, once the Damping value passes 50%. At elevated settings the mechanism turns so rigid that it rebounds off the string. That in turn shortens the total time the damper stays in contact, which lengthens the decay. To really feel out this parameter, slowly raise the knob while striking one key over and over.

The String Section

Tension’s String Section.

A stringed instrument's sound rests chiefly on the string's vibration. That string's working length also sets the pitch we end up hearing.

How long the ringing string takes to fade into silence is set by the Decay slider, with larger values lengthening the decay. Sitting next to Decay, the < Key slider lets note pitch modulate the decay time.

The Ratio slider establishes the proportion between the decay times of the string's oscillation at the note's onset versus its release. At 0% the Decay slider's value governs the decay for both the onset and the release. Pushing the Ratio up shortens the release while leaving the onset decay unchanged.

In theory a ringing string is harmonic, so its partials line up as whole-number multiples of the fundamental frequency. Actual strings, by contrast, are all inharmonic to some degree, an effect that grows with string thickness. The Inharm slider captures this, pushing upper partials progressively out of tune as you raise its value.

How much high-frequency energy resides in the string's vibration is set by the Damping slider. Larger values keep more upper partials present (meaning less damping). The < Key slider on its right lets note pitch modulate this parameter.

The Vibrato Section

Tension’s Vibrato Section.

To modulate the string's pitch, the Vibrato section employs an LFO. Like all of Tension's parameters, these controls can heighten the realism of a stringed-instrument model — or conjure sounds nobody has heard before.

A switch beside its name turns the Vibrato section on or off.

The Delay slider sets the lag before vibrato kicks in after the note starts, whereas Attack sets how long vibrato needs to climb to full strength (the level the Amount knob defines).

This section's two key parameters are the Rate and Amount sliders. Rate sets how fast the pitch wavers, and Amount sets how strong (the amplitude of) the effect is.

How much the modulation wheel influences vibrato strength is set by the < Mod slider. This control operates relative to whatever the Amount knob is set to.

The Error slider injects randomness into the vibrato by adding random drift to the Rate, Amount, Delay and Attack parameters.

<a id="source-301225-the-termination-section"></a>
#### 30.12.2.5 The Termination Section

Tension’s Termination Section.

What the Termination section models is the interplay among fret, finger and string. On a real instrument that interplay alters the string's working length, which then dictates the pitch of the note you hear.

A switch beside its name turns the Termination section on or off.

Via the Vel and Key sliders, the Finger Mass parameter can also be modulated by velocity or by note pitch.

<a id="source-live-instrument-reference-part-10"></a>

Use the Finger Mass and Finger Stiff knobs to dial in the finger’s physical traits: the former governs how forcefully the finger presses against the string, while the latter controls how rigid the finger is. A separate Fret Stiff parameter handles the simulated rigidity of the fret.
