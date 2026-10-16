# Operator Global Parameters And Modulation Targets

Open when you need guidance on Operator Global Parameters And Modulation Targets in Ableton Live.

Context: [The Complete Parameter List](operator-and-sampler-routes.md#30910-the-complete-parameter-list).

<a id="source-309101-global-shell-and-display"></a>
#### 30.9.10.1 Global Shell and Display

Time — A single master control governing the rate of every envelope.

Tone — High-frequency timbres are well within Operator's reach, and these can occasionally bring on aliasing artifacts. How much high-frequency material a sound carries is set by the Tone control. Higher values tend to sound brighter while also raising the chance of aliasing.

Volume — Establishes the instrument's overall output level.

Algorithm — One oscillator may act as a modulator of others, be modulated by others, or do both at once. By determining how the oscillators link together, the algorithm exerts a major influence on the resulting timbre.

Voices — Fixes the upper limit on how many notes may sound at the same time. Should the request exceed the available voices, the notes played earliest are dropped.

Retrigger (R) — With this on, notes that are already enabled are retriggered instead of spawning an extra voice.

Interpolation — Engages or bypasses the interpolation algorithm used by the oscillators and the LFO. When off, certain timbres take on a rougher character, the noise waveform especially. Switching it off also reclaims a little CPU power.

Antialias — Engages or bypasses Operator's high-quality antialias mode, which works to hold down high-frequency distortion. Switching this mode off lightens the CPU load.

Time < Key — Note pitch can steer the rate of all envelopes. Raising the value of the global Time < Key parameter makes the envelopes progress more quickly as higher notes are sounded.

Pitch Bend Range (PB Range) — Sets how strongly MIDI pitch bend messages take effect.

Pan — Adjusts the stereo placement of every note. It comes in especially handy when driven by clip envelopes.

Pan < Key (Key) — Turning Pan < Key up sends low notes increasingly toward the left channel and high notes toward the right. This is the usual choice for piano-style sounds.

Pan < Random (Rnd) — Governs how widely notes scatter at random across the left and right channels.

<a id="source-309102-modulation-targets"></a>
#### 30.9.10.2 Modulation Targets

The modulation targets below show up as MIDI routing destinations within the global display, and serve as modulation targets for the LFO and pitch envelope too.

Off — Switches off this controller’s modulation routing.

OSC Volume A-D — Modulates the volume of the selected oscillator.

OSC Crossfade A/C — Uses the modulation source's value to crossfade between the volumes of the A and C oscillators.

OSC Crossfade B/D — Uses the modulation source's value to crossfade between the volumes of the B and D oscillators.

OSC Feedback — Modulates how much feedback every oscillator gets. Remember that feedback reaches only those oscillators that aren't being modulated by another oscillator.

OSC Fixed Frequency — Modulates the pitch of every oscillator currently set to Fixed Frequency mode.

FM Drive — Modulates the level of all oscillators that are modulating other oscillators, which alters the timbre.

Filter Frequency — Modulates the cutoff frequency of the filter.

Filter Q (Legacy) — Modulates filter resonance when the legacy filter types are in use.

Filter Res — Modulates filter resonance when the newer filter types are in use.

Filter Morph — Modulates where you are within the filter’s morph cycle (this matters only for the Morph filter type.)

Filter Drive — Modulates how much Drive is applied (unavailable while the Morph filter is chosen.)

Filter Envelope Amount — Modulates the filter’s envelope intensity.

Shaper Drive — Modulates how much gain feeds the filter’s waveshaper.

LFO Rate — Modulates the rate of the LFO.

LFO Amount — Modulates the intensity of the LFO.

Pitch Envelope Amount — Modulates the intensity of the pitch envelope.

Volume — Modulates Operator’s global output volume.

Panorama — Modulates where Operator’s output sits in the stereo field.

Tone — Modulates the global Tone parameter.

Time — Modulates the master control over every envelope rate.
