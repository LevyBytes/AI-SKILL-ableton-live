# Wavetable Oscillators Sub And Filters

Open when you need guidance on Wavetable Oscillators Sub And Filters in Ableton Live.

Context: [Wavetable](tension-and-wavetable-routes.md#3013-wavetable).

<a id="source-30131-wavetable-synthesis"></a>
### 30.13.1 Wavetable Synthesis

Sound from Wavetable’s oscillators is generated through a method known as wavetable synthesis. At its core, a wavetable is just a freeform set of short, looping samples laid out side by side. Lock the oscillator onto a single one of those samples and a held note rings out with one fixed timbre. The technique’s real strength, though, emerges when you sweep across the samples in the table while the note sounds, giving a timbre that morphs as it plays. That makes wavetable synthesis an excellent fit for evolving, time-varying sounds.

<a id="source-30132-oscillators"></a>
### 30.13.2 Oscillators

The oscillators in Wavetable are tuned for the highest possible sound quality. Provided you apply no modulation, their unprocessed output is fully band-limited, so no aliasing artifacts appear regardless of the pitch you play.

Wavetable’s Oscillators.

A switch on each oscillator’s tab lets you enable or disable that oscillator on its own. Clicking the tab brings the oscillator into focus and exposes its parameters for editing.

Each oscillator’s total output level rides on its Gain slider, and its placement across the stereo image is handled by the Pan control. Coarse and fine tuning are dialed in with the Semi and Detune controls, with that tuning measured relative to the global Transposition slider.

Pick a wavetable by way of the choosers or the arrow buttons. The first chooser narrows you to a wavetable category, and the second drills down to a particular wavetable inside it. Once you hit the last entry in a category, the arrow buttons roll over to the next one automatically, letting you scroll straight through every wavetable using only the arrows.

You can broaden the oscillator section’s palette by importing any WAV or AIFF file to serve as a wavetable. Just drag a sample out of the browser and drop it onto the wavetable visualization. From then on the choosers and arrow buttons point at the folder that holds your imported sample, so you can swiftly preview the other samples sitting alongside it.

Imported samples are processed automatically by Wavetable to cut down on unwanted artefacts. You can skip that processing, though, by turning on the Raw mode switch. Raw mode comes in handy above all when you load files already crafted specifically to act as wavetables. That said, it can equally be “misused” to conjure unpredictable, noisy or glitchy textures.

Wavetable’s Raw Mode Switch.

A display in the middle of the oscillator tab visualizes that oscillator’s wavetable. Drag inside this display to jump to another spot within the wavetable, or alternatively move there with the Wave Position slider.

The wavetable visualization switch flips between two available visualization styles. Each conveys identical information, just rendered differently. In the linear view the waveforms stack from bottom to top with time advancing left to right, whereas the polar view draws them as loops running from the inside outward with time advancing clockwise.

Plentiful as the wavetable selection is, you can also reshape any wavetable’s sound itself using oscillator effects. Choose one of three effects in the chooser, then tune their parameters with the sliders on the right. These oscillator effects are:

- FM — Imposes frequency modulation on the oscillator. The Amt slider scales how strong that frequency modulation is, while the Tune slider sets the pitch of the modulating oscillator. At a tuning of 50% (and -50%) the modulating oscillator lands an octave above (or below) the main one. At 100% (and -100%) it sits two octaves above (or below). Anywhere in between leaves the modulating oscillator at inharmonic ratios, perfect for spawning gritty overtones.
- Classic — Offers two modulation flavors familiar from vintage analog synths. PW changes the waveform’s pulse width. Bear in mind that hardware synths usually only let you vary pulse width on square waves, whereas Wavetable allows it across every wavetable. Sync brings in a “hidden” oscillator that resets the phase of the one you hear, reshaping its timbre.
- Modern — Supplies two more ways to warp the waveform’s shape. Warp behaves much like pulse width, and Fold introduces wavefolding distortion.

Keep in mind that switching the effect type leaves the two effect parameter values where they are. That lets you hop between effects and audition how each process colors the timbre using identical settings.

<a id="source-30133-sub-oscillator"></a>
### 30.13.3 Sub Oscillator

Wavetable’s Sub Oscillator.

Beyond its two primary oscillators, Wavetable also carries a sub oscillator. The Sub toggle switches it on or off, and the Gain knob sets its output level.

Reaching for the Tone control reshapes the sub oscillator’s timbre. Held at 0% it puts out a clean sine wave, and raising Tone adds harmonic content to the waveform.

The sub’s pitch follows the note you play together with the global Transpose value, though the Octave switches let you drop the sub one or two octaves lower.

<a id="source-30134-filters"></a>
### 30.13.4 Filters

The filters in Wavetable are a great tool for carving up the harmonically dense timbres the oscillators and their effects throw off. And because those oscillators also hand you the classic analog-synth waveforms, putting together a subtractive-style synth is a breeze.

Wavetable’s Filters.

You get an assortment of filter types in Wavetable — low-pass, high-pass, band-pass, notch, plus a distinctive Morph filter. Every filter can be set to either a 12 or 24 dB slope, and you can pick from a range of analog-modeled circuit behaviors, built together with Cytomic, that recreate the hardware filters of certain classic analog synths.

The Clean circuit is a top-quality, CPU-light design — the very same filtering found in EQ Eight — and it works with every filter type.

The OSR circuit is a state-variable design whose resonance is reined in by a distinctive hard-clipping diode. It’s patterned on the filters of a fairly uncommon British monosynth and is offered for all filter types.

The MS2 circuit relies on a Sallen-Key topology with soft clipping to cap resonance. Modeled on the filters of a celebrated semi-modular Japanese monosynth, it’s offered for the low-pass and high-pass filters.

The SMP circuit is a bespoke design tied to no specific hardware. Blending traits of both the MS2 and PRD circuits, it’s offered for the low-pass and high-pass filters.

The PRD circuit employs a ladder design and applies no deliberate resonance limiting. It’s modeled on the filters of a vintage dual-oscillator monosynth from the United States and is offered for the low-pass and high-pass filters.

Frequency and Resonance are the two filter parameters that matter most, the usual synth staples. Frequency picks the spot in the harmonic spectrum where the filter acts, and Resonance lifts the frequencies right around that spot. You can also set both Frequency and Resonance by dragging either of the filter dots within the filter display.

Engaging the low-pass, high-pass, or band-pass filter with any circuit other than Clean exposes an extra Drive control, which you can use to push gain or distortion into the signal ahead of the filter.

For the Morph filter there’s an added Morph control that continuously glides the filter type from low-pass through band-pass and high-pass to notch, then loops back to low-pass.

Filter routing lets you wire the filters together in different layouts for wildly varied sculpting approaches. Three routings are on offer:

- Serial — Sends every oscillator into Filter 1, then feeds Filter 1 into Filter 2. Sub goes to both filters.
- Parallel — Feeds the two main oscillators separately into Filter 1 and Filter 2. Sub goes to both filters.
- Split — Routes Oscillator 1 into Filter 1, while Oscillator 2 heads into Filter 2. Sub gets divided in two and supplied to both filters. Should either filter be switched off, you’ll still hear the matching oscillator’s signal. Split lets you process each filter on its own, which is handy when you’re after layered synth tones. And with the main oscillators turned off while both filters stay active, Split doubles as a way to lavish extra processing on the Sub oscillator.
