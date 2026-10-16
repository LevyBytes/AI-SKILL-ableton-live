# Simpler Filter Types And Controls

Open when you need guidance on Simpler Filter Types And Controls in Ableton Live.

Context: [Filter](sampler-modulation-and-simpler-routes.md#30113-filter).

<a id="source-live-instrument-reference-part-9"></a>

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
