# Spectral Resonator Pitch Modulation And Output

Open when you need guidance on Spectral Resonator Pitch Modulation And Output in Ableton Live.

Context: [Spectral Resonator](roar-saturator-shifter-spectral-resonator-routes.md#2836-spectral-resonator).

<a id="source-28361-pitch-mode-section"></a>
### 28.36.1 Pitch Mode Section

Spectral Resonator’s Pitch Mode Section.

Spectral Resonator gives you a choice of two modes governing how the fundamental pitch of its resonant harmonics is established: Internal or MIDI.

With Internal mode active, the device stays locked to one pitch; under MIDI mode, by contrast, external note input tunes the resonator dynamically. Switching on MIDI mode reveals some extra controls:

- _External Source_ and _Tapping Point_ allow you to pick any MIDI track as the input source and to decide whether the signal is captured before or after the MIDI effects in that track’s device chain. For an external MIDI controller, choose it in the Input Type chooser on a MIDI track, and then point Spectral Resonator’s External Source chooser at that track.
- Toggling _Mono/Poly_ flips between single-voice and polyphonic operation. With Poly selected, Spectral Resonator can take in polyphonic material like chords.
- The number of voices the effect runs, anywhere from 2 to 16, is set by the _Polyphony_ slider.
- How the resonator gets triggered is decided by the _MIDI Gate_ toggle. With it On, the device behaves more like an instrument and resonates only while MIDI notes are being played. With it Off, the resonator keeps reacting to audio input even when no notes arrive. Keep in mind that MIDI Gate stays active at all times in Poly mode.
- _Glide_ sets, in milliseconds, how long pitch takes to slide from one note to the next. Note that this parameter works only in Mono mode.
- _PB_ determines how far MIDI pitch bend messages move the resonator’s pitch, across 0-24 semitones. Note that Spectral Resonator can also take in MPE data.

<a id="source-28362-frequency-section"></a>
### 28.36.2 Frequency Section

The Frequency Section in Spectral Resonator.

With Internal pitch mode active, Spectral Resonator tunes to whatever frequency the Freq control specifies. The frequency can be dialed in Hertz or pinned to a particular pitch; flip between those two options with the Frequency Control Mode buttons sitting beneath the Freq control. Should the Use Current Scale toggle be on, the device tracks the active clip scale instead. At that point the control turns into SD Shift, letting you transpose the resonator by scale degrees. Note that with scale awareness on but no scale active, Spectral Resonator defaults to the chromatic scale.

Under MIDI mode, Spectral Resonator tunes to the frequencies of the MIDI notes coming in. That MIDI input can be transposed up to ±48 semitones with the Transp. control, or up to ±28 scale degrees when Use Current Scale is engaged. Once the effect is scale aware, Transp. turns into the SD Shift control.

In both modes Spectral Resonator supports tuning systems. While a tuning system is in effect, the Freq control under Internal mode and the Transp. control under MIDI mode rely on note indices rather than note names and semitones, respectively.

Spacing between the resonant harmonics is set with the Stretch slider. Settings under 0% pull that spacing tighter, while settings above 0 push it wider. At 100%, only odd harmonics survive, giving you a square-wave-like timbre.

By ±48 semitones, the Shift slider transposes the spectrum of the input signal. Note that what it alters is the signal entering the device, not the resonator’s own spectrum.

How long the resonances hang on is controlled by the Decay control. Larger values yield longer, sustained tones.

HF Damp governs how much damping is applied to high-frequency partials, and LF Damp governs how much is applied to low-frequency partials. For each of these, the targeted frequency ranges move along with the current pitch (under Internal mode) or with the pitch of the incoming MIDI notes (under MIDI mode).

<a id="source-28363-modulation-section"></a>
### 28.36.3 Modulation Section

Spectral Resonator’s Modulation Section.

Using the corresponding toggles, you can put the effect into any of four modulation modes: None, Chorus, Wander, or Granular. Which mode you choose dictates how each harmonic’s pitch and amplitude get modulated:

- _None_ leaves the signal unmodulated.
- _Chorus_ drives every partial with triangle wave modulation. With Mod Rate at 0, this mode modulates nothing but the amplitudes of the partials.
- _Wander_ draws on random sawtooth waveforms to modulate each partial.
- _Granular_ randomly modulates the amplitude of every partial by means of exponential decay envelopes. Its partials emerge at uneven intervals, and the Mod Rate parameter governs how dense they become.

The Mod Rate and Pch. Mod controls bear on all of the modulation modes. Mod Rate establishes the modulation rate, and Pch. Mod sets the span of pitch modulation in semitones. Even though Pch. Mod shows only a positive figure, the pitch modulation runs bipolar in every mode apart from Granular, where the grain envelopes act in a positive direction alone.

<a id="source-28364-spectrogram"></a>
### 28.36.4 Spectrogram

Spectral Resonator’s Display with Integrated Controls.

A spectrogram is built into Spectral Resonator, charting how frequencies in the dry and wet signals behave over time. The dry signals appear in yellow and the wet ones in blue. The toggle at the display’s upper-left corner lets you tuck the spectrogram away. This visualization makes it easier to spot which parts of the spectrum the resonator is boosting or reshaping.

The spectrogram display houses two controls: Harmonics and Quantize. Harmonics lets you choose how many resonant harmonics the device employs. Larger values brighten the sound, while smaller ones darken the timbre. Note that under polyphony the harmonics are split evenly among the voices, so each voice gets fewer of them at high voice counts. Pushing the harmonics up also raises CPU usage.

With Quantize switched on, every harmonic snaps to the active scale or tuning system. When neither a scale nor a tuning system is active, the harmonics instead snap to chromatic pitches.

<a id="source-28365-global-parameters"></a>
### 28.36.5 Global Parameters

The Global Controls in Spectral Resonator.

How much gain is applied to the processed signal is set by the Input Send control. A built-in limiter keeps the signal from clipping, and the LED beside Input Send lights up whenever that limiter kicks in.

The Unison parameter dictates how many unison voices there are, each being a detuned copy of the resonator’s partials. The Uni. Amt parameter sets how much detuning separates those voices. Adding more voices fattens the sound, while greater detuning values lend a broader, livelier character. Within the Wander and Granular modulation modes, every voice is modulated on its own, which builds particularly thick and warbly textures.

How the processed and unprocessed signals balance, and how strongly each one shows up in the spectrogram, is set by the Dry/Wet control. When Spectral Resonator sits on a return track, set Dry/Wet to 100%.

<a id="source-28366-spectral-resonator-tips"></a>
### 28.36.6 Spectral Resonator Tips

The following are a few approaches for putting Spectral Resonator to work in your projects:
