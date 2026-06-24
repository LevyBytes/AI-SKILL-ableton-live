# Live Audio Effect Reference (part 10)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

- Build pitched drum patterns by dropping Spectral Resonator onto a percussion track and feeding the MIDI sidechain input to push chosen notes. The result lets percussion carry a melodic role, so the kit lines up harmonically with parts like the bassline.
- To make Spectral Resonator chase a melody line, start by turning audio into MIDI through [Convert Harmony to New MIDI Track](https://www.ableton.com/en/live-manual/12/converting-audio-to-midi/#convert-harmony-to-new-midi-track) or [Convert Melody to New MIDI Track](https://www.ableton.com/en/live-manual/12/converting-audio-to-midi/#convert-melody-to-new-midi-track), and then send that resulting MIDI track into the device.
- For a reverb-style tail, dial Freq down low, push the Unison and Uni. Amt amounts up, and pick the Wander modulation mode together with gentle Mod Rate and Pch. Mod settings. Use the Decay parameter to shape how long that “reverb” lingers.
- Treat Spectral Resonator as a vocoder by inserting it on a vocal track and driving it through the MIDI sidechain input.
- Stack harmonic content by chaining two Spectral Resonators one after another and feeding each a separate MIDI part, which yields layered resonant textures.

### 28.37 Spectral Time

The Spectral Time Effect.

Spectral Time merges time-freezing with spectral delay inside one creatively rich device. Incoming material can be resynthesized by running it through assorted spectral filters, delays, and frequency-shifting tricks, which spawns wildly varied, distinctive copies. Because the freeze and delay stages run either jointly or on their own, the range of outcomes is broad — you might hold a sound forever, or pair delays with tempo-locked fade transitions. Smearing frequencies across time reshapes sounds with ease, and you can layer metallic echoes plus ambience onto any source.

The device splits into two principal stages, Freezer and Delay, usable separately or chained, where the freezer feeds into the delay. Switch each stage on or off with the Freezer On and Delay On buttons.

A spectrogram in Spectral Time visualizes how the dry and wet signal frequencies evolve across time. The dry signal appears in yellow and the wet signal in blue. Clicking its toggle button hides this display.

Within Spectral Time’s context menu sits a Zero Dry Signal Latency switch. Turning it on drops the dry signal’s latency all the way to zero rather than matching it to the effect’s output timing. It comes in handy when you route a live instrument through Spectral Time and listen to the result.

### 28.37.1 Freezer Section

Spectral Time’s Freezer Section.

Whichever of the Manual/Retrigger Mode buttons is engaged governs how the Freezer section fires the freeze and which timing traits of the captured audio get shaped. Keep in mind that, in either mode, the Freeze button must also be engaged for anything to happen.

Under Manual mode, a click on the Freeze button captures the audio. The Fade In and Fade Out duration of that captured signal is also adjustable in milliseconds.

Retrigger mode hands you extra controls for tightening the timing of the frozen audio, which it can capture on its own at each transient (onset) or on a steady schedule.

With Onsets mode, the audio freezes once a transient shows up in the signal. Tune how readily onsets are caught using the Sensitivity knob — it peaks at 100% and bottoms out at 0%.

Sync mode captures the audio on a steady schedule governed by the Interval control. Flipping the Freezer Time Unit buttons lets the Interval control read in either milliseconds or beat-time values.

Across both Onsets and Sync modes, the Freezer Fade Shape buttons switch among two fade shapes on offer: Crossfade and Envelope. Each shape carries its own controls dictating how a fresh freeze fades in and back out.

With the Crossfade shape chosen, the incoming freeze rises while the previous freeze (or dry signal) drops away. Its length comes from the X-Fade control, which precisely sets the time in milliseconds during which a new freeze rises, expressed as a portion of the sync interval defined by the Interval control.

With the Envelope shape chosen, a fresh freeze fades up and down following the millisecond durations entered in the Fade In and Fade Out parameters. Here, as many as eight freezes can pile up simultaneously, one over the next.

### 28.37.2 Delay Section

Spectral Time’s Delay Section.

Spectral Time’s Delay section switches on or off via the Delay toggle button and lets you spawn delayed copies of the spectral data. Whenever the Freezer section is running, the Freezer’s output feeds straight into the Delay section.

How long the spectral delay lines wait is governed by the Time parameter. Which kind of value appears depends on the unit type picked in the “Mode” drop-down chooser:

- Time mode adjusts the delay time in milliseconds.
- Notes adjusts delay time in beat divisions.
- 16th, 16th Triplet, and 16th Dotted peg the delay to a count of whichever 16th notes variety you picked.

Feedback governs how much of the output returns to the delay input. Raising it makes the signal’s echoes more pronounced.

Shift moves the frequency of the delayed copies. Every following delay gets nudged higher or lower by the chosen frequency amount.

Stereo scales the spread of the Tilt and Spray controls.

Balance between the dry and delayed signals is handled by the Dry/Wet control. Bear in mind it touches only the device’s Delay section.

Tilt tilts the delay timing across frequencies. A positive setting holds high frequencies back more than low ones, whereas a negative setting holds low frequencies back more than high ones.

Spray scatters the delay timing for various frequencies at random inside the supplied time span.

Mask confines the reach of the Tilt and Spray controls to either the high or the low end. Positive settings restrict the action to high frequencies, and negative settings restrict it to low frequencies.

### 28.37.3 Resolution Section

Spectral Time’s Resolution Control.

Tucked into the spectrogram display’s top-right corner is the Resolution control, which dictates the resolution applied when processing the incoming signal. Dropping it down trims total latency but sacrifices precision and fidelity. Because raising it adds to overall latency, lowering the Resolution while tracking is often worthwhile.

### 28.37.4 Global Controls

Spectral Time’s Global Controls.

Input Send trims the gain of the signal coming in.

A pair of radio buttons, Frz > Dly and Dly > Frz, flip the order in which the effects run.

The overall Dry/Wet control balances the dry signal against the processed one. Push it to 100% whenever Spectral Time sits on a return track.

### 28.38 Spectrum

The Spectrum Device.

Spectrum carries out live frequency analysis on the audio arriving at it. Its findings appear as a graph, dB running up the vertical axis and frequency/pitch running across the horizontal. Peak readings stay drawn on the graph until you restart the song. Keep in mind that Spectrum is a measurement tool rather than an audio effect — it leaves the incoming signal untouched.

How many samples get examined per measurement is governed by the Block chooser. Larger settings sharpen accuracy while loading the CPU more heavily.

Channel picks which channel gets analyzed — left, right, or both.

How frequently Spectrum runs an analysis comes from the Refresh slider. Like the Block parameter, it trades accuracy against CPU load. Quicker response brings more accuracy yet leans harder on the CPU.

With the Avg slider you state how many sample blocks get averaged for every display refresh. At a value of one, every block appears on its own. That makes the display far busier, which helps when hunting down the spectrum of brief peaks. Raising the Avg value smooths the refresh, showing the spectrum averaged over time, which lines up better with how our ears truly perceive sound.

The Graph button flips the spectrum between a single interpolated line and separate frequency bins.

Max turns the readout of the running peak amplitude on or off. While Max is active, a click in the display clears the stored maximum amplitude.

Using the Scale X buttons you can swap the frequency display’s scaling among linear, logarithmic, and semitone. Note that logarithmic and semitone share the same scaling and merely change the legending at the display’s top from Hertz to note names. Linear scaling shines when you analyze high frequencies in detail.

Hovering your pointer across Spectrum’s display brings up a box reporting the amplitude, frequency, and note name beneath the cursor. At the lower left of Spectrum’s interface, the Range/Auto button swaps between adjusting the display’s dynamic range by hand or automatically. Under Range, you zoom and scroll the amplitude by moving over the amplitude legending along the display’s left edge — drag up and down to scroll, side to side to zoom. The Range sliders likewise let you fix the lowest and highest amplitude values on view. Under Auto, the display rescales itself in response to the incoming audio level. Note that the Range sliders and zooming go inactive while Auto is engaged.

For a still clearer look, swap where the display sits — the device chain or Live’s main window — by clicking the button on Spectrum’s title bar, or simply double-click inside the display.

### 28.39 Tuner

The Tuner Device.

Tuner reads out the arriving monophonic pitch together with how far it sits from the closest semitone. Modeled on traditional guitar tuners, its oversized display reads easily from across a stage and excels at tuning outboard instruments or synthesizers.

Bear in mind that Tuner serves as a measurement tool, not an audio effect – the incoming signal passes through unchanged. It is built to read monophonic pitches and performs best on a tidy, well-defined signal. Polyphonic, noisy, or harmonically dense input can throw off its readings.

### 28.39.1 View Switches

A pair of buttons at the lower-left flip Tuner among its two primary views. Classic View mimics familiar analog tuners, whereas Histogram View charts pitch across time. Color cues in the display signal tuning accuracy in either view: green for in tune, red for out of tune.

Tuner’s View Switches.

### 28.39.2 Classic View

Within Classic View, a colored ball riding along a curve stands in for the arriving pitch, and the closest matched note name sits at the display’s middle. Arrows flanking that note name illuminate to show whether the signal should rise or fall to land on the target pitch.

Under Target Mode, a ring drawn at the curve’s center marks the goal pitch, and you are in tune once the colored ball rests precisely inside that ring. A sharp input pushes the ball to the right of the target, while a flat input shifts it to the left.

Tuner in Target Mode.

Under Strobe Mode, the curve turns into a spinning band of lights. Which way it spins tells you whether the pitch runs sharp or flat. Rightward rotation marks a sharp input, and flat input sends the band spinning leftward. The farther off your pitch is, the faster the band travels.

Tuner in Strobe Mode.

The Hertz/Cents Switch flips between reporting the incoming signal’s outright frequency in Hertz and its gap from the target pitch in cents. You will also find this switch in the Histogram View.

### 28.39.3 Histogram View

Histogram View plots pitch as it unfolds over time. A scale along the display’s right edge lists the available note names, and the horizontal gray bars mark each note’s flawlessly in-tune “center.” A sharp note sits above its matching gray line, and a flat note drops below it.

Tuner in Histogram View.

Dragging up or down inside the display scrolls through pitches, and dragging side to side zooms in or out. When Auto is on, the display realigns itself so the arriving pitch stays centered.

The Hertz/Cents Switch flips between reporting the incoming signal’s outright frequency in Hertz and its gap from the target pitch in cents. You will also find this switch in the Classic View.

### 28.39.4 Note Spellings

Tuner’s Note Spellings.

Three note-spelling choices ship with the Tuner device. Right-clicking anywhere inside Tuner’s view display opens a menu holding them:

- Sharps (C#)
- Flats (D♭)
- Sharps and Flats (C#/D♭)

### 28.39.5 Reference Slider

Tuner’s Reference Slider.

With the Reference slider you reset the tuning reference Tuner relies on while reading incoming signals. It sits at 440 Hz by default, the “standard” concert pitch, yet you can move it to any figure within 410-480 Hz.

### 28.40 Utility

The Utility Effect.

Utility handles a number of genuinely handy chores, particularly when paired with other devices.

It carries two independent Phase controls, one per input channel (Left and Right). True to their labels, each one flips the phase of its channel.

Selective handling of a sample’s left and right channels comes from the Channel Mode chooser. Pick Left, for instance, and the right channel is dropped while the left channel feeds both outputs. That helps a great deal when a stereo file holds distinct content on each channel and you only want one of them.

How wide the wet signal spreads is set by the Width control. At 0% you get a mono signal, while figures past 100% push the stereo image wider.

Picking Mid/Side Mode from the Width control’s context menu lets you flip between the Width and Mid/Side controls. Across 0 to 100M, the Mid/Side control behaves as a smooth mono-to-stereo dial. Pushing it to 100M collapses the audio to mono. Settings from 0 up to 100S play up a signal’s stereo or “out of phase” content. At 100S you hear the side signal alone, with the left and right channels sitting 180 degrees out of phase from each other.

Bear in mind that picking either Left or Right in the Channel Mode chooser leaves the Width and Mid/Side controls inactive and grayed out.

Switching on the Mono control folds the stereo input down to mono.

The Bass Mono switch collapses the input’s low frequencies to mono, which keeps low end from coloring oddly when it plays back in mono. The Bass Mono Frequency slider sets that crossover point anywhere from 50-500 Hz.

Turning on Bass Mono Audition leaves only the low frequencies audible, which helps when you dial in the Bass Mono Frequency.

Level of the incoming signal is shaped by the Gain control, spanning -infinite dB to +35 dB. It is handy for automating volume fades on a track while leaving that track’s Volume control open for mix work. Nudging the Gain parameter between -18 and +35 dB with the up and down arrow keys moves it in 1 dB steps; from -18 dB down toward -inf dB, though, the value ramps with a smooth acceleration.

The Balance control places the signal anywhere across the stereo field.

Engaging the Mute button just quiets the arriving signal. A track’s active/mute controls always sit at the very tail of its signal chain. Yet because Utility can go anywhere in a chain, its mute can choke the feed into a delay line or reverb without shutting down those devices’ output tails.

The DC switch strips away DC offsets and ultra-low frequencies sitting well beneath what we can hear. It only changes the sound when a signal actually carries those frequencies and gets hit, after Utility, by nonlinear processing such as compressors or waveshapers.

### 28.41 Vinyl Distortion

The Vinyl Distortion Effect.

Vinyl Distortion recreates several of the characteristic distortions that crop up while a vinyl record plays back. They stem from the geometric interplay of the stylus and the cut groove. A crackle generator is built in as well, layering noisy artifacts on top.

Even harmonic distortion gets added to the input by the Tracing Model section. Set how much with the Drive knob, or click and drag up and down inside the Tracing Model X-Y display. To shift the distortion’s frequency or ”color,” drag sideways in the X-Y display, or double-click the Freq field and key in a number. Holding Alt (Win) / Option (Mac) while you drag vertically in the X-Y display alters the frequency band’s Q (bandwidth).

Odd harmonics get added to the input by the Pinch Effect section. Such distortions usually land 180 degrees out of phase, which fattens the stereo image. Its controls mirror the Tracing Model’s, yet it puts out a noticeably different tone.

The Drive control raises or lowers the total distortion coming from both the Tracing Model and Pinch.

Two distortion modes are on offer: Soft and Hard. Soft Mode evokes the tone of a dub plate, whereas Hard Mode leans nearer to a typical vinyl pressing.

Whether the Pinch distortion runs in stereo or mono rides on the stereo/mono switch. Leave it on stereo for a lifelike take on vinyl distortion.

The Crackle section seeds the signal with noise, its thickness governed by the Density control. The Volume control dials how much gain hits that noise.

### 28.42 Vocoder

The Vocoder Effect.

(Note: You won't find the Vocoder effect in the Intro and Lite Editions.)

A vocoder is an effect that fuses the frequency content of one audio signal (the _carrier_) with the amplitude shape of a second audio signal (the _modulator_). The modulator usually carries a distinct rhythmic feel, such as speech or drums, while the carrier is most often a harmonically dense synth tone like a string or pad. People reach for a vocoder most commonly to conjure ”talking synthesizer” or robotic voice sounds.

A vocoder operates by passing both the carrier and the modulator through banks of band-pass filters. It then reads the output level from each of the modulator’s filters and uses that to drive the volume of the matching carrier filter.

Place Live’s Vocoder on whichever track holds the audio you intend to serve as the modulator. From there, the Carrier chooser offers several possibilities for the carrier signal:

- _Noise_ draws on Vocoder’s built-in noise generator for the carrier. Choosing it brings up an X-Y display for shaping the noise’s character. Its horizontal axis tunes downsampling — drag leftward to lower the sample rate of the carrier’s output. Its vertical axis tunes the noise density — drag downward to thin it out.
- _External_ lets you tap any of the internal routing points available in the choosers underneath. This is the pick for the classic ”robot voice” sound.
- _Modulator_ feeds the modulator back in as the carrier. In effect it puts out a resynthesized take on the modulator signal, while still letting Vocoder’s sound-shaping controls reshape the tone.
- _Pitch Tracking_ turns on a monophonic oscillator that tunes itself to the modulator’s pitch. With the High and Low sliders you can hem in the frequency span the oscillator tries to follow. Pick sawtooth or one of three pulse waveforms and set the oscillator’s coarse tuning through the Pitch slider. Pitch tracking works especially well on monophonic modulators like melodic instruments or voices. Keep in mind the oscillator refreshes its frequency only on detecting a definite pitch, after which it holds that pitch until a fresh one arrives. So tweaking the oscillator’s parameters or forcing it to reset (say, when [grouping](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks) Vocoder’s track) may produce surprising shifts in the sound. On polyphonic material or drums, pitch tracking is mostly unpredictable (though it can be quite intriguing.)

Especially with external carrier sources, a vocoder’s output may shed a good deal of high end. Switching on the Enhance button brightens the tone by evening out the carrier’s spectrum and dynamics.

The Unvoiced knob sets the level of an extra noise generator, which rebuilds the pitchless parts of the modulator, such as ”f” and ”s” sounds.

Sens. governs how readily the unvoiced detector fires. At 100% the unvoiced noise generator stays on the whole time; at 0% only the primary carrier source plays. The Fast/Slow switch sets how rapidly Vocoder flips between unvoiced and voiced detection.

The wide central panel of Vocoder displays the levels of each band-pass filter. A click inside this panel lets you pull those levels down.

How many filters are in play comes from the Bands chooser. More bands sharpen the read on the modulator’s frequency content while drawing more CPU.

The Range sliders set the frequency span the band-pass filters cover. A reasonably wide span suits most sources, though you may want to trim the outer edges if the sound turns too shrill or boomy. The BW control fixes the filters’ bandwidth. At low percentages each filter narrows toward a single frequency; widening the bandwidth makes the filter bands overlap more. A bandwidth of 100% is the truest, yet figures above or below it can yield intriguing results.

The Precise/Retro switch flips between two filter behaviors. Under Precise mode every filter shares one gain and bandwidth. Under Retro mode the bands grow tighter and louder as frequency rises.

Gate fixes a threshold for the filterbank. Any band sitting under that threshold falls silent.

The Level slider lifts or trims Vocoder’s output.

Depth controls how much of the modulator’s amplitude envelope lands on the carrier signal. At 0% that envelope is thrown away; at 200% only the loud peaks come through; 100% gives ”classic” vocoding.

The Attack and Release controls govern how fast Vocoder reacts to amplitude swings in the modulator. Very quick settings hold onto the modulator’s transients but may breed distortion artifacts.

The Mono/Stereo switches set how many channels serve the carrier and modulator. Under Mono mode both carrier and modulator count as mono sources. Stereo keeps the modulator mono but runs the carrier in stereo. L/R runs both carrier and modulator in stereo.

The carrier filterbank’s frequencies can slide up or down through the Formant knob. With a voice as the modulator, slight Formant moves can shift the perceived gender of the source.

The Dry/Wet control balances the dry signal against the processed one.

### 28.42.1 Vocoder Tips

This part walks through configuring the most frequent Vocoder use cases.

#### 28.42.1.1 Singing Synthesizer

The textbook vocoder use case is the ”singing synthesizer.” To build one in Live:
