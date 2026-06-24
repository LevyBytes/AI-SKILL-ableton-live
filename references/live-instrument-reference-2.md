# Live Instrument Reference (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Beside the Noise button sits a drop-down listing the noise filter types on offer. The available picks are LP, HP, BP, and LP+HP. To shape cutoff and resonance, turn the Freq knob and move the Res slider.

When BP is active, the Res slider works on resonance; under LP+HP it instead governs bandwidth. Filter frequency responds to modulation too — from note pitch, from velocity, or from the envelope generator — routed through the Key and Vel sliders on the MIDI tab or through the Env Amt knob.

Output level for the entire Noise section comes from Volume, which pitch and velocity can drive through the Key and Vel sliders found on the MIDI tab.

A conventional ADSR envelope generator — covering attack, decay, sustain, and release stages — is governed by the Env Amt knob.

How rapidly Noise climbs to its peak loudness is dialed in with the A (Attack) slider; the span needed for the envelope to settle at the sustain level once the attack stage finishes is dialed in with the D (Decay) slider.

Where the envelope holds from the close of decay until the key lifts is determined by the S (Sustain) slider. A setting of 0 removes any sustain stage entirely. A setting of 100 removes the decay stage instead.

The R (Release) slider, lastly, governs release time — the span the envelope needs to fall back to zero once you let go of the key.

Center or cut-off frequency for the filter is established by the Freq knob. Across the LP, HP, and BP filters the Res slider controls resonance at that frequency, and for the LP+HP filter it instead sets its width.

### 30.2.4 Resonator Tabs

Collision’s Resonators.

What gives Collision most of its personality are the controls living in its pair of Resonator tabs. A switch inside each tab flips that resonator on or off. Be aware that switching both resonators off yields silence.

Up at the head of the Resonator tab there is a Resonance Type drop-down listing resonant objects:

- Beam reproduces how beams made of assorted materials and sizes resonate.
- Marimba is a tailored offshoot of the Beam model that captures how marimba bar overtones are tuned — a quality stemming from the bars’ pronounced arch-cut underside.
- String mimics the tone of strings built from assorted materials and sizes.
- Membrane represents a rectangular membrane — a drum head, say — whose dimensions and build can be varied.
- Plate emulates the sound made by a rectangular plate, that is a flat sheet, across assorted materials and sizes.
- Pipe represents a cylindrical tube left fully open on one side with an adjustable aperture on the other (set through the Opening parameter.)
- Tube represents a cylindrical tube sealed at each end.

Picking an object places a depiction of it onto the X-Y Controller display.

Beside the Resonance Type drop-down lies a Quality menu offering settings from Eco through to High. By cutting how many overtones get computed, Quality balances resonator fidelity against CPU load. Choosing Eco keeps CPU demand low, whereas High yields richer resonances. Bear in mind that no Quality menu appears for the Pipe or Tube resonators.

A copy button sits inside each resonator (labeled 1 → 2 within Resonator 1 and 2 → 1 within Resonator 2), letting you transfer every setting from one resonator over to its counterpart.

With the X-Y Controller, dragging the mouse left-to-right alters the resonant object’s decay time, and dragging up-and-down alters the Material/Radius parameter.

Internal damping inside the resonator is what decay time governs, and the Decay slider provides another way to set it.

How damping varies from one frequency to the next is set by the Material slider. With lower settings, the low-frequency content fades more gradually than the high-frequency content (the behavior of wood, rubber, or nylon objects). With higher settings, it is the high-frequency content that lingers longer (the behavior of glass or metal objects).

For the Pipe and Tube resonators, a Radius parameter takes the slot the Material parameter would otherwise hold. That slider governs how wide the pipe or tube is. A growing radius lengthens both the decay time and the high-frequency sustain. Push the size very large and the resonator’s fundamental pitch shifts as well.

Note pitch and velocity can drive the Decay and Material/Radius parameters by way of the Key and Vel sliders on the MIDI tab.

For the Membrane and Plate resonators only, a Ratio parameter appears that controls how the object’s dimensions compare along its x and y axes.

How loud the various frequency components are is governed by the Brightness control. Crank it up and the upper frequencies grow louder. The Pipe and Tube resonators ignore this parameter.

Pitch of the resonator’s harmonics is shifted by the Inharm knob. Drive it negative and the frequencies bunch together, swelling the count of lower partials. Drive it positive and the frequencies spread apart, swelling the count of upper partials. Velocity, via the MIDI tab slider, can also drive Inharm. Bear in mind the Pipe and Tube resonators ignore this parameter.

Found only on the Pipe resonator, Opening interpolates between a closed and an open pipe. Set to 0%, one side stays sealed; set to 100%, both ends are open. Velocity on the MIDI tab can drive this parameter too.

Where along the resonator the object gets struck or otherwise set in motion is governed by the Hit slider. Set to 0%, the strike lands dead center. Larger settings shift the strike point toward the edge. Raising the Rnd slider can also scatter the Hit position randomly. Bear in mind the Pipe and Tube resonators ignore this parameter.

How far MIDI Note Off messages silence the resonance is governed by Note Off. Set to 0%, Note Offs go unheeded and decay time follows only the Decay parameter. That mirrors how genuine mallet instruments — marimbas and glockenspiels among them — actually behave. Set to 100%, the resonance cuts off the instant a Note Off arrives, no matter the Decay time.

Where on the left and right resonator the vibrations get picked up is governed by the Pos. L and Pos. R sliders. Set to 0%, the resonance is read at the object’s center. Larger settings shift the pickup point toward the edge. Neither applies to the Pipe or Tube resonators, whose reading is always taken at the midpoint of their permanently open end.

#### 30.2.4.1 Tuning Section

Resonator Tuning Parameters.

Coarse and fine tuning are handled respectively by the Tune knob and Fine slider. Tune steps in semitones either direction, while Fine works in one-cent steps (reaching at most a quarter tone, or 50 cents, in either direction).

The Key slider on the MIDI tab can also drive the Tune knob. That Key slider governs how strongly shifts in MIDI note pitch retune the resonator. Its 100% default keeps the resonator on a standard equal-tempered scale. Raise it to 200% and each keyboard semitone produces a whole-step tuning shift. Push it negative and the resonator falls in pitch as you ascend the keyboard.

A ramp that sweeps the resonator’s pitch across time is supplied by the Pitch Envelope parameters (Pitch Env and Time). Pitch Env fixes the initial pitch and Time controls how long the glide to the destination pitch lasts. Velocity, by way of the matching Vel slider on the MIDI tab, can drive that initial pitch.

#### 30.2.4.2 Mixer Section

Resonator Mixer.

A dedicated Gain and Pan control belongs to each resonator. Note pitch, through the Key slider on the MIDI tab, can also drive Pan.

A share of the unprocessed oscillator signal is blended in alongside the resonated signal by the Bleed control. Turn it up and more of that raw signal comes through. It comes in handy for bringing back high frequencies, which low tuning or quality settings tend to dampen.

Output level for the chosen resonator is set by Gain.

### 30.2.5 LFO Tab

Collision’s LFOs.

Serving as modulators for an array of mallet, noise, and resonator parameters — picked in the Destination choosers — are Collision’s two standalone LFOs. They are also able to modulate one another.

Flipping each LFO on or off are the LFO 1 and LFO 2 switches, with the wave shape itself picked through the waveform chooser. On offer are sine, square, triangle, sawtooth up, sawtooth down and a couple of noise variants. One noise variant jumps between random levels; the other glides smoothly between them.

Phase offset for the LFO is set by the Offs. slider. With Retrigger active, playing a note relaunches the LFO at the waveform phase fixed by the Offset parameter.

Two targets per LFO can be modulated, each chosen in the Destination choosers. How intense each modulation is gets set with the LFO Destination Amount sliders. Bear in mind these depths are scaled relative to the LFO’s own Amount value.

Speed of the LFO is governed by Rate, expressed either in Hertz or as tempo-synced beat divisions. Overall LFO intensity comes from the Amount knob. On the MIDI tab, note pitch can drive Rate and velocity can drive Amount.

### 30.2.6 MIDI/MPE Tab

Collision’s MIDI/MPE Tab.

A broad set of internal MIDI assignments is opened up by the MIDI/MPE tab, serving both ordinary and MPE-capable MIDI controllers. The pitch bend (per-note pitch bend included), modulation wheel, pressure, and slide from a MIDI controller can each feed two destinations, with separate depths fixed by the Amount sliders.

Pitch or velocity, by way of the Key and Vel sliders, can drive further mallet, noise, resonator, and LFO parameters.

