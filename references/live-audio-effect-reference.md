# Live Audio Effect Reference (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 28. Live Audio Effect Reference

Bundled with Live is an assortment of purpose-built, native audio effects. The collection spans practical workhorses — EQs, compressors, and filters — through to imaginative sound-design devices like delays, reverbs, and saturators, plus more.

For an introduction to applying effects within Live, see the [Working with Instruments and Effects](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects) chapter.

Keep in mind that the various [feature sets](https://www.ableton.com/en/live/compare-editions/) differ from one Live edition to another, so certain effects described here might be absent from particular editions.

### 28.1 Amp

The Amp Effect.

Amp is a device that recreates the tone and personality of seven vintage guitar amplifiers. Built together with Softube, Amp relies on physical modelling technology to deliver a selection of genuine, practical amp voicings, all driven by a straightforward, unified control layout.

Seven amp models are available for selection:

- _Clean_ draws on the ”Brilliant” channel of a vintage amp from the ’60s. Guitarists of the British Invasion leaned on this amp heavily.
- _Boost_ draws on the ”Tremolo” channel of that same amp, and works well for gritty rock riffs.
- _Blues_ draws on a guitar amp from the ’70s with a bright voice. Players in country, rock and blues styles favor this classic amp.
- _Rock_ takes its cues from a vintage 45 watt amp dating to the ’60s. It may well be the most recognizable rock amp ever made.
- _Lead_ draws on the ”Modern” channel of a high-gain amp favored by metal players.
- _Heavy_ draws on the ”Vintage” channel of that same amp and suits metal and grunge tones just as well.
- _Bass_ takes its cues from an uncommon PA from the ’70s that bass players embraced thanks to its powerful bottom end and ”fuzz” when pushed loud.

Even though the actual hardware versions of these amps each carry their own distinct parameters, Live’s Amp effect applies one common control set across every model. As a result, you can rapidly reshape your sound’s broad character without fiddling with countless settings.

Gain sets how hot the signal feeding the preamplifier is, whereas Volume governs the power amplifier’s output stage. Even though Gain and Volume jointly shape Amp’s total level, Gain is what mainly drives how much distortion appears. The more you raise Gain, the dirtier the tone becomes. With the Blues, Heavy and Bass models, pushing Volume high can introduce a fair bit of distortion too.

The Bass, Middle and Treble knobs serve as EQ controls that shape the tone color. Just like on actual hardware, Amp’s EQ parameters affect one another — and the rest of Amp’s parameters — in nonlinear and at times surprising ways. Boosting the EQ, for instance, may in certain situations also raise how much distortion is present.

Presence acts as a further tone control covering the mid/high range within the power amp stage. How strongly it shapes the sound shifts a good deal according to which amp model is selected, but it can introduce (or remove) ”edge” or ”crispness.”

The Output switch flips between mono and stereo (Dual) processing. Bear in mind that Amp consumes double the CPU while in Dual mode.

The Dry/Wet control sets the mix between the affected and unaffected signals.

### 28.1.1 Amp Tips

Since Amp models actual analog hardware, predicting how it behaves can occasionally be tricky. Below are a few suggestions for getting the most from Amp:

#### 28.1.1.1 Amps and Cabinets

Guitar amplifiers are meant to be paired with matching speaker cabinets. That is why Amp ships with a partner device named [Cabinet](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#cabinet), intended to sit _after_ Amp within a device chain. When authenticity is the goal, we suggest that signal flow. That said, you can also reach unusual and exotic textures by running Amp and Cabinet on their own.

#### 28.1.1.2 Electricity

The assorted circuits inside guitar amps draw on a steady, fixed supply of electricity. Because of this, boosting one parameter may unintentionally pull available power away from some other part of the amp. The EQ controls show this most clearly. Raising Treble, for example, can pull down the level of the bass and midrange. You might discover that several apparently disconnected parameters need careful tweaking before you reach the result you’re after.

#### 28.1.1.3 More than Guitars

Although Amp and Cabinet pair beautifully with guitars, feeding them drums, synthesizers or other material can yield very compelling results. As an example, route [Operator](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#operator) or [Analog](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#analog) through Amp to lend analog grit to your digital tones.

### 28.2 Auto Filter

The Auto Filter Effect.

Auto Filter is a filtering device that reshapes whatever sound arrives by running it through frequency-selective filters. It supplies an assortment of filter types plus filter circuit types modeled on vintage analog filters. Thanks to the device’s LFO modulation and envelope follower, you can build moving, tone-shaping effects. The envelope follower may react to the filtered signal on its own or to an external sidechain feed.

### 28.2.1 Filter Types

The Filter Type chooser lets you pick one of ten filters. The available choices are Low-pass, then High-pass, plus Band-pass, the Notch type, Morph, the DJ option, Comb, Resampling, Notch + LP, and lastly Vowel.

The Filter Type Chooser.

The Low-pass filter cuts back frequencies sitting above the cutoff. Use it to tame brightness or strip away high-frequency content. The slope can be toggled between 12 and 24 dB.

High-pass lets through frequencies sitting above the cutoff frequency while cutting back the lower ones. It comes in handy for stripping low-frequency rumble or making sounds thinner. The slope can be toggled between 12 and 24 dB.

The Band-pass filter passes only a narrow band of frequencies surrounding the cutoff, reducing both the lower and higher frequencies that fall outside that band. This lets you single out a slice of the spectrum or build resonant, concentrated tones. The slope can be toggled between 12 and 24 dB.

Notch cuts back a slim band of frequencies while leaving nearby frequencies mostly untouched. Reach for it to strip out particular frequencies or to produce gentle phasing-style effects. The slope can be toggled between 12 and 24 dB.

The Morph filter offers a continuous sweep from low-pass through high-pass filtering, passing through band-pass response in the middle. Four filter slopes are on offer: 6, 12, 24, and 48 dB.

The DJ filter folds low-pass and high-pass filtering together under a single bipolar control, much like the ones on certain DJ mixer. Pushing above zero removes low frequencies and lifts the highs, while going below zero strips out the highs and lifts the lows. Be aware that filter resonance shifts too: settings close to 0.0% give a slight bump of the boosted frequencies, and that bump grows steadily as the value heads toward -100% or 100%.

Comb lays down a row of peaks or notches spread over the frequency spectrum and, when modulated, can yield flanger-style effects.

The Vowel filter molds the tone toward something voice-like by accentuating particular formants.

The Resampling filter trims high-frequency content by repeatedly resampling the signal at a rate tied to the cutoff frequency, which brings about aliasing and sampling degradation.

Notch + LP merges a notch filter with a low-pass filter, so a slim band of frequencies gets reduced while high frequencies are simultaneously rolled off. The slope can be toggled between 12 and 24 dB.

You dial in the chosen filter’s cutoff frequency through the Freq control positioned above the Filter Type chooser. Note that the DJ filter omits Freq and instead supplies the Control knob, letting you glide the device smoothly from low-pass toward high-pass filtering. The Vowel filter swaps Freq for the Pitch control; with it you set how many semitones the formants are nudged upward or downward.

The majority of filter types carry a Res (Resonance) control that lets you dial in how much emphasis sits at the cutoff frequency. It does nothing for the Resampling filter type and is grayed out to signal that. The Vowel filter swaps it for the Formant control; use that to fix the spot within the vowel spectrum matching the vowels a, e, i, o, and u.

The Morph, Comb, Notch + LP, and Vowel filters add an extra Morph control whose setting governs how the chosen filter’s personality shifts over the control’s span. You can lean on it to glide smoothly among different filtering styles, with the outcome tied to the filter type:

- With the Morph filter, low Morph values give low-pass filtering, mid-range settings deliver band-pass filtering, and high values give high-pass filtering.
- With the Comb filter, you can move the filter onto either the peaks (using low Morph values) or the notches (using high Morph values) that show up at multiples of the chosen cutoff frequency.
- With the Notch + LP filter, you can shift where the notch sits in relation to the low-pass cutoff. When Morph values stay low, the notch begins further from the cutoff and creeps steadily nearer as the control’s value goes up. By 100% the notch lands right at the cutoff.
- With the Vowel filter, the Morph control lets you progressively even out the gain across the formants.

### 28.2.2 Filter Display

Sitting in the device’s center, the display draws the filter curve for the chosen filter type, the modulated filter curves for both the left and right channels, plus the live signal spectrum of the output. Dragging the handle adjusts the Freq and Res controls (or, with the Vowel filter, Pitch and Formant in turn).

The controls beneath the display split into two groups: the LFO controls and the Envelope control. Whenever a group is active, it also brings a set of parameters that appear along the bottom of the display.

Auto Filter’s Display with Envelope Parameters Visible.

### 28.2.3 LFO Controls

Auto Filter’s LFO Controls.

Auto Filter can drive the left and right channels with independent LFO modulation, letting the modulation be staggered across the stereo field. The LFO Stereo Mode toggle along the bottom of the display flips between the two stereo offset modes: Phase and Spin.

Phase holds both LFOs at one shared frequency yet can push the two LFO waveforms out of phase, producing stereo movement. You can stagger the left and right modulation channels in degrees with the LFO Phase control. At 180° the channels sit fully out of phase, so the moment one LFO hits its peak the other rests at its minimum. The Spin mode pulls the two LFO rates apart from one another by a percentage dialed in with the LFO Spin control. With Phase at 0° or Spin at 0%, the left and right channels receive identical modulation.

The LFO Phase Offset parameter lets you slide the starting position of both LFO channels along their waveforms. Bear in mind this parameter does anything only when the LFO time mode sits on tempo-synced beat divisions or sixteenth note values.

The LFO Quantization Mode chooser lets you make the modulation step rhythmically at fixed intervals (Steps) or follow the tempo (S&H). Under Steps, each LFO cycle is split into a count of intervals chosen with the LFO Steps control. Under S&H, the LFOs are quantized to the beat-time value dialed in with the LFO S&H parameter.

The LFO Amt control governs the degree to which the low frequency oscillators influence the filter. You can run the LFOs alongside the envelope follower or in place of it.

The Rate control governs the LFO frequency, expressed either in Hertz, in seconds, as tempo-synced beat divisions, or as sixteenth note values, according to whichever LFO time mode is picked through the Mode chooser. Note that with the mode on Time, the Rate control’s display name switches to “Time.”

Through the Wave chooser you pick the LFO’s waveform from this group of shapes: Sine (whose modulations stay smooth, with peaks and valleys that are rounded), then Triangle, Saw, Square, Ramp Up, then Ramp Down, Wander, plus S&H (which yields modulation values that are randomly positive and negative). Note that with Wander or S&H picked, the Spin control has no audible effect and is grayed out.

The Morph control reshapes the LFO contour. Note that once the S&H waveform is picked, this control gives way to the Smooth parameter, which lets you soften the waveform.

### 28.2.4 Envelope Follower Controls

Envelope Controls in Auto Filter.

The envelope controls let you dictate the way the envelope modulation acts on the filter frequency.

The Envelope Attack slider sitting at the foot of the display determines how the envelope reacts to incoming signals that rise. Low settings give a quick reaction to input levels, while high settings smooth out any movement over time, yielding a looser, more gradual reaction. Picture it as lending inertia to the reaction.

The Envelope Hold toggle governs the way the envelope passes from the attack into the release phase. Switched on, the envelope finishes the whole attack phase ahead of beginning the release phase.

The Envelope Release slider lets you dictate how rapidly the envelope reacts to falling input levels. Lower settings make the envelope react sooner, whereas higher settings stretch out the envelope’s decay.

You can quantize the envelope modulation to beat-time values. To turn on envelope quantization, flip on the Envelope S&H toggle and then dial the quantization value with the Envelope S&H Rate slider.

You steer both the direction and the degree to which the envelope modulation acts on the filter through the Envelope control sitting below the display.

### 28.2.5 Filter Drive and Circuits

Filter Drive and Circuit Controls.

The Drive control lets you push extra input drive into the signal ahead of the filter. This comes in handy for introducing distortion to the signal. At 0.0% the sound stays untouched, growing steadily more distorted and saturated as the Drive setting climbs.

Auto Filter’s filter circuit types capture the personality of assorted analog filter designs. With the Filter Circuit chooser, pick a type from these: SVF, DFM, MS2, and PRD. Note that the filter circuits matter only alongside the Low-pass, High-pass, Band-pass, Notch, and Morph filters.

The SVF circuit option behaves as a clean filter, yet it can also bring in distortion when Drive sits above zero.

DFM routes more of its own distortion back through itself, giving a wide span of tones reaching from gentle filter sweeps to warm drive.

The MS2 circuit relies on a Sallen-Key design plus soft clipping to keep resonance in check. It is modeled on the filters found in a renowned semi-modular Japanese monosynth.

PRD draws on a ladder design and applies no deliberate resonance limiting. It is modeled on the filters found in a legacy dual-oscillator monosynth from the United States.

### 28.2.6 Global Controls

Global Controls in Auto Filter.

The Clip toggle lets you apply soft clipping to whatever the effect outputs. This can help rein in any peaks that arise from high resonance settings. The LED beside the toggle blinks any time the signal clips.

The Output slider fixes how loud the processed signal is at the device’s output. It lets you offset jumps in loudness, which proves handy when you run high Drive settings.

Dry/Wet sets the mix between the processed and unprocessed signals.

### 28.2.7 Sidechain Parameters

Out of the box, Auto Filter draws on its own input source to drive the envelope follower. You can, however, configure the device to follow an external sidechain signal in its place. Reach the external sidechain parameters by clicking the Sidechain Section toggle at the device’s upper left corner.

Auto Filter’s Sidechain Parameters.

Flip on the External toggle to switch on the external sidechain. With it enabled, the External Source chooser lets you name the signal’s source. The External Tapping Point chooser additionally lets you decide whether the signal arrives Pre FX, Post FX, or Post Mixer.

The Mix slider lets you blend the external and internal sidechain signals together as the trigger for the envelope follower. At 100% the envelope follower follows the external sidechain source alone. At 0% only the internal sidechain comes into play.

The SC Gain control lets you set the level arriving from the external sidechain. Note that the sidechain audio merely triggers the envelope follower, so raising the gain does not raise the source signal’s volume.

To audition the sidechain signal, switch on the Sidechain Listen toggle. This overrides Auto Filter’s output and plays the sidechain input straight to your ears, which helps while you adjust sidechain parameters.

The Sidechain Listen Toggle.

The sidechain carries its own dedicated frequency-selective filter, switched on via the SC Filter toggle. Once active, Auto Filter responds solely to the frequency range fixed by the sidechain filter controls.

The Sidechain Filter Frequency control fixes the cutoff frequency of the sidechain filter. With the Type chooser, pick a filter from these: low-shelf, peak, high-shelf, low-pass, band-pass, and high-pass.

The low-shelf filter raises or lowers frequencies beneath the cutoff frequency, leaving those above largely untouched. Rather than rolling off endlessly the way a low-pass does, the response settles onto a steady gain fixed with the Shelf Gain slider. Positive settings lift the signal, while negative settings cut it.

The peak filter raises or lowers frequencies surrounding the cutoff frequency, with frequencies above and below that band increasingly less affected. The Peak Gain slider fixes the degree of boost or cut.

The high-shelf filter raises or lowers frequencies above the cutoff frequency, leaving frequencies beneath the cutoff largely untouched. As with the low-shelf filter, the response settles onto a steady gain fixed with the Shelf Gain slider rather than rolling off without end.

The low-pass filter cuts back frequencies above the cutoff. High-pass lets through frequencies sitting above the cutoff frequency while cutting back the lower ones. Notch cuts back a slim band of frequencies while leaving nearby frequencies mostly untouched. The Sidechain Filter Q slider lets you fix the filter’s bandwidth.

#### 28.2.7.1 Mono Sidechain

Out of the box, the sidechain signal is folded down to mono, and the envelope follower modulation matches across the left and right channels. The Mono Sidechain option can be switched off from the device’s context menu.

### 28.3 Auto Pan-Tremolo

The Auto Pan-Tremolo Effect.

Auto Pan-Tremolo applies LFO modulation to the incoming signal’s stereo position or amplitude in order to build automatic panning, tremolo, and gating effects.

Two modes exist: _Panning_ and _Tremolo_. Under Panning mode, a pair of LFOs shift where the input signal sits across the stereo panorama by trading its amplitude back and forth between the left and right channels. Under Tremolo mode, one LFO varies the signal’s amplitude to produce changes in volume. Flip between the modes with their respective toggles. The LFO waveform along with the controls in the display refresh to match whichever mode is active and mirror its corresponding properties.

The Effect Can Be Used in Panning Mode or Tremolo Mode.

Below the LFO waveform, the live visualization displays the present stereo position under Panning mode or the present amplitude level under Tremolo mode. This lets you tell at a glance how the input signal travels across the left and right channels or how its amplitude rises and falls.

Through the Waveform drop-down, choose the LFO contour you want. On offer are Sine, then Triangle, Shark Tooth, Saw Up, plus Saw Down, the Square shape, Random, Wander, and finally S&H (Sample and Hold).

Choose one of the offered Time modes to fix the LFO’s rate: Rate, Time, Synced, Dotted, Triplet, or 16th. After you pick one, the matching modulation rate control beneath the drop-down refreshes to show the value linked to that mode. Under Time mode, for instance, the LFO’s period can be set anywhere between 100 milliseconds and 200 seconds, handy for building lengthy modulation cycles.

You can pick from two Stereo Offset modes: _Phase_ and _Spin_. Under Phase mode, each LFO waveform driving the left channel and the right one may be staggered by a chosen number of degrees. At 180° the LFOs sit fully out of phase, so that as one LFO arrives at its peak value the other rests at its minimum. Under Spin mode, the left and right channels drift apart steadily according to the chosen percentage. This introduces a gentle asymmetry across the two channels. Note that only Phase mode is on offer with the Random, Wander, and S&H waveforms.

With any of the beat-division-based Time modes active (Synced, Triplet, Dotted, or 16th), the Phase Offset control turns available and lets you slide where each LFO channel begins inside its cycle relative to the beat grid. This proves handy for nudging the modulation so it kicks in slightly ahead of or behind the beat.

With the Random, Wander, or S&H waveforms in use, Phase Offset behaves as a stereo width control and can be used to add variation across the channels.

The Invert toggle flips the LFO’s polarity. Switched on, the waveform’s positive and negative values are swapped, which in effect flips the waveform upside down. Under Panning mode, for example, inverting the Saw Up waveform yields a Saw Down waveform. Under Tremolo mode, the waveform’s peaks turn into valleys and the reverse. With ramp-shaped waveforms, switching Invert on yields a ducking effect, while leaving it off yields a gating effect.

Tremolo mode brings two extra options you can switch on to shape how the LFO modulation behaves: _Harmonic_ and _Vintage_.

The Harmonic and Vintage Tremolo Mode Toggles.

When Harmonic is on, the high and low frequencies get modulated in an alternating fashion instead of together. A set crossover at 600 Hz divides the signal into a pair of frequency bands.

When Vintage is on, the LFO varies the signal’s amplitude and a non-linear curve also shapes it, lending warmth and grit to the tremolo effect.

Beneath the display sit controls that adjust the LFO’s amount, rate, shape, attack, and reaction to the input signal’s level.

Use the Controls Below the Display to Adjust the LFO Modulation.

With the Amount control you set how strongly LFO modulation is applied to the arriving signal.

The control sitting to the right of the Amount control fixes the LFO rate. That control’s name and unit shift according to the chosen Time mode. As an example, it shows up as _Freq_ when Rate is picked and the value reads in hertz (Hz). Under Time mode it shows up as _Time_ with the value in milliseconds (ms). Under the Synced, Triplet, Dotted, and 16th modes it shows up as _Rate_ with the value in beat divisions.

Note that the Amount control’s value and the LFO rate are shared across the Panning and Tremolo modes and can’t be set on their own.

The Shape control molds the LFO waveform in a different way for each mode. Under Panning mode, positive Shape values drive each waveform toward its upper and lower extremes. This trims the overlap between the LFOs, so the handoff from one channel to the next grows more abrupt. Under Tremolo mode, positive values steadily round out the waveform into rounded peaks, while negative values steadily squeeze the peaks into an angular form. Pushed to its highest or lowest setting, the Shape control can form ramps that yield gating effects (when Invert is off) along with pumping effects (when Invert is on).

Use the Shape Control to Create Ramps for Gating and Ducking Effects.
