# Simpler Envelopes LFO And Global Controls

Open when you need guidance on Simpler Envelopes LFO And Global Controls in Ableton Live.

Context: [Simpler](sampler-modulation-and-simpler-routes.md#3011-simpler).

<a id="source-30114-envelopes"></a>
### 30.11.4 Envelopes

Simpler’s Filter and Amplitude Envelope Controls.

Like most synthesizers, Simpler provides three traditional ADSR envelopes for sculpting how the sample evolves over time. You can edit modulation of amplitude, filter frequency, and pitch by switching on their respective buttons in the envelope section. Attack sets, in milliseconds, how long the envelope needs to climb to its maximum once a note triggers. Decay governs how long the envelope takes to fall to the Sustain level, where it stays put until the note ends. Release determines, once the note finishes, how long the envelope needs to fall from the Sustain level all the way to zero. You can tweak these values with their dedicated controls or graphically by dragging the handles inside the envelope displays.

How strongly the envelopes act on filter cutoff and on pitch is set through the envelope amount controls located at the upper right of each of those sections.

The Filter and Pitch Envelope Amount Controls.

You can loop the Amplitude Envelope using the Loop Mode chooser. Under Loop and Trigger modes, should a note remain held once the Decay stage finishes, the envelope returns to its starting value. How quickly it travels from the Sustain level back to that starting value is governed by the Time parameter. Under Beat and Sync modes, if a note is still held past the duration set by the Rate slider, the envelope likewise returns to its starting value.

The Amplitude Envelope Loop Mode Chooser and Time Control.

<a id="source-30115-lfo"></a>
### 30.11.5 LFO

Simpler’s LFO Section.

Waveform options in the LFO (low-frequency oscillator) section include sine, square, triangle, sawtooth down, sawtooth up and random. You can let the LFO oscillate freely anywhere from 0.01 to 30 Hz, or lock it to subdivisions of the Set's tempo. In Simpler, an LFO operates separately for every _voice_, that is, each note being sounded.

How long the LFO takes to climb to full strength is set by the Attack control. Retrigger is toggled by the R switch. With it active, the LFO's phase snaps back to the Offset value at the onset of each note. Keep in mind that Offset does nothing while Retrigger is switched off.

Each LFO's Rate is scaled relative to the pitch of arriving notes by the Key parameter. With a high Key value, higher notes receive a faster LFO rate. When Key sits at zero, every voice's LFO shares one rate and might vary only in phase.

How far the LFO modulates volume, pitch, pan, and filter is governed by the Volume, Pitch, Pan, and Filter sliders, in that order.

<a id="source-30116-global-parameters"></a>
### 30.11.6 Global Parameters

Simpler’s Global Parameters.

The stereo placement is set with the Pan control, though it can be nudged additionally by randomness (using the Random > Pan slider) or driven by the LFO.

Simpler additionally provides a dedicated Spread parameter that produces a lush stereo chorus by sounding two voices for each note, with one panned left and the other right. Those two voices are detuned from one another, and the degree of detuning is dialed in with the Spread control.

Whether a given note receives spread is decided by where the Spread parameter sits at the moment of the Note On event. For unusual results you might, for example, build a pattern in which Spread stays at zero most of the way and is engaged only for a handful of notes. Those notes then sound in stereo while the rest remain mono.

Simpler's overall output level is set by the Volume control, which may additionally respond to note velocity according to the Velocity > Volume control. You can produce tremolo by letting the LFO drive the Volume parameter.

When the arriving MIDI note is C3, Simpler reproduces a sample at its native pitch, but the Transpose control lets you shift it by +/- 48 semitones. The LFO or the pitch envelope can also modulate pitch. That pitch envelope is particularly useful for crafting percussive tones. Simpler responds to MIDI Pitch Bend data with a range of +/- 5 semitones. The Transpose parameter can additionally be driven by clip envelopes and outboard controllers. To fine-tune pitch, turn to the Detune control, adjustable across +/- 50 cents.

A glide capability is built into Simpler. With it switched on, a fresh note begins at the pitch of whatever note preceded it, then glides smoothly to its target pitch. There are two glide modes: Glide operates monophonically, and Portamento operates polyphonically. The glide's speed is dialed in with the Time control.

<a id="source-30117-context-menu-options-for-simpler"></a>
### 30.11.7 Context Menu Options for Simpler

Certain Simpler functions become available only when you open the context menu from either the sample display or Simpler's title bar.

Out of the box, Simpler applies constant-power fades. To switch instead to linear crossfades, open the context menu on Simpler's title bar and uncheck the entry labeled “Use Constant Power Fade for Loops“. Bear in mind the Fade parameter disappears whenever warp is switched on.

Presets built in Simpler may be translated for use in [Sampler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sampler), and the reverse works too. Accomplish this by right-clicking Simpler's title bar and selecting the Simpler -> Sampler command. Doing so lets a Simpler preset sit inside a multisample setup within Sampler. Be aware, though, that Sampler lacks Simpler's warping and slicing features, so any preset relying on those will sound and act quite differently once it reaches Sampler.

Choosing Manage Sample displays the loaded sample inside Live's [File Manager](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#managing-files-in-a-project), whereas Show in Browser surfaces it in Live's browser. Show in Finder/Explorer opens the sample inside its containing folder in your computer's OS. Keep in mind this entry is absent for samples that originated from official Ableton Packs.

The Normalize Volumes command raises the loaded sample's level so its loudest peak fills the entire available headroom.

The Crop command discards whatever sits beyond the Start and End markers, while Reverse plays the whole sample in reverse. Both Crop and Reverse leave your data intact: they duplicate the sample and operate on the copy, so the source remains untouched.

While in Slicing Playback Mode, two extra context-menu entries appear. Slice to Drum Rack swaps the Simpler for a Drum Rack where every existing slice lands on its own pad. Slice to New MIDI Track behaves much the same, except it adds a separate track holding a Drum Rack instead of swapping out the current Simpler. On top of that, slicing to a new track produces a clip that triggers the slices in sequence. For deeper coverage of slicing, consult the [dedicated section](https://www.ableton.com/en/live-manual/12/converting-audio-to-midi/#slice-to-new-midi-track) on the subject.

<a id="source-30118-strategies-for-saving-cpu-power"></a>
### 30.11.8 Strategies for Saving CPU Power

Synthesis on the fly demands considerable processing. There are, however, ways to lighten the CPU burden. Trim the CPU that Simpler consumes by applying some of these measures:

- During warping, keep in mind that the Complex and Complex Pro modes draw far more CPU than the remaining Warp Modes.
- Switch off the Filter whenever you don't need it.
- The CPU demand of a filter rises with how steep its slope is — the 24 dB slope costs more than the 12 dB slope.
- Disabling the LFO gives CPU a modest break.
- Because they double the workload, stereo samples consume far more CPU than mono ones.
- Lower how many voices may sound at once using the Voices control.
- Set Spread to 0% whenever it isn't required.
