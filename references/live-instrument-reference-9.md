# Live Instrument Reference (part 9)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

The filter portion of Simpler provides several filter shapes — low-pass, high-pass, band-pass, notch, plus a distinctive Morph filter. Any filter may toggle between 12 and 24 dB slopes, and you can also pick from a range of analog-modeled circuit behaviors, built together with Cytomic, that reproduce the hardware filters of certain vintage analog synthesizers.

The Clean circuit choice is a precise, low-CPU implementation identical to the filters found in [EQ Eight](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#eq-eight). It can be used with every filter shape.

The OSR circuit choice is a state-variable design whose resonance is capped by a distinctive hard-clipping diode. Its model comes from a fairly uncommon British monosynth, and you can apply it to any filter shape.

The MS2 circuit choice relies on a Sallen-Key topology together with soft clipping to bound resonance. Drawn from a celebrated semi-modular Japanese monosynth, it works with the low-pass and high-pass filters only.

The SMP circuit is an original design that doesn't trace back to any specific piece of gear. Combining traits of the MS2 and the PRD circuits, it can be selected for the low-pass and high-pass filters.

The PRD circuit follows a ladder topology and applies no deliberate resonance ceiling. Modeled after a classic dual-oscillator American monosynth, it is offered for the low-pass and high-pass filters.

The chief filter controls are the standard synth knobs Frequency and Resonance. Frequency sets the point in the harmonic spectrum where filtering takes effect, and Resonance emphasizes the frequencies around that spot.

If you select the low-pass, high-pass, or band-pass filter together with any circuit other than Clean, an extra Drive control appears for adding gain or distortion to the audio ahead of the filter stage.

For the Morph filter, an extra Morph control continuously sweeps the shape from low-pass through band-pass and high-pass to notch, then loops back around to low-pass.

Right-clicking the Morph knob exposes context-menu entries; each one instantly snaps the Morph control onto a single shape — namely low-pass, band-pass, high-pass, or notch.

Within the filter section's display, the Frequency and Envelope buttons switch the view between the filter's frequency response and its envelope. You set cutoff frequency and resonance either with the knobs or by dragging the response curve directly in that display. Several sources can additionally modulate filter frequency:

- Note velocity, through the Vel control located in the filter's display.
- Note pitch, through the Key control located in the filter's display.
- Filter envelope, through the Envelope control located in the filter's display.
- LFO, through the Filter slider found in the LFO section.

### 30.11.4 Envelopes

Simpler’s Filter and Amplitude Envelope Controls.

Like most synthesizers, Simpler provides three traditional ADSR envelopes for sculpting how the sample evolves over time. You can edit modulation of amplitude, filter frequency, and pitch by switching on their respective buttons in the envelope section. Attack sets, in milliseconds, how long the envelope needs to climb to its maximum once a note triggers. Decay governs how long the envelope takes to fall to the Sustain level, where it stays put until the note ends. Release determines, once the note finishes, how long the envelope needs to fall from the Sustain level all the way to zero. You can tweak these values with their dedicated controls or graphically by dragging the handles inside the envelope displays.

How strongly the envelopes act on filter cutoff and on pitch is set through the envelope amount controls located at the upper right of each of those sections.

The Filter and Pitch Envelope Amount Controls.

You can loop the Amplitude Envelope using the Loop Mode chooser. Under Loop and Trigger modes, should a note remain held once the Decay stage finishes, the envelope returns to its starting value. How quickly it travels from the Sustain level back to that starting value is governed by the Time parameter. Under Beat and Sync modes, if a note is still held past the duration set by the Rate slider, the envelope likewise returns to its starting value.

The Amplitude Envelope Loop Mode Chooser and Time Control.

### 30.11.5 LFO

Simpler’s LFO Section.

Waveform options in the LFO (low-frequency oscillator) section include sine, square, triangle, sawtooth down, sawtooth up and random. You can let the LFO oscillate freely anywhere from 0.01 to 30 Hz, or lock it to subdivisions of the Set's tempo. In Simpler, an LFO operates separately for every _voice_, that is, each note being sounded.

How long the LFO takes to climb to full strength is set by the Attack control. Retrigger is toggled by the R switch. With it active, the LFO's phase snaps back to the Offset value at the onset of each note. Keep in mind that Offset does nothing while Retrigger is switched off.

Each LFO's Rate is scaled relative to the pitch of arriving notes by the Key parameter. With a high Key value, higher notes receive a faster LFO rate. When Key sits at zero, every voice's LFO shares one rate and might vary only in phase.

How far the LFO modulates volume, pitch, pan, and filter is governed by the Volume, Pitch, Pan, and Filter sliders, in that order.

### 30.11.6 Global Parameters

Simpler’s Global Parameters.

The stereo placement is set with the Pan control, though it can be nudged additionally by randomness (using the Random > Pan slider) or driven by the LFO.

Simpler additionally provides a dedicated Spread parameter that produces a lush stereo chorus by sounding two voices for each note, with one panned left and the other right. Those two voices are detuned from one another, and the degree of detuning is dialed in with the Spread control.

Whether a given note receives spread is decided by where the Spread parameter sits at the moment of the Note On event. For unusual results you might, for example, build a pattern in which Spread stays at zero most of the way and is engaged only for a handful of notes. Those notes then sound in stereo while the rest remain mono.

Simpler's overall output level is set by the Volume control, which may additionally respond to note velocity according to the Velocity > Volume control. You can produce tremolo by letting the LFO drive the Volume parameter.

When the arriving MIDI note is C3, Simpler reproduces a sample at its native pitch, but the Transpose control lets you shift it by +/- 48 semitones. The LFO or the pitch envelope can also modulate pitch. That pitch envelope is particularly useful for crafting percussive tones. Simpler responds to MIDI Pitch Bend data with a range of +/- 5 semitones. The Transpose parameter can additionally be driven by clip envelopes and outboard controllers. To fine-tune pitch, turn to the Detune control, adjustable across +/- 50 cents.

A glide capability is built into Simpler. With it switched on, a fresh note begins at the pitch of whatever note preceded it, then glides smoothly to its target pitch. There are two glide modes: Glide operates monophonically, and Portamento operates polyphonically. The glide's speed is dialed in with the Time control.

### 30.11.7 Context Menu Options for Simpler

Certain Simpler functions become available only when you open the context menu from either the sample display or Simpler's title bar.

Out of the box, Simpler applies constant-power fades. To switch instead to linear crossfades, open the context menu on Simpler's title bar and uncheck the entry labeled “Use Constant Power Fade for Loops“. Bear in mind the Fade parameter disappears whenever warp is switched on.

Presets built in Simpler may be translated for use in [Sampler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sampler), and the reverse works too. Accomplish this by right-clicking Simpler's title bar and selecting the Simpler -> Sampler command. Doing so lets a Simpler preset sit inside a multisample setup within Sampler. Be aware, though, that Sampler lacks Simpler's warping and slicing features, so any preset relying on those will sound and act quite differently once it reaches Sampler.

Choosing Manage Sample displays the loaded sample inside Live's [File Manager](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#managing-files-in-a-project), whereas Show in Browser surfaces it in Live's browser. Show in Finder/Explorer opens the sample inside its containing folder in your computer's OS. Keep in mind this entry is absent for samples that originated from official Ableton Packs.

The Normalize Volumes command raises the loaded sample's level so its loudest peak fills the entire available headroom.

The Crop command discards whatever sits beyond the Start and End markers, while Reverse plays the whole sample in reverse. Both Crop and Reverse leave your data intact: they duplicate the sample and operate on the copy, so the source remains untouched.

While in Slicing Playback Mode, two extra context-menu entries appear. Slice to Drum Rack swaps the Simpler for a Drum Rack where every existing slice lands on its own pad. Slice to New MIDI Track behaves much the same, except it adds a separate track holding a Drum Rack instead of swapping out the current Simpler. On top of that, slicing to a new track produces a clip that triggers the slices in sequence. For deeper coverage of slicing, consult the [dedicated section](https://www.ableton.com/en/live-manual/12/converting-audio-to-midi/#slice-to-new-midi-track) on the subject.

### 30.11.8 Strategies for Saving CPU Power

Synthesis on the fly demands considerable processing. There are, however, ways to lighten the CPU burden. Trim the CPU that Simpler consumes by applying some of these measures:

- During warping, keep in mind that the Complex and Complex Pro modes draw far more CPU than the remaining Warp Modes.
- Switch off the Filter whenever you don't need it.
- The CPU demand of a filter rises with how steep its slope is — the 24 dB slope costs more than the 12 dB slope.
- Disabling the LFO gives CPU a modest break.
- Because they double the workload, stereo samples consume far more CPU than mono ones.
- Lower how many voices may sound at once using the Voices control.
- Set Spread to 0% whenever it isn't required.

### 30.12 Tension

The Tension Instrument.

Tension is a synth devoted to recreating string instruments, designed together with Applied Acoustics Systems. It rests entirely on physical-modeling techniques, employing neither samples nor wavetables. Rather, it generates audio by computing the mathematical equations that describe a string instrument's various parts and the ways they interact. This sophisticated engine reacts in real time to the playing gestures it receives, so it captures the depth and expressiveness of genuine string instruments.

Tension provides four exciter varieties (a pair of hammer types, plus a pick and a bow), a faithful string model, a model of how fret and finger meet, a damper model, and several soundboard varieties. Blending these components together makes it possible to recreate a broad assortment of string instruments. Tension additionally carries filters, LFOs, envelope parameters, and MPE support, all of which push its sound-shaping reach past what any “real-world“ instrument could do. Lastly, Tension supplies a large set of performance tools, among them keyboard modes, portamento, vibrato, and legato functions.

### 30.12.1 Architecture and Interface

An instrument's principal sound-generating mechanism is the vibration of its _string_. That string is set vibrating by an _exciter_, which may be a hammer, a pick or a bow. How fast it oscillates depends on the string's working length, governed in turn by the finger/fret contact, or _termination_. Applying a _damper_ to the strings shortens how long the oscillation takes to fade. On a piano, for instance, this happens when felt presses against the strings as you let go of the keys and sustain pedal. From there the string's vibration passes to the instrument's _body_, which can project sound effectively. Some instruments route the string's vibration straight to the body by way of the bridge. Others, like the electric guitar, rely on a _pickup_ to carry the string vibration to an amplifier. Beyond these core stages, a _filter_ section sits between the string and body stages to broaden the instrument's tonal range.

Tension's interface splits into two primary tabs, each broken down further into sections. Every core sound-generating element bound up with the string itself sits on the _String_ tab, namely these: _Exciter, Damper, String, Vibrato, Termination, Pickup,_ and _Body_. Over on the _Filter/Global_ tab you'll find the Filter section, the MPE section, and the controls for global performance parameters. Every section — apart from String and the global Keyboard section — can be switched on or off on its own. Disabling a section cuts CPU usage.

### 30.12.2 String Tab

Within the String tab live the parameters governing the string's physical characteristics along with how it gets played.

#### 30.12.2.1 The Exciter Section

Tension’s Exciter Section.

#### 30.12.2.2 Exciter Types

You can sound the modeled string with a range of exciters so as to mimic various instrument types and playing styles.

A switch beside its name turns the Exciter section on or off. While it's off, only contact with its damper can excite the string. Should you deactivate both the Exciter and Damper sections, there's nothing left to start the string vibrating — so if no sound emerges, confirm that at least one of these sections is active.

Four options appear in the Exciter Type chooser - _Bow, Hammer, Hammer (bouncing)_ and _Plectrum_.

_Bow_ — tied to bowed instruments like the violin, viola or cello, this exciter drives the string into continuous oscillation. As the bow hair travels over the string, friction makes the string repeatedly cling to the hair and then release. How frequently that stick-and-slip cycle repeats sets the fundamental pitch. Keep in mind the Damping knob is disabled while the Bow exciter is chosen.

_Hammer_ — this exciter recreates the action of soft hammers or mallets. Hammer simulates a hammer sitting beneath the string that strikes it a single time, then drops away. A piano is one place this kind of mechanism turns up.

_Hammer (bouncing)_ - this exciter resembles _Hammer_, but it instead simulates a hammer positioned over the string and let fall onto it, so it may rebound off the string several times. A hammered dulcimer is one instrument where this playing style appears.

_Plectrum_ — a plectrum, or “pick“, goes with instruments like guitars and harpsichords. Picture it as a slanted object tucked beneath the string that flicks the string into motion.

#### 30.12.2.3 Exciter Parameters

Five parameter knobs sit alongside the Exciter Type chooser. Which Exciter Type you pick determines the first two parameters, while the remaining three stay the same across all types.

_Bow Parameters:_

- The Force knob sets how much pressure the bow exerts on the string. Raising this value gives the tone a more “scratchy“ character.
- The Friction knob sets the degree of friction between the bow and the string. Larger values typically yield a quicker attack.

_Hammer / Hammer (bouncing) Parameters:_

- The Mass knob sets the hammer's mass.
- The Stiffness knob sets how rigid the hammer's striking surface is.

_Plectrum Parameters:_

- The Protrusion knob sets how far the plectrum's surface reaches under the string. Smaller values give a “thinner,“ slighter tone, since less mass drives the string into motion.
- The Stiffness knob sets how rigid the plectrum is.

_Universal Exciter Parameters:_

- The Velocity knob sets how fast the exciter drives the string.
- The Position knob defines where along the string the exciter touches it. At 0% the exciter meets the string at its termination point, and at 50% it strikes the string's midpoint. Once the Fix. Pos switch (covered further below) is on, however, position no longer scales with the string's length.
- The Damping knob sets how much of the exciter's striking energy gets reabsorbed into the exciter. Note: With the _Hammer (bouncing)_ exciter this roughly parallels the Stiffness parameter, except that rather than the rigidity of the hammer's surface it governs the rigidity of the virtual “spring“ linking the hammer to the mass driving it. Raising the Damping value shortens the contact between hammer and string, which usually yields a louder, brighter result.

When you engage the Fix. Pos switch, the contact point stays locked to one spot instead of shifting as the string's length changes. That mirrors a guitar, where the picking spot stays roughly constant no matter which notes you play. With a piano the exciter position is proportional — the hammers typically hit the string near 1/7th of its length — so it's best captured with Fix. Pos switched off.

Lastly, the Vel and Key sliders let you modulate these behaviors according to note velocity and pitch respectively.

Do keep in mind that the parameters in the Exciter section interact tightly to shape how the instrument behaves overall. Some setting combinations can leave you with no sound whatsoever.

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

#### 30.12.2.5 The Termination Section

Tension’s Termination Section.

What the Termination section models is the interplay among fret, finger and string. On a real instrument that interplay alters the string's working length, which then dictates the pitch of the note you hear.

A switch beside its name turns the Termination section on or off.

Via the Vel and Key sliders, the Finger Mass parameter can also be modulated by velocity or by note pitch.