#### 30.2.6.1 The Global Section

Collision’s Global Section.

Parameters tied to how Collision behaves and performs as a whole live in the global section.

How many notes are allowed to ring at once is set by the Voices drop-down.

With Retrig. enabled, a note already sounding is retriggered instead of spawning one more voice. Doing so can conserve CPU.

How signal travels among the resonators is decided by Structure.

Under serial routing 1 > 2, both resonators feed Resonator 1. That output is then summed to mono and passed along to Resonator 2, while also reaching its own mixer (kept in stereo).

Resonators in 1 > 2 (Serial) Configuration.

Under parallel routing 1 + 2, the combined output of the Mallet and Noise sections goes straight to each resonator.

Resonators in 1 + 2 (Parallel) Configuration.

Overall output level is set by Volume.

### 30.2.7 Sound Design Tips

Even though Collision was built to emulate how real-world objects behave, keep in mind that these emulations permit far greater latitude than the physical originals ever could. Collision is capable of strikingly lifelike renderings of standard mallet instruments — marimbas, vibraphones, and glockenspiels — yet it is equally simple to “misuse“ its controls to conjure tones no acoustic instrument could ever yield.

When aiming for lifelike instrument emulations, it pays to picture the sequence of happenings that creates a sound on a mallet instrument (take a marimba), then map each happening onto a corresponding part of Collision:

- A striker (Mallet) makes contact with a pitched bar (Resonator 1).
- That bar’s resonance gets boosted through a resonating tube (Resonator 2).

So the standard arrangement pairs the Mallet Exciter with the two resonators wired serially (1 > 2).

And naturally, when chasing _unrealistic_ tones, all bets are off:

- Reach for the Noise Exciter, especially alongside drawn-out envelopes, to build washy, near-granular textures. The same controls can mimic unusual acoustic phenomena such as bowed vibraphones or singing crystal glasses.
- Try wiring the resonators in the parallel (1 + 2) arrangement.
- Bring in the LFOs and MIDI controllers (MPE-capable ones included) to drive Collision’s controls.

_A word of caution_: in numerous respects Collision’s models are idealized stand-ins for real objects. As a result, it is all too simple to dial in resonances far touchier to input than any real-world resonator. Some parameter pairings can trigger sharp swings in loudness. Keep output low while you audition fresh sounds.

### 30.3 Drift

The Drift Instrument.

Fully MPE-capable, Drift is an adaptable synthesizer pairing approachable controls with a clean layout. Resting on subtractive synthesis, Drift was deliberately engineered for fast, painless sound design at a light CPU cost.

Six principal sections make up Drift’s layout: an oscillator block, a dynamic filter block, an envelopes block, a pair of modulation blocks (LFO and Mod), and a block of global controls.

### 30.3.1 Subtractive Synthesis

The subtractive-synthesis approach typically opens with a waveform, then carves the source timbres into fresh shapes using filters. On top of that workflow, Drift supplies plentiful modulation choices for further tweaking and personalizing the sound, making it simple to conjure a broad palette of tones. Drift’s namesake control introduces pitch and frequency wobble per voice, lending the tone a faintly detuned, shifting pulse.

### 30.3.2 Oscillator Section

Drift’s Oscillator Section.

Drift’s Oscillator section is assembled from a noise generator, an oscillator mixer, a waveform display, controls for pitch modulation, and a pair of independent oscillators.

#### 30.3.2.1 Oscillator 1

Several hand-picked waveforms are available from the Osc 1 drop-down: Sine, Triangle, Shark Tooth, Saturated, Saw, Pulse, and Rectangle. Drift alone carries the Shark Tooth and Saturated waveforms; Shark Tooth draws on a vintage Moog analog shape of that name, while Saturated suits bass tones nicely.

Oscillator 1 is shifted by octaves with the Oct knob. Reach for the Shape knob to nudge the waveform’s harmonic makeup into something subtly altered, giving an outcome akin to pulse-width modulation. Because each waveform’s timbre differs, every one reacts in its own way to the Shape control. While you adjust it, the outcome shows up in the Waveform Display down at the foot of the Oscillator section. The waveform visibly morphs as you alter the Shape value.

Just past the Shape knob, the Oscillator 1 Shape Mod Source drop-down picks a modulation source to act on the Shape control, letting you reshape the waveform further:

