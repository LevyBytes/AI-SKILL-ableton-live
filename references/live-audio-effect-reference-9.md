# Live Audio Effect Reference (part 9)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Activating the Compressor Sidechain HP Filter toggle routes a high-pass filter onto the detection signal that feeds the compressor’s sidechain. The benefit here is reducing how much gain reduction occurs when the compressor reacts to low frequency content.

Positioned ahead of a hard clipping stage that then passes into the Dry/Wet stage, the Output Gain knob determines the output level of the wet signal. Reach for this parameter whenever you need to offset level shifts caused by the Drive or Shaper Amount knobs.

Use the Dry/Wet slider to set how the dry and wet portions of Roar’s output are balanced against each other.

### 28.33.6 Sidechain Parameters

Out of the box, Roar relies on its own input signal both to feed its envelope follower and to determine its feedback pitch. With the Sidechain section, however, you can substitute external audio and MIDI signals for that role. Reveal the external and MIDI sidechain controls by clicking the Sidechain Section toggle located at the device’s top-left corner.

Roar’s Sidechain Parameters.

Turn on the External SC toggle to activate the external sidechain. After it is enabled, the External Source chooser lets you point to whichever signal you want to use. The External Tapping Point chooser additionally controls whether that signal arrives Post FX or Post Mixer.

With the Mix slider, you can blend the external and internal sidechain signals together so they jointly act as the envelope follower’s trigger. Setting it to 100% makes the envelope follower follow only the external sidechain source, whereas at 0% just the internal sidechain feeds it.

Adjust the incoming level of the external sidechain through the SC Gain control. Keep in mind that this sidechain audio serves purely as a trigger for the envelope follower, so raising the gain has no bearing on how loud the source signal sounds.

