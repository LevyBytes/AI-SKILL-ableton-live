# Live Instrument Reference (part 6)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

How many Operator voices (notes) may sound at once is governed by the Voices parameter, found in the global display. In an ideal world you would keep this value high enough that nothing ever gets cut while you perform, yet for the sake of CPU headroom a range from 6 to 12 tends to be more practical. Up to 32 voices of polyphony are available in Operator.

Tip: Certain timbres are inherently monophonic and ought to occupy just one voice — a flute being the classic illustration. For such patches, dial Voices down to 1. Choosing a value of 1 for Voices brings a second consequence as well: voices that overlap will sound legato, so the envelopes carry over from one note to the next without retriggering, and pitch alone shifts.

The shell's global section houses a master Volume control for the instrument, while the display within that global section holds a Pan control. Note pitch or a random amount can modulate Pan, by way of the neighbouring Pan < Key and Pan < Rnd controls, in turn.

A broad assortment of internal MIDI mappings is offered from the middle of the global display. Each of the MIDI controllers Velocity, Key, Aftertouch, Pitch Bend and Mod Wheel may drive two destinations, and the Amount sliders set a separate modulation depth for each. Keep in mind that Time < Key and pitch bend range come with fixed assignments, even though both of those sources can additionally feed a further target. To read more about the modulation choices on offer, consult the [complete parameter list](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#the-complete-parameter-list).

### 30.9.7 Glide and Spread

Operator’s Pitch Display and Shell Parameters.

A polyphonic glide capability is built into Operator. With it switched on, a fresh note begins at the pitch of whatever note preceded it and then glides smoothly toward its own intended pitch. The Glide Time control inside the pitch display switches Glide on or off and sets its behaviour.

There is also a distinctive Spread parameter in Operator, which manufactures a lush stereo chorus by allotting two voices to each note and steering one toward the left while the other goes to the right. Detuning separates these two voices, and the Spread control in the shell's pitch section governs how much detuning is applied.

Whether spread takes effect on any given note is decided by where the Spread parameter sits at the moment of the Note On event. For unusual results, you might, say, build a passage in which Spread stays at 0 for most of the time and is engaged only on certain notes. Those notes alone will sound in stereo, whereas the rest stay mono. Bear in mind that Spread draws heavily on the CPU.

A global Transpose knob is likewise housed in the pitch section.

### 30.9.8 Strategies for Saving CPU Power

To conserve CPU power, switch off whatever functions you have no use for, or trim the voice count. In particular, deactivating the filter or the LFO whenever they add nothing to the timbre will reclaim CPU power.

To economize on CPU resources, you'll typically also want to bring the voice count down to roughly 6 to 12, and apply the Spread feature sparingly. Switching off the Interpolation and Antialias modes within the global display likewise frees up CPU resources.

Keep in mind that silencing the oscillators does nothing to lower CPU power.

### 30.9.9 Finally…

Operator grew out of a deep fascination with FM synthesis paired with affection and devotion toward the vintage hardware FM synthesizers — among them the Yamaha SY77, the Yamaha TX81Z and the NED Synclavier II. The first musical investigations of FM synthesis came from composer and computer-music pioneer John Chowning during the mid-1960s. By 1973, he together with Stanford University struck up a partnership with Yamaha, which gave rise to the DX7, among the best-selling commercial musical instruments ever made.

Working from a synthesis idea that you can now investigate firsthand simply by experimenting with Operator in Live, John Chowning brought to life some truly astonishing and gorgeous musical works.

We wish you loads of fun with it!

### 30.9.10 The Complete Parameter List

What every Operator parameter does gets covered in the sections that follow. Bear in mind, too, that within Live itself you can read descriptions of controls (Operator's among them) straight from the application — just hover the mouse above a control and study the wording that shows up in the Info View. The list below organizes parameters into groups according to where they sit inside Operator.

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

#### 30.9.10.3 Pitch Shell and Display

Pitch Envelope On — Switches the pitch envelope on or off. Leaving it off while it goes unused reclaims a little CPU power.

Pitch Envelope Amount (Pitch Env) — Establishes the overall depth of the pitch envelope. At 100% the pitch shift matches exactly what the pitch envelope’s levels prescribe. At -100% the sign of those pitch envelope levels is flipped.

Spread — When Spread is raised, the synthesizer assigns two detuned voices to each note, one to the left and one to the right stereo channel, producing chorusing sounds. Spread places a heavy demand on the CPU.

Transpose — The instrument-wide transposition control. Adjusting it will change the pitch of notes that are already sounding.

Pitch Envelope Rates < Velocity (Time < Vel) — This control is present for the filter, pitch, LFO and volume envelopes alike. For that reason it is documented in the section covering [envelopes](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#envelope-display).

Glide (G) — With Glide active, a note glides from the previously played pitch to its own pitch. Keep in mind that none of the envelopes retrigger here when notes are sounded legato.

Glide Time (Time) — The duration of the slide from the previously played pitch to a note's final pitch once Glide is engaged. The control does nothing while Glide is disengaged.

Pitch Envelope to Osc (Destination A-D) — When this is switched on, the pitch envelope drives the frequency of the corresponding oscillator.

Pitch Envelope to LFO (Destination LFO) — When this is switched on, the pitch envelope drives the frequency of the LFO.

Pitch Envelope Amount A — Establishes how strongly the pitch envelope modulates the oscillators and LFO.

Pitch Envelope Destination B — Selects the pitch envelope's second modulation destination.

Pitch Envelope Amount B — Establishes how strongly the pitch envelope modulates the secondary target.

#### 30.9.10.4 Filter Shell and Display

Filter On — Switches the filter on or off. Leaving it off while unused reclaims CPU power.

Filter Type — A chooser offering low-pass, high-pass, band-pass, notch, and Morph filters.

Circuit Type — A chooser offering an assortment of circuit types that mimic the personality of vintage analog synthesizers.

Filter Frequency (Freq) — Sets the center or cutoff frequency of the filter. Bear in mind that note velocity and the filter envelope may further modulate the resulting frequency.

Filter Resonance (Res) — Sets the resonance surrounding the filter frequency for the low-pass and high-pass filters, and the bandwidth for the band-pass and notch filters.

Envelope / Filter Switches — These switches flip the display between the filter’s envelope and its frequency response.

Filter Frequency < Velocity (Freq < Vel) — This setting controls how strongly note velocity modulates the filter frequency.

Filter Frequency < Key (Freq < Key) — This setting controls how strongly note pitch modulates the filter frequency. At 100% the frequency doubles with every octave. C3 serves as the center point for this function.

Filter Envelope Rates < Velocity (Time < Vel) — This control is present for the filter, pitch, LFO and volume envelopes alike. For that reason it is documented in the section on envelopes.

Filter Frequency < Envelope (Envelope) — This setting controls how strongly the filter envelope modulates the filter frequency. At 100% the envelope is capable of shifting the frequency by roughly 9 octaves at most.

Filter Drive (Flt. Drive) — Adds extra input gain to the signal ahead of the filter.

Morph — Sets where the Morph filter sits within its morph cycle.

Shaper — A chooser that picks the curve used by the filter’s waveshaper.

Shaper Drive (Shp. Drive) — Raises or lowers the level of the signal feeding the waveshaper.

Dry/Wet — Sets the mix between the untouched signal and the one shaped by the waveshaper.

#### 30.9.10.5 LFO Shell and Display

LFO On — Switches the LFO (low-frequency oscillator) on or off. Leaving it off while unused reclaims a little CPU power.

LFO Waveform — Pick from a handful of common LFO waveforms. Sample and Hold (S&H) produces random steps, while Noise delivers band-pass filtered noise. Every waveform is band-limited so that stray clicks are avoided.

LFO Range — A vast frequency span is covered by the LFO. Pick Low for anything from 50 seconds up to 30 Hz, or Hi for 8 Hz through 12 kHz. With Sync, the LFO’s rate locks to your Set’s tempo. Because such high frequencies are possible, the LFO can double as a fifth oscillator.

Retrigger (R) — With this on, the LFO jumps back to the identical phase position whenever a note fires. With R off, the LFO keeps running freely.

LFO Rate (Rate) — Sets the rate of the LFO. Its true frequency also hinges on how the LFO Range and the LFO Rate < Key controls are set.

LFO Amount (Amount) — Sets the LFO's overall intensity. Keep in mind that the actual outcome also hinges on the LFO envelope.

LFO to Osc (Destination A-D) — When this is switched on, the LFO modulates the frequency of the corresponding oscillator.

LFO to Filter Cutoff Frequency (Destination FIL) — When this is switched on, the LFO modulates the cutoff frequency of the filter.

LFO Amount A — Sets how strongly the LFO modulates the oscillators and filter.

LFO Destination B — Selects the LFO's second modulation destination.

LFO Amount B — Sets how strongly the LFO modulates the secondary target.

LFO Envelope Rates < Velocity (Time < Vel) — This control is present for the filter, pitch, LFO and volume envelopes alike. For that reason it is documented in the section on envelopes.

LFO Rate < Key (Rate < Key) — Note pitch can govern the LFO’s frequency. Set to 100%, the LFO doubles its frequency every octave, behaving like an ordinary oscillator.

LFO Amount < Velocity (Amt < Vel) — This control tunes how much note velocity modulates the LFO intensity.

#### 30.9.10.6 Oscillators A-D Shell and Display

Osc On — Switches the oscillator on or off.

Osc Coarse Frequency (Coarse) — How oscillator frequency relates to note pitch is governed by the Coarse and Fine parameters. Coarse fixes that ratio in whole numbers, yielding a harmonic relationship.

Osc Fine Frequency (Fine) — How oscillator frequency relates to note pitch is governed by the Coarse and Fine parameters. Fine fixes that ratio in fractions of whole numbers, yielding an inharmonic relationship.

Osc Fixed Frequency On (Fixed) — Under Fixed Mode, oscillators ignore note pitch and hold a fixed frequency instead.

Osc Fixed Frequency (Freq) — The oscillator's frequency expressed in Hertz. It stays constant no matter the note pitch.

Osc Fixed Multiplier (Multi) — Serves to scale the range of the fixed frequency. Take this value times the oscillator’s Freq knob value to arrive at the true frequency in Hz.

Osc Output Level (Level) — Sets the oscillator's output level. When that oscillator modulates another, its level weighs heavily on the resulting timbre. Higher levels tend to yield bright and/or noisy sounds.

Envelope / Oscillator Switches — These switches flip the display between the oscillator’s envelope and its harmonics editor.

16/32/64 — These switches determine how many partials are open to user editing.

Osc Waveform (Wave) — Pick from an assortment of thoughtfully chosen waveforms. They can then be edited through the harmonics editor.

Osc Feedback (Feedback) — An oscillator is able to modulate itself provided no other oscillator is modulating it. That modulation hinges not only on the feedback control's setting but also on the oscillator level and the envelope. More feedback yields a more intricate resulting waveform.

Osc Phase (Phase) — Fixes the oscillator's starting phase. The available span covers one complete cycle.

Retrigger (R) — With this on, the oscillator jumps back to the identical phase position whenever a note fires. With R off, the oscillator keeps running freely.

Repeat — Repeating the drawn partials with a progressive fadeout can manufacture higher harmonics, governed by what's chosen in the Repeat chooser. Low Repeat settings yield a brighter tone, while higher ones bring more high-end roll-off and a stronger fundamental. With Repeat off, any partials beyond the 16th, 32nd or 64th harmonic get cut.

Osc Frequency < Velocity (Osc < Vel) — Note velocity can modulate an oscillator's frequency. Positive values push the oscillator’s pitch up as velocity grows, and negative values pull it down.

Osc Freq < Vel Quantized (Q) — Lets you quantize the result of the Frequency < Velocity parameter. When active, the audible outcome equals manually altering the Coarse parameter for every note.

Volume Envelope Rates < Velocity (Time < Vel) — This control is present for the filter, pitch, LFO and volume envelopes alike. For that reason it is documented in the section on envelopes.

Osc Output Level < Velocity (Vel) — Sets the degree to which note velocity governs the oscillator’s level. Applied to modulating oscillators, this produces velocity-dependent timbres.

Osc Output Level < Key (Key) — Sets the degree to which note pitch governs the oscillator’s level. C3 serves as the center point for this function.

#### 30.9.10.7 Envelope Display

Envelope Attack Time (Attack) — Sets how long a note takes to climb from the initial level up to the peak level. With the oscillator envelopes, this envelope segment is linear in shape. With the filter and pitch envelopes, the segment's shape is adjustable.

Envelope Decay Time (Decay) — Sets how long a note takes to fall from the peak level to the sustain level. With the oscillator envelopes, this envelope segment is exponential in shape. With the filter and pitch envelopes, the segment's shape is adjustable.

Envelope Release Time (Release) — How long a note takes to arrive at the end level once a Note Off message comes in. For the oscillator envelopes this level is fixed at -inf dB and the segment is exponential in shape. For the filter and pitch envelopes the End Level parameter sets the end level and the segment's shape is adjustable. Whatever segment happens to be running, this release segment commences from the envelope's value at the instant the Note Off message arrives.

Envelope Initial Level (Initial) — Sets the envelope's starting value.

Envelope Peak Level (Peak) — The high point reached when the note attack finishes.

Envelope Sustain Level (Sustain) — The level held once the note decay finishes. The envelope rests here until note release, except when it is in Loop, Sync or Beat Mode.

Envelope End Level (End) — (LFO, Filter and pitch envelopes only) The level arrived at when the Release stage ends.

Envelope Loop Mode (Loop) — Set to Loop, the envelope restarts once the decay segment ends. Set to Beat or Sync, it restarts after a specified beat-time. Under Sync Mode this restart is quantized to song time. Under Trigger mode the envelope disregards Note Off.

Envelope Beat/Sync Rate (Repeat) — As long as it remains on, the envelope is retriggered after this span of beat-time. On retriggering, the envelope climbs at the chosen attack rate from wherever it is up to the peak level.

Envelope Loop Time (Time) — Should a note linger past the close of the decay/sustain segment, the envelope restarts from its initial value. This parameter sets how long the journey from the sustain level back to the initial value takes.

Envelope Rates < Velocity (Time < Vel) — This setting determines how much note velocity modulates the envelope segments. It becomes particularly intriguing when the envelopes loop. Note that this modulation leaves the beat-time in Beat or Sync Modes untouched, acting instead on the envelope segments themselves.

The filter and pitch envelopes additionally supply controls for tilting the slope of their envelope segments. With positive slope values the envelope dashes ahead at the start and eases off afterward. With negative slope values the envelope holds flat for a stretch and then accelerates toward the close. At a slope of zero the response is linear, the envelope advancing at a steady rate across the whole segment.

Attack Slope (A.Slope) — Shapes the Attack envelope segment.

Decay Slope (D.Slope) — Shapes the Decay envelope segment.

Release Slope (R.Slope) — Shapes the Release envelope segment.

#### 30.9.10.8 Context Menu Options for Operator

A few of Operator's operations and parameters can be reached solely through the context menu. They comprise:

Copy commands for Oscillators — Within the context menu of the oscillator’s shell and envelope display you'll find options for copying parameters from one oscillator to another.

Envelope commands — Within the context menu of every envelope display you'll find options that swiftly drive all envelope levels to their maximum, minimum, or middle values.

Harmonics editor commands — The harmonics editor's context menu can confine partial drawing to even or odd harmonics and switch normalization of an oscillator’s output level on or off. A command for exporting the waveform as an .ams file is present as well.

Play By Key — Found in the context menu of the filter’s Freq control, this command tunes the filter for key tracking by placing the cutoff at 466 Hz and the Freq < Key at 100%.

Enable Per-Note Pitch Bend — This is switched on by default, letting Operator react to per-note pitch bend changes. Should you wish, you can turn the behaviour off by clearing the option in the context menu of the device title bar.

### 30.10 Sampler

The Sampler Instrument.

Sampler is a streamlined yet powerful multisampling instrument that makes the most of Live‘s nimble audio engine. From the outset it was built to cope effortlessly with multi-gigabyte instrument libraries, and it brings in the majority of common library formats. Yet with Sampler, playback merely opens the door; the wide-reaching internal modulation system, touching almost every facet of its sound, turns it into a logical outgrowth of Live‘s sound-shaping methods.

### 30.10.1 Getting Started with Sampler

Beginning with Sampler is as simple as picking a preset from the browser. As with every one of Live‘s devices, the presets for Sampler sit in folders shown beneath its name. Presets brought in from third-party sample libraries appear here as well, inside the _Imports_ folder.

After loading a Sampler preset onto a track, don't forget to arm that track for recording (which additionally lets you hear whatever MIDI notes you may wish to play), and then begin playing!

### 30.10.2 Multisampling

First, let's bring in the idea of _multisampling_. The purpose of this technique is to faithfully reproduce the intricacy of instruments whose timbre shifts dynamically. Instead of leaning on plain transposition of one recorded sample, multisampling records an instrument at several spots throughout its important sonic span. Generally this means recording the instrument across various pitches together with various degrees of emphasis (played softly, moderately, loudly, etc.). What results — the _multisample_ — gathers together every one of those separately recorded sample files.

Take the acoustic piano as a common example of a multisampled instrument. Given that the piano's range of pitch and dynamics is so broad and rich in timbre, stretching a single sample over many octaves would fail to capture the instrument's subtleties. Because multisampling draws on distinct sound sources, you might record three or more samples for each piano key (soft, medium, loud, very loud, and the like), squeezing the greatest expressive range out of the sampler.