- Env 1
- Env 2/Cyc - Either Envelope 2 or the Cycling Envelope serves as the modulator, whichever happens to be switched on.
- LFO
- Key - With the Shape Mod Amount on the positive side, taller note pitches yield greater modulation and lower ones yield less, and the relationship reverses once the amount goes negative.
- Velocity - Arriving velocity feeds the modulation; stronger note velocities yield greater modulation and weaker velocities yield less.
- Modwheel
- Pressure
- Slide

Modulation depth anywhere from -100% to 100% is dialed in using the Oscillator 1 Shape Mod Amount slider. Keep in mind that Shape Mod is able to add waveform modulation on its own at settings of 1% - 100%, even while the Shape control itself stays at 0%.

#### 30.3.2.2 Oscillator 2

Through the Osc 2 drop-down, you pick a waveform for the second oscillator from Sine, Triangle, Saturated, Saw, and Rectangle.

Oscillator 2 is shifted by octaves with the Oct knob, whereas the Detune control shifts it in semitones.

#### 30.3.2.3 Pitch Mod

A pair of modulation source slots, both acting on the pitch of the two oscillators, make up the Pitch Mod section. For a source, the Oscillator Pitch Mod Source drop-downs let you reach for any of Env 1, Env 2 / Cyc, LFO, Key, Velocity, Modwheel, Pressure, or Slide. How strongly each source drives the pitch, anywhere from -100% to 100%, is fixed by the Oscillator Mod Amount sliders.

Drive pitch with an LFO running in the Ratio time mode and you can produce FM tones.

#### 30.3.2.4 Waveform Display

Drift’s Waveform Display.

What the waveform display renders is the merged output of Osc 1, Osc 2, and, when switched on, the noise generator. Tweak the oscillators and you will watch the waveform shift in the display.

#### 30.3.2.5 Oscillator Mixer

Drift’s Oscillator Mixer.

Within Drift’s Oscillator Mixer, switches let you switch on Oscillator 1 and 2 along with a noise generator that mixes white noise into the combined waveform.

Each oscillator and the noise generator also gets its own gain, set with the Osc 1, Osc 2, and Noise controls. With filter processing engaged, pushing oscillator gain high can hit the filters’ ceiling, or “headroom,” where they cease behaving linearly and yield an intricate distortion reminiscent of analog gear.

Two saturation stages within the filter circuitry are responsible for that distortion — one ahead of the filter and one behind it. Raising oscillator gain past its -6.0 dB default kicks in the first saturation stage, and the second engages once gain climbs above 0.0 dB.

Flipping the arrow toggles beside the gain controls turns on filter processing for the oscillators and noise generator. Leave filter processing off and the oscillator and noise output skips the filter altogether.

Retrigger for the oscillators is toggled on or off by the R toggle. With Retrigger on, each oscillator’s phase snaps back to a shared starting point whenever a note sounds; leave it off and the oscillators run freely.

### 30.3.3 Filter Section

Drift’s Filter Section.

A major part of carving the oscillators’ timbres falls to filtering.

Drift’s Filter section provides a low-pass filter switchable between two types, filter key tracking, a resonance control, a high-pass filter, and a pair of frequency modulation controls.

Cutoff for the low-pass filter is set by the Freq knob. The Type toggle moves between a couple of separate low–pass options: Type I (12 dB/octave) alongside Type II (24 dB/octave).

Type I relies on a DFM-1 filter that recirculates more of its own distortion, spanning a wide tonal range from gentle filter sweeps to warm drive.

Type II carries the Cytomic MS2 filter, built on a Sallen-Key topology with soft clipping to rein in resonance.

How strongly the pitch of arriving MIDI notes steers the low-pass filter’s frequency is set by the Key slider. At a value of 0.00, MIDI notes leave filter frequency untouched. At 1.00, low notes pull the filter frequency down and high notes push it up.

Resonance of the low-pass filter is set by the Res knob, and cutoff for the high-pass filter is set by the HP knob.

You may also click anywhere within the Filter section to reach and edit the envelope through the Envelopes section display via an X-Y controller. Drag the left filter dot side to side to fix the high-pass frequency. Drag the right filter dot side to side for the low-pass frequency or up and down for the resonance amount.

For the low-pass filter cutoff, up to two modulation sources are pickable through the Low-pass Modulation Source drop-downs inside the Freq Mod section. How strongly each source drives the frequency, anywhere from -100% to 100%, is fixed by the Low-pass Modulation Amount sliders.

### 30.3.4 Envelopes Section

Drift’s Envelopes Section.

In general, envelopes dictate the way a sound’s amplitude evolves from the instant a note begins until it stops.

A pair of standalone envelopes lives in Drift’s Envelopes section: one governing how amplitude changes and a second meant purely for modulation.

#### 30.3.4.1 Envelope 1

How the Oscillator section’s output amplitude (taking in both oscillators plus the Noise generator when active) starts and evolves once a note begins and then ends is governed by Envelope 1.

The Attack, Decay, Sustain, and Release controls can be set via their knobs or by reshaping the envelope right in the display.

_Attack_ fixes the span needed to climb from the starting value up to the peak value.

_Decay_ fixes the span needed to fall from the peak value down to the Sustain level.

_Sustain_ fixes the level held once the Decay stage closes; the envelope stays there until the note finishes.

_Release_ fixes the span needed to drop back to zero after the note ends.

Switching between Envelope 1 and Envelope 2 happens by clicking the matching section in the UI or by using the _1_ and _2_ toggles within the display. Whichever envelope is active appears in the display ready to edit.

#### 30.3.4.2 Envelope 2

Attack, Decay, Sustain, and Release controls belong to Envelope 2 as well; unlike Envelope 1 though, Envelope 2 is not tied to amplitude by default and can serve as a source for every modulation source slot inside Drift.

Flipping the switch to the left of the Attack control converts Envelope 2 from an ADSR envelope into a Cycling Envelope.

Cycling Envelope.

What the Cycling Envelope behaves like is an LFO modulation that relaunches with every arriving MIDI note.

The envelope’s midpoint is shifted by the Tilt knob, and at very low or very high settings it can also reshape the envelope’s slopes. How long the envelope sits at its peak is fixed by the Hold control.

Out of the box, the Cycling Envelope shows the Rate control, one of four available time modes alongside Ratio, Time, and Sync. Click the switches beside the control to choose another. According to the time mode, the cycle rate is set in Hz, ratio, milliseconds, or tempo-synced beat divisions.

### 30.3.5 LFO Section

Drift’s LFO Section.

Just like the Cycling Envelope, Drift’s LFO offers one of four distinct time modes: Rate, Ratio, Time, or Sync. Which mode is chosen sets the LFO’s cycle rate in Hz, ratio, milliseconds, or tempo-synced beat divisions.

Within the LFO display, nine waveforms are pickable from the drop-down:

- Sine
- Triangle
- Saw Up
- Saw Down
- Square
- Sample & Hold
- Wander is a sample and hold carrying an S-shape that eases between a pair of values at the LFO’s rate.
- Linear Envelope is a single-shot decay envelope whose decay is linear.
- Exponential Envelope is a single-shot decay envelope whose decay is exponential.

Retrigger is toggled on or off with the R switch. When on, the LFO snaps back to the same point in its phase each time a note fires. When off, the LFO runs freely.

Overall LFO intensity is set by the LFO Amount knob. A source for the LFO is picked from the LFO Modulation Source drop-down, while how strongly that source acts on the LFO is fixed by the LFO Modulation Amount slider.

### 30.3.6 Mod Section

Drift’s Mod Section.

Nearly every parameter in Drift can be modulated; within the Mod section you may pick as many as three modulation sources and their destinations.

Available sources, picked through the Modulation Source choosers, are Env 1, Env 2 / Cyc, LFO, Key, Velocity, Modwheel, Pressure, or Slide.

The Modulation Destination choosers expose the following targets. Among the oscillator and noise options are Osc 1 Gain, Osc 1 Shape, Osc 2 Gain, Osc 2 Detune, and Noise Gain. On the filter and rate side you will find LP Frequency, LP Resonance, HP Frequency, LFO Rate, Cyc Env Rate, plus Main Volume.

How strongly the chosen destination responds to the source, anywhere from -100% to 100%, is fixed with the Modulation Amount sliders.

### 30.3.7 Global Section

Drift’s Global Section.

How the instrument behaves and performs overall is governed by Drift’s global controls.

Drift’s four Voice Modes are selectable through the Mode chooser:

_Poly_ assigns a single voice to each note and supplies as many as 32 voices of polyphony.