Enable the MIDI > FB Note toggle so that MIDI input governs the pitch of Roar’s feedback engine whenever the [feedback mode](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#feedback-section) is configured to Note. After the MIDI sidechain is on, the External Source chooser found beneath MIDI From selects which MIDI sidechain source is used. The Tapping Point chooser likewise sets whether the signal is captured Pre FX or Post FX.

Be aware that while the MIDI sidechain is engaged, the Feedback Mode and Feedback Amount controls within the [feedback section](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#feedback-section) become inactive.

Activate the Sidechain Listen toggle to audition the sidechain signal on its own. Doing so mutes Roar’s normal output so you can listen straight to the sidechain input, which comes in handy while you dial in the sidechain settings.

The Sidechain Listen Toggle.

### 28.34 Saturator

The Saturator Effect.

As a waveshaping effect, Saturator lends your sound the grit, punch, or warmth it might be lacking. It achieves this by subjecting the input signal to non-linear shaping, producing anything from gentle saturation through to heavy coloration.

The way Saturator works is by remapping every single sample value in the incoming signal to a fresh value, guided by whichever shaping curve you pick. Since that mapping is generally non-linear, the signal ends up being reshaped on the fly according to how loud it is from one instant to the next.

The Curve Type chooser is where you pick which curve handles the input shaping. Eight options are offered. The first four are Analog Clip, Soft Sine, Bass Shaper, and Medium Curve; the remaining four are Hard Curve, Sinoid Fold, Digital Clip, and Waveshaper.

Each curve type carries its own shaping behavior. Once the clipping point is crossed, Digital Clip clips abruptly and hard, whereas Analog Clip eases through that point more gently. Below the clipping point, both of these curves stay linear. Saturation with distinct tonal flavors is provided by the Soft Sine, Medium Curve, and Hard Curve options. As a wavefolding curve, Sinoid Fold makes the output fold back on itself as the input grows louder, yielding strange textures.

Although the Bass Shaper curve resembles Analog Clip in some respects, it delivers a cleaner harmonic spectrum when low frequency signals are pushed with high gain. That trait makes it well suited to low-end material such as 808 kick drums and synth basslines.

A separate Bass Shaper Threshold control comes with Bass Shaper and defines the curve’s threshold across a range of 0 to -50 dB. As long as the input stays under the threshold the curve stays linear, but it begins clipping gradually once the signal rises past that point. This lets you transition smoothly from one clipping style into another: lower threshold settings yield soft clipping while higher ones yield hard clipping. For bass material the lower threshold settings are most effective, particularly alongside high Drive values.

If you want the boldest shaping of all, choose the Waveshaper curve. It comes with a dedicated control set of its own that you open by clicking the Toggle Expanded View button on the device title bar; further detail on how those parameters shape the signal appears in [the dedicated section below](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#saturators-waveshaper-controls).

Serving two purposes at once, the Shaper Curve display visualizes Saturator’s shaping curve and, in real time, plots the input signal against the chosen curve type. Saturation kicks in wherever the input reaches the curve’s non-linear regions.

A post-clipping stage applicable to every curve type can be chosen from the Post Clip Mode chooser sitting beneath the Shaper Curve display. With either Soft Clip or Hard Clip engaged, Saturator’s output stays at or below the ceiling defined by the Output control. That proves especially handy for taming any extra boost introduced by negative Color values.

Engaging the Color toggle activates the device’s pair of color filters, which draw a color curve shown in the device’s expanded view. These filters impose an EQ curve once before the shaper and then once more, inverted, after it. As a result you could, for instance, strip out bass frequencies ahead of the shaper so that only the mid and high range gets saturated while the bass energy is preserved in the output.

The Amt Lo slider lets you set how much saturation reaches the low frequencies. Going negative pulls back the total saturation on the lows, whereas going positive boosts it.

Before Saturator processes the signal, the Drive control raises its input gain. The extent of that effect on the input is visible inside the device’s Shaper Curve display.

Saturator’s final output level is reduced by the Output control. Whenever Soft Clip is engaged in the Post Clip Mode chooser, Saturator additionally runs an Analog Clip curve across the device’s output.

How the dry and processed signals are balanced at Saturator’s output is governed by the Dry/Wet control. When Saturator sits on a return track, set this to 100%.

Found in the expanded view, the Color Curve display renders a picture of the curve produced by the device’s two color filters.

The Color Curve Display and Color Filter Parameters.

Three further controls for sculpting Saturator’s color filters sit underneath the display. The Amt Hi slider governs how much saturation the second filter applies across the chosen frequency range. Going positive piles on more saturation while going negative pulls it back. With the Frequency slider you set the center frequency that the second color filter targets, and Width sets how broad a span of frequencies it touches.

These color filter settings can also be edited by dragging the handles within the Color Curve display — moving the first handle controls the Amt Lo parameter, while moving the second handle controls either the Amt Hi or the Frequency parameter, according to whether you drag it horizontally or vertically.

#### 28.34.0.1 Saturator’s Waveshaper Controls

Choosing the Waveshaper curve type brings six extra parameters to life in the expanded view.

The Waveshaper Controls.

Here is how the Waveshaper controls shape the device’s signal-processing behavior:

- _Drive_ sets the degree to which the Waveshaper curve’s parameters act on the input signal. At 0%, those parameters leave the Waveshaper curve untouched, while at 100% they shape the curve completely.
- _Curve_ contributes primarily third-order harmonics to the input signal.
- _Depth_ governs how tall a sine wave is laid over the top of the Waveshaper curve. Raising the value lifts that sine wave’s amplitude so it bends the shaping curve more strongly. At 0%, the sine wave exerts no effect.
- _Linear_ operates together with the Curve and Depth parameters to reshape the linear region of the Waveshaper curve.
- _Damp_ levels off any signals sitting close to the waveform’s center. Its behavior resembles an extremely fast noise gate.
- _Period_ sets how tightly the ripples in the overlaid sine wave are packed, relative to the Depth control.

#### 28.34.0.2 Context Menu Options for Saturator

Saturator’s context menu exposes two further modes you can switch on: Hi-Quality and Pre-DC Filter. Engaging Hi-Quality mode cuts down aliasing and raises audio fidelity (most noticeably on high frequency signals), though it draws a little extra CPU. Turning on Pre-DC Filter mode inserts a DC filter at Saturator’s input stage, handy for stripping DC offsets out of audio that carries them.

### 28.35 Shifter

The Shifter Effect.

Shifter is a versatile pitch- and frequency-shifting audio effect, capable of layering ring modulation over incoming audio or of moving the pitch or frequency of that audio on the fly.

### 28.35.1 Tuning and Delay Section

Shifter’s Tuning and Delay Section.

Depending on the active shift mode (covered in the [Shifter Mode](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#shifter-mode-section) section), the Coarse and Fine knobs move the pitch or the frequency by the amount you dial in.

Switching on the Wide button flips the polarity of the Spread value for the right channel, yielding a stereo effect. In practice, raising the Spread value drives the frequency downward in the right channel and upward in the left. Bear in mind that Wide does nothing when the Spread value sits at 0.

While in Pitch mode, the Window slider controls the size of the window the algorithm employs. Longer window sizes tend to suit low frequency signals, whereas shorter ones tend to favor high frequencies. Tone trims the highs from the delay’s feedback path.

Switching on the Delay button introduces delay time, which the slider control lets you specify either in Hertz or in beat-synced divisions according to the Delay Mode button you pick. How much of the output is routed back into the delay’s input is governed by the Delay Feedback knob.

### 28.35.2 LFO Section

Shifter’s LFO Section.

Shifter’s LFO gives you a way to modulate both the left and right stereo channels.

Within the LFO waveform display sit the Duty Cycle and Phase/Spin/Width controls. Duty Cycle determines the duty cycle of the LFO waveform. Phase sets the offset separating the left- and right-channel waveforms; at 180° the two LFOs end up exactly out of phase. According to the LFO waveform in use or the Rate parameter, a Spin or Width control may take the place of Phase, as described further on.

Should the Rate parameter (detailed more fully below) be set to beat-synced time divisions, an Offset parameter appears alongside the Phase parameter, nudging the point at which each LFO begins along its waveform.

The LFO drop-down menu holds a number of LFO waveforms to pick from. The first group covers Sine, Triangle, Triangle Analog, Triangle 8, and Triangle 16; the rest are Saw Up, Saw Down, Rectangle, Random, and Random S&H.

The option of Spin in place of Phase is available for these waveforms: Sine, Triangle, and Triangle Analog, together with Triangle 8, Triangle 16, Saw Up, Saw Down, and Rectangle. Spin pushes the two LFO speeds slightly apart from each other.

By contrast, the Random and Random S&H waveforms allow only Phase and Width, respectively. Width controls the Stereo width of the random LFO waveform. At 0%, both the left and right channels share an identical waveform. At 100%, the waveform becomes fully stereo, so a peak on the left lines up with a trough on the right and the reverse as well.

The Rate parameter steers LFO modulation and may be specified in Hertz or locked to the song tempo in meter subdivisions (for example, sixteenth notes). How strongly that LFO modulation hits the incoming signals is set by the Amount parameter.

### 28.35.3 Envelope Follower Section

Shifter’s Envelope Follower.

Taking the amplitude of an incoming audio signal, Shifter’s envelope follower converts it into a modulation source.

The Envelope Attack governs how fast the envelope follower reacts as input levels climb, and the Envelope Release governs how fast it reacts as those levels fall.

Shifter’s envelope follower is turned on with the Env Fol button. The Amount dials in the strength of the envelope follower’s modulation. You can specify the Amount value in semitones while in Pitch mode, or in Hertz when using the Freq and Ring modes.

### 28.35.4 Shifter Mode Section

The Shifter Mode Section.

You can choose among three Shifter Mode button switches: Pitch, Freq, and Ring.

In Pitch mode, the incoming audio is shifted up or down by an amount you set in semitones (Coarse tuning) and cents (Fine tuning).

Freq mode displaces the frequencies of the incoming audio up or down by an amount you specify in Hertz. Modest shifts can yield gentle tremolo or phasing, whereas large ones can generate clashing, metallic timbres.

Within Ring mode, the frequency amount you specify in Hertz gets both added to and subtracted from the input.

Drive switches on a distortion effect, with the slider beneath it setting the distortion level. Note: Drive is offered only within Ring mode.

How the dry and processed signals balance out at Shifter’s output is determined by the Dry/Wet knob.

### 28.35.5 Sidechain Parameters

Shifter’s Sidechain Parameters.

Reach the Sidechain parameters by expanding the Shifter window via the triangle button at the left edge of the title bar. Two Pitch Modes control how the pitch or frequency gets established: Internal and MIDI. Under Internal mode, Shifter’s Coarse and Fine knobs set the pitch or frequency, while under MIDI mode an incoming MIDI note does so.

While in MIDI mode, a drop-down menu appears for picking an external MIDI source. A Glide parameter is also present, setting the time in milliseconds it takes for notes to glide their pitch toward the next incoming pitch. Using the PB slider, you can establish a pitch bend range from 0-24 semitones that determines how MIDI pitch bend messages behave.

### 28.35.6 Shifter Tips

#### 28.35.6.1 Pitch-shifted Drum Layers

For glitchy, metallic echoes on a drum loop, make a copy of your drum track and place Shifter after the Drum Rack. While in Pitch mode, try tweaking or automating the Coarse knob and switch on the Delay button. The larger pitch shifts produce a crisp, metallic echoed delay, whereas smaller ones produce a more stretched-out delay. Dropping the volume of the pitch-shifted track keeps it sitting underneath, lending a bit of motion to the primary drum track.

#### 28.35.6.2 Phasing Effects

For rich phasing effects, nudge the Fine knob only slightly (around 2 Hz at most) while in Freq mode. The phasing comes from how the processed and dry signals interact, so set the Mix balance to keep both within earshot. You will hear the most pronounced phasing with MIx at 50%.

#### 28.35.6.3 Tremolo Effects

Within Ring mode, frequencies that fall beneath what we can hear (roughly 20 Hz or a touch under) bring about a tremolo effect. To add a feeling of stereo movement to that tremolo, switch on Wide and keep the Spread values small.

### 28.36 Spectral Resonator

The Spectral Resonator Effect.

By imposing tuned resonances across a signal’s spectrum, Spectral Resonator reshapes the audio. You can spotlight selected frequencies among the resonating partials and reshape their decay, producing either brief percussive reverberations or lengthy, washed-out tones. The frequencies that get affected are chosen either through an internal resonator or through an external MIDI sidechain. Much like a vocoder, the MIDI input lets you lock the resonances to the key of the music around them, and you can play the effect polyphonically across as many as 16 voices. Further sculpting is possible with the various modulation modes, which inject movement and depth or yield more broken-up, textural outcomes. On top of that, the effect handles [scale awareness](https://www.ableton.com/en/live-manual/12/live-concepts/#scale-awareness) and [tuning systems](https://www.ableton.com/en/live-manual/12/using-tuning-systems/#using-tuning-systems).

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

### 28.36.2 Frequency Section

The Frequency Section in Spectral Resonator.

With Internal pitch mode active, Spectral Resonator tunes to whatever frequency the Freq control specifies. The frequency can be dialed in Hertz or pinned to a particular pitch; flip between those two options with the Frequency Control Mode buttons sitting beneath the Freq control. Should the Use Current Scale toggle be on, the device tracks the active clip scale instead. At that point the control turns into SD Shift, letting you transpose the resonator by scale degrees. Note that with scale awareness on but no scale active, Spectral Resonator defaults to the chromatic scale.

Under MIDI mode, Spectral Resonator tunes to the frequencies of the MIDI notes coming in. That MIDI input can be transposed up to ±48 semitones with the Transp. control, or up to ±28 scale degrees when Use Current Scale is engaged. Once the effect is scale aware, Transp. turns into the SD Shift control.

In both modes Spectral Resonator supports tuning systems. While a tuning system is in effect, the Freq control under Internal mode and the Transp. control under MIDI mode rely on note indices rather than note names and semitones, respectively.

Spacing between the resonant harmonics is set with the Stretch slider. Settings under 0% pull that spacing tighter, while settings above 0 push it wider. At 100%, only odd harmonics survive, giving you a square-wave-like timbre.

By ±48 semitones, the Shift slider transposes the spectrum of the input signal. Note that what it alters is the signal entering the device, not the resonator’s own spectrum.

How long the resonances hang on is controlled by the Decay control. Larger values yield longer, sustained tones.

HF Damp governs how much damping is applied to high-frequency partials, and LF Damp governs how much is applied to low-frequency partials. For each of these, the targeted frequency ranges move along with the current pitch (under Internal mode) or with the pitch of the incoming MIDI notes (under MIDI mode).

### 28.36.3 Modulation Section

Spectral Resonator’s Modulation Section.

Using the corresponding toggles, you can put the effect into any of four modulation modes: None, Chorus, Wander, or Granular. Which mode you choose dictates how each harmonic’s pitch and amplitude get modulated:

- _None_ leaves the signal unmodulated.
- _Chorus_ drives every partial with triangle wave modulation. With Mod Rate at 0, this mode modulates nothing but the amplitudes of the partials.
- _Wander_ draws on random sawtooth waveforms to modulate each partial.
- _Granular_ randomly modulates the amplitude of every partial by means of exponential decay envelopes. Its partials emerge at uneven intervals, and the Mod Rate parameter governs how dense they become.

The Mod Rate and Pch. Mod controls bear on all of the modulation modes. Mod Rate establishes the modulation rate, and Pch. Mod sets the span of pitch modulation in semitones. Even though Pch. Mod shows only a positive figure, the pitch modulation runs bipolar in every mode apart from Granular, where the grain envelopes act in a positive direction alone.

### 28.36.4 Spectrogram

Spectral Resonator’s Display with Integrated Controls.

A spectrogram is built into Spectral Resonator, charting how frequencies in the dry and wet signals behave over time. The dry signals appear in yellow and the wet ones in blue. The toggle at the display’s upper-left corner lets you tuck the spectrogram away. This visualization makes it easier to spot which parts of the spectrum the resonator is boosting or reshaping.

The spectrogram display houses two controls: Harmonics and Quantize. Harmonics lets you choose how many resonant harmonics the device employs. Larger values brighten the sound, while smaller ones darken the timbre. Note that under polyphony the harmonics are split evenly among the voices, so each voice gets fewer of them at high voice counts. Pushing the harmonics up also raises CPU usage.

With Quantize switched on, every harmonic snaps to the active scale or tuning system. When neither a scale nor a tuning system is active, the harmonics instead snap to chromatic pitches.

### 28.36.5 Global Parameters

The Global Controls in Spectral Resonator.

How much gain is applied to the processed signal is set by the Input Send control. A built-in limiter keeps the signal from clipping, and the LED beside Input Send lights up whenever that limiter kicks in.

The Unison parameter dictates how many unison voices there are, each being a detuned copy of the resonator’s partials. The Uni. Amt parameter sets how much detuning separates those voices. Adding more voices fattens the sound, while greater detuning values lend a broader, livelier character. Within the Wander and Granular modulation modes, every voice is modulated on its own, which builds particularly thick and warbly textures.

How the processed and unprocessed signals balance, and how strongly each one shows up in the spectrogram, is set by the Dry/Wet control. When Spectral Resonator sits on a return track, set Dry/Wet to 100%.

### 28.36.6 Spectral Resonator Tips

The following are a few approaches for putting Spectral Resonator to work in your projects:
