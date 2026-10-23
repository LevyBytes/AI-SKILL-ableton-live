# Operator Pitch Filter And LFO Reference

Open when you need guidance on Operator Pitch Filter And LFO Reference in Ableton Live.

Context: [The Complete Parameter List](operator-and-sampler-routes.md#30910-the-complete-parameter-list).

<a id="source-309103-pitch-shell-and-display"></a>
#### 30.9.10.3 Pitch Shell and Display

Pitch Envelope On: Switches the pitch envelope on or off. Leaving it off while it goes unused reclaims a little CPU power.

Pitch Envelope Amount (Pitch Env): Establishes the overall depth of the pitch envelope. At 100% the pitch shift matches exactly what the pitch envelope’s levels prescribe. At -100% the sign of those pitch envelope levels is flipped.

Spread: When Spread is raised, the synthesizer assigns two detuned voices to each note, one to the left and one to the right stereo channel, producing chorusing sounds. Spread places a heavy demand on the CPU.

Transpose: The instrument-wide transposition control. Adjusting it will change the pitch of notes that are already sounding.

Pitch Envelope Rates < Velocity (Time < Vel) — This control is present for the filter, pitch, LFO and volume envelopes alike. For that reason it is documented in the section covering [envelopes](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#envelope-display).

Glide (G): With Glide active, a note glides from the previously played pitch to its own pitch. Keep in mind that none of the envelopes retrigger here when notes are sounded legato.

Glide Time (Time): The duration of the slide from the previously played pitch to a note's final pitch once Glide is engaged. The control does nothing while Glide is disengaged.

Pitch Envelope to Osc (Destination A-D): When this is switched on, the pitch envelope drives the frequency of the corresponding oscillator.

Pitch Envelope to LFO (Destination LFO): When this is switched on, the pitch envelope drives the frequency of the LFO.

Pitch Envelope Amount A: Establishes how strongly the pitch envelope modulates the oscillators and LFO.

Pitch Envelope Destination B: Selects the pitch envelope's second modulation destination.

Pitch Envelope Amount B: Establishes how strongly the pitch envelope modulates the secondary target.

<a id="source-309104-filter-shell-and-display"></a>
#### 30.9.10.4 Filter Shell and Display

Filter On: Switches the filter on or off. Leaving it off while unused reclaims CPU power.

Filter Type: A chooser offering low-pass, high-pass, band-pass, notch, and Morph filters.

Circuit Type: A chooser offering an assortment of circuit types that mimic the personality of vintage analog synthesizers.

Filter Frequency (Freq): Sets the center or cutoff frequency of the filter. Bear in mind that note velocity and the filter envelope may further modulate the resulting frequency.

Filter Resonance (Res): Sets the resonance surrounding the filter frequency for the low-pass and high-pass filters, and the bandwidth for the band-pass and notch filters.

Envelope / Filter Switches: These switches flip the display between the filter’s envelope and its frequency response.

Filter Frequency < Velocity (Freq < Vel) — This setting controls how strongly note velocity modulates the filter frequency.

Filter Frequency < Key (Freq < Key) — This setting controls how strongly note pitch modulates the filter frequency. At 100% the frequency doubles with every octave. C3 serves as the center point for this function.

Filter Envelope Rates < Velocity (Time < Vel) — This control is present for the filter, pitch, LFO and volume envelopes alike. For that reason it is documented in the section on envelopes.

Filter Frequency < Envelope (Envelope): This setting controls how strongly the filter envelope modulates the filter frequency. At 100% the envelope is capable of shifting the frequency by roughly 9 octaves at most.

Filter Drive (Flt. Drive) — Adds extra input gain to the signal ahead of the filter.

Morph: Sets where the Morph filter sits within its morph cycle.

Shaper: A chooser that picks the curve used by the filter’s waveshaper.

Shaper Drive (Shp. Drive) — Raises or lowers the level of the signal feeding the waveshaper.

Dry/Wet: Sets the mix between the untouched signal and the one shaped by the waveshaper.

<a id="source-309105-lfo-shell-and-display"></a>
#### 30.9.10.5 LFO Shell and Display

LFO On: Switches the LFO (low-frequency oscillator) on or off. Leaving it off while unused reclaims a little CPU power.

LFO Waveform: Pick from a handful of common LFO waveforms. Sample and Hold (S&H) produces random steps, while Noise delivers band-pass filtered noise. Every waveform is band-limited so that stray clicks are avoided.

LFO Range: A vast frequency span is covered by the LFO. Pick Low for anything from 50 seconds up to 30 Hz, or Hi for 8 Hz through 12 kHz. With Sync, the LFO’s rate locks to your Set’s tempo. Because such high frequencies are possible, the LFO can double as a fifth oscillator.

Retrigger (R): With this on, the LFO jumps back to the identical phase position whenever a note fires. With R off, the LFO keeps running freely.

LFO Rate (Rate): Sets the rate of the LFO. Its true frequency also hinges on how the LFO Range and the LFO Rate < Key controls are set.

LFO Amount (Amount): Sets the LFO's overall intensity. Keep in mind that the actual outcome also hinges on the LFO envelope.

LFO to Osc (Destination A-D): When this is switched on, the LFO modulates the frequency of the corresponding oscillator.

LFO to Filter Cutoff Frequency (Destination FIL) — When this is switched on, the LFO modulates the cutoff frequency of the filter.

LFO Amount A: Sets how strongly the LFO modulates the oscillators and filter.

LFO Destination B: Selects the LFO's second modulation destination.

LFO Amount B: Sets how strongly the LFO modulates the secondary target.

LFO Envelope Rates < Velocity (Time < Vel) — This control is present for the filter, pitch, LFO and volume envelopes alike. For that reason it is documented in the section on envelopes.

LFO Rate < Key (Rate < Key) — Note pitch can govern the LFO’s frequency. Set to 100%, the LFO doubles its frequency every octave, behaving like an ordinary oscillator.

LFO Amount < Velocity (Amt < Vel) — This control tunes how much note velocity modulates the LFO intensity.
