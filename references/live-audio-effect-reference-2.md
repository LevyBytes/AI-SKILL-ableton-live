# Live Audio Effect Reference (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Once a transient is registered, the Attack Time slider governs the number of milliseconds required before modulation climbs to its peak depth. Setting a lengthy attack lets you confine the processing to the held tail of a sound while sparing the opening spikes. With Panning mode active, this keeps those spikes anchored at the center of the stereo image; under Tremolo mode, it protects their punch instead.

How strongly the incoming level steers the LFO rate is governed by the Dynamic Frequency Modulation slider. Push it positive and louder material speeds the LFO rate up; pull it negative and the rate slows down instead.

### 28.4 Auto Shift

The Auto Shift Effect.

Tracking and tuning pitch in real time, Auto Shift bundles vibrato, pitch shifting, and formant shifting under one roof. While it shines at reshaping vocals, the device accepts any monophonic source. Correction can follow either a chosen scale or the MIDI notes arriving from another track. A built-in LFO is included as well, letting you modulate the incoming material as it plays.

### 28.4.1 Input Section

Auto Shift’s Input Section.

Both audio and MIDI can be fed into Auto Shift. Within the Input section you decide how the device handles those arriving signals.

Reported in notes and cents, the Input Pitch display reads out the pitch of whatever audio is coming in.

Three Pitch Range toggles let you constrain the audio input to a particular frequency band, which sharpens the accuracy of the pitch estimate and the correction. Pick High when the material sits up high, Mid for the middle band, and Bass for low-end content. An LED on each toggle blinks whenever the arriving audio lands inside that toggle’s band.

A Blinking Pitch Range LED Signals Which Band the Arriving Audio Occupies.

Keep in mind that every pitch range option carries its own latency cost, so moving from one toggle to another shifts the total latency.

To trim or boost the level of the arriving signal across a -24 to +24 dB span, reach for the Input Gain slider.

Expressed in milliseconds, the Latency Readout reports the device’s latency. Turning on Live Mode from the toggle in the title bar trims that latency, a handy benefit when you are performing live. Be aware, though, that this mode can introduce minor glitches at note onsets or during fast pitch movement.

Enable Live Mode to Reduce Latency.

#### 28.4.1.1 MIDI Input

Auto Shift’s MIDI Input Panel.

Switching on MIDI input means the notes from a different MIDI track drive the pitch correction of your audio, in place of locking it to a scale through the Quantizer.

Toggling MIDI In reveals or conceals the MIDI Input panel, where the track routing and voice mode controls live.

The MIDI On toggle turns MIDI input on or off. With it engaged, the [Quantizer tab](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#quantizer-tab) gives way to the [MIDI tab](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#midi-tab), which offers extra ways to mold how the arriving MIDI notes behave.

Which track feeds notes to Auto Shift — the MIDI sidechain source — is picked with the External Source chooser. With the Tapping Point chooser you decide whether that sidechain is tapped ahead of or behind any MIDI effects sitting in the source track’s chain. Choose Pre FX to skip those effects, or Post FX or Post Mixer to keep them in play.

Two voice mode toggles are on offer: Mono and Poly. Mono runs a single voice, so just one note drives the correction at any moment. The Glide slider controls how long overlapping notes take to glide from one pitch to the next. Poly stacks as many as eight voices simultaneously, which suits harmony work; the Voice Count chooser caps that total at 2, 4, or 8.

Bear in mind that with MIDI input engaged, Auto Shift stays silent until it actually receives MIDI notes.

### 28.4.2 Quantizer Tab

Auto Shift’s Quantizer Tab.

Working from the notes of a chosen scale, the Quantizer pulls your incoming audio into tune. The Quantizer tab gathers both the controls for watching how the signal gets handled and the ones for fine-tuning the correction itself.

In cents, the Pitch Correction Meter shows the degree to which the arriving signal is being nudged toward the target note named just under the meter. That target note comes from whichever scale you have set.

Dial in how aggressive the correction is with the Correction Strength slider — raise it and the audio is pulled harder toward the target note. The Smooth toggle flips smoothing on or off; once on, the jumps between notes are eased and a more lifelike vibrato survives. Smoothing duration runs from 0 to 200 milliseconds via the Smoothing Time slider. Together, the Correction Strength and Smoothing parameters set the character of the tuning, spanning everything from delicate and organic to stiff and heavily quantized.

Which notes feed the correction is decided by the Included Notes in Scale display. Build a scale of your own by clicking notes there, or define the key and scale through the Root and Scale choosers. The Pitch Shift slider transposes the pitch by scale degrees in either direction, and that shift lands after the correction has been applied.

Scale awareness is supported too: flip on the Use Current Scale toggle in the title bar and the Quantizer tracks the clip’s active scale. On top of that, the Included Keys in Scale display tints the chosen scale’s notes purple, and the Root and Scale choosers go dim.

### 28.4.3 MIDI Tab

Auto Shift’s MIDI Tab.

Once [MIDI input](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#midi-input) is switched on, the MIDI tab takes the place of the Quantizer tab and lets you tailor how arriving MIDI behaves.

As notes stream in from the source track, the piano visualization shows them; the device then leans on those notes to tune the incoming audio.

Using MIDI Notes to Pitch Correct Audio.

Keep in mind that scale awareness drops out the moment you switch to MIDI input. If you still want notes confined to a particular scale, drop the [Scale MIDI effect](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#scale) onto the source track. Just be sure Auto Shift’s Tapping Point chooser sits at Post FX or Post Mixer, so that effect gets picked up.

Spanning 0 to 1,000 milliseconds, the Attack Time slider governs the attack of the note’s envelope. Its Release Time counterpart sets the envelope’s release across a 0 to 5 seconds range.

Flip on the Note Latch toggle and MIDI notes sustain right up until the next Note On message arrives. The device’s bend span, from 0 to 48 semitones, is dialed in with the Pitch Bend Range control.

Within the Mod Routing section, MIDI or MPE data can drive four targets: Pitch, Formant, Volume, and Pan. Six sources are available to drive any of them: Velocity, Pressure, Mod Wheel, Pitch Bend, Note PB, or Slide. Pick the source from each target’s own Mod Source drop-down menu, then dial in how deep the effect goes using its matching Mod Depth slider.

### 28.4.4 LFO Tab

Auto Shift’s LFO Tab.

The onboard LFO lets you push modulation onto the pitch, formants, volume, and panning of the audio coming in.

Re-triggering of the LFO is governed by the LFO Reset toggle. With it on, the LFO’s phase restarts at each note onset. Under the Quantizer, an onset registers whenever a pitch surfaces following a stretch of unpitched sound. Every time the phase restarts, the Onset Indicator LED blinks. Switch to MIDI input and an onset instead marks the beginning of a fresh note, with the Onset Indicator turning into the Trigger Indicator.

Across a 0 to 1.5 seconds window, the LFO Delay slider holds off the attack phase. Its companion LFO Attack slider, ranging from 0 to 2 seconds, governs how long the LFO takes to climb to full level. Adjust either one and the waveform shown in the display updates to match.

Nine modulation shapes sit in the LFO Waveform drop-down menu. The choices are Sine, Triangle, Triangle 8 and Triangle 16, followed by Saw Up, Saw Down, Rectangle, then Random and Random S&H.

Whether the LFO Rate slider is read in milliseconds or as tempo-locked beat divisions depends on how the LFO Sync toggles are set; the slider sets the LFO’s speed either way.

The same four destinations — Pitch, Formant, Volume, and Pan — can be driven by the LFO from within the Mod Routing section. Each one has its own Mod Depth slider that fixes how much modulation reaches that parameter.

It is worth noting that the LFO modulates the arriving signal whether or not pitch correction is happening at the time.

### 28.4.5 Pitch Section

Auto Shift’s Pitch Section.

The Pitch section gives you controls for laying both pitch and formant shifting onto whatever signal arrives.

In semitones, the Pitch Shift control fixes how far the material is transposed, while the Pitch Shift Fine slider lets you trim that transposition in cents.

Formants — the resonant frequencies that lend a sound its tonal character — are moved with the Formant Shift control over a -100% to 100% span. Crank it up and pitches read brighter and more resonant; bring it down and they turn darker and thinner. Moving the formants is a way to push a sound higher or lower without ever transposing the actual pitch.

How closely formant shifting trails the pitch shifting is set by the Formant Follow slider; the more you raise it, the more natural the resulting transposition sounds.

Keep in mind that the Pitch Shift and Formant Shift controls work whether or not you are correcting the signal’s pitch.

### 28.4.6 Vibrato Section

Auto Shift’s Vibrato Section.

Controls for adding vibrato to the arriving audio, plus the overall blend of dry against processed sound, live in the Vibrato section.

Three core vibrato controls are on hand:

- Vibrato Amount — sets the vibrato depth across a 0 to 200 cents range.
- Vibrato Rate — sets the vibrato speed, anywhere from 2 to 15 Hz.
- Vibrato Fade In — sets, in milliseconds, how long the vibrato takes to fade in.

Turn on the Natural Vibrato toggle and slight fluctuations enter the vibrato’s rate and depth, lending it a more believable feel.

As before, these vibrato controls function with or without pitch correction engaged.

Blend between the dry and processed signals with the Dry/Wet slider. Hold it at 0% and no correction is heard; push it to 100% and only the corrected sound remains. Park it at 50% for a doubler-style effect, since that splits the original and corrected signals evenly.

### 28.5 Beat Repeat

The Beat Repeat Effect.

With Beat Repeat you can spin out either tightly controlled or randomized echoes of whatever signal feeds it.

How frequently Beat Repeat grabs fresh audio and starts looping it is governed by the Interval control. Locked to the song tempo, Interval takes values from ”1/32” up to ”4 Bars.” The Offset control nudges the moment that Interval marks later in time. Say Interval reads ”1 Bar” and Offset reads ”8/16”: audio is then grabbed for repetition once each bar at the third beat — that is, halfway, or eight-sixteenths, into the bar.

Inject some unpredictability with the Chance control, which governs how probable it is that repetitions actually fire when Interval and Offset call for them. Set Chance to 100 percent and a repetition fires every time at the chosen Interval/Offset moment; drop it to zero and none occur at all.

In sixteenth notes, Gate fixes how long all the repetitions run in total. With Gate at ”4/16”, the repeats span a single beat, kicking off from wherever Interval and Offset place them.

Pressing the Repeat button overrides everything above, instantly grabbing audio and looping it for as long as the button stays engaged.

Grid size — how big each repeated slice is — is set with the Grid control. At ”1/16”, a one-sixteenth-note slice gets grabbed and looped for the Gate length you specified (or until Repeat is switched off). Big grid settings spawn rhythmic loops, whereas tiny ones yield sonic artifacts. Pressing No Triplets forces the grid divisions to stay binary.

The Variation control randomizes grid size. Leave Variation at ”0” and the size stays locked; raise it and the grid swings widely around your chosen Grid value. The chooser underneath offers several Variation modes: Trigger spawns grid variations each time repetitions fire; 1/4, 1/8 and 1/16 spawn them on a steady clock; and Auto makes Beat Repeat roll a fresh random variation after every repetition — the densest grid variation the device offers, all the more so when triplets are permitted.

For unusual textures, the repetitions can be dropped in pitch. Beat Repeat handles this by resampling — stretching the segments to lower their pitch and then leaving them long rather than squeezing them back to compensate. The upshot is that the rhythm can grow rather murky at steep Pitch settings. The Pitch Decay control slopes the pitch curve so each successive slice plays lower than the one before. Warning: This is the most obscure parameter of Beat Repeat.

A joint low-pass and high-pass filter is built in to carve out the frequency range the device lets through. Dedicated controls let you toggle the filter and dial in the center frequency along with the width of that passed band.

The dry input that arrived at Beat Repeat gets blended with its repetitions through one of three mix modes: Mix lets the dry signal continue through with repetitions layered on top; Insert silences the dry signal while repetitions sound but lets it through otherwise; and Gate emits the repetitions alone and never the dry signal. That Gate mode comes in handy when the device sits on a return track.

The Volume control sets the device’s output level, and Decay lets you taper the repetitions so they fade away gradually.

### 28.6 Cabinet

The Cabinet Effect.

Cabinet is a device that recreates the tone of five vintage guitar cabinets. Built together with Softube, it relies on physical modelling to deliver a spread of convincing tones, complete with well-chosen mics and mic placement.

A range of speaker sizes and configurations is available from the Speaker chooser, whose entries spell out how many speakers there are and their size in inches. ”4x12,” for instance, denotes four 12-inch speakers. As in actual rigs, more speakers and bigger ones tend to push higher volume.

Where the virtual mic sits relative to the cabinet is governed by the Microphone chooser. Near On-Axis micing yields a bright, tightly focused tone, whereas Near Off-Axis comes across as more resonant and slightly duller. Pick the Far position for an even tone that also carries a touch of the simulated ”room.”

Cabinet Mic Positions.

Sitting under the Microphone chooser, a switch flips between a Dynamic and Condenser mic. Dynamic mics sound a little rougher and are the usual pick for close-micing guitar cabinets, since they cope with far louder levels. Condenser mics capture more faithfully and are the typical choice when micing at a distance. Naturally, Cabinet’s virtual condenser mic shrugs off loud levels unharmed, so experiment freely.

Mono versus stereo (Dual) processing is selected with the Output switch. Bear in mind that Dual mode doubles Cabinet’s CPU draw.

Balance between the processed and dry sound is handled by the Dry/Wet control.

### 28.6.1 Cabinet Tips

A few pointers for getting the most out of Cabinet:

#### 28.6.1.1 Amps and Cabinets

In practice, guitar amps drive guitar cabinets, which is why Cabinet ships alongside [Amp](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#amp) and the pair are typically run together. That said, running Amp and Cabinet apart from each other can yield intriguing, offbeat tones too.

#### 28.6.1.2 Multiple mics

Engineers often place several mics on one cabinet and then dial in their balance at mix time. Live’s [Audio Effect Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks) make this straightforward. Give this a go:

1. Dial in a single Cabinet instance however you prefer.
2. Drop that Cabinet inside an Audio Effect Rack.
3. Copy the Rack chain holding your original Cabinet as often as you wish.
4. Within each new chain, pick a fresh Microphone setting and/or a different mic type.
5. Balance the level of each Rack chain using the Rack’s mixer.

### 28.7 Channel EQ

The Channel EQ Effect.

Drawing on the EQs of vintage consoles, Channel EQ is a straightforward but adaptable three-band unit, tuned to give musical outcomes across many kinds of source material.

Flip the HP 80 Hz switch to engage a high-pass filter, handy for stripping low-end rumble out of a signal.

A low shelf filter centered at 100 Hz is driven by the Low parameter, which can lift or cut the low end by as much as +/- 15 dB. Its curve adapts on the fly, reshaping itself according to how much gain you apply.

A sweepable peak filter is governed by the Mid parameter, which — unlike Low and High — spans +/- 12 dB. The frequency slider sitting above Mid lets you place that filter’s center anywhere from 120 Hz to 7.5 kHz.

On a boost, the High parameter feeds a high shelf filter reaching up to 15 dB. On a cut, that shelf pairs with a low-pass filter: sweeping the control from 0 dB down toward -15 dB also drags the low-pass cutoff from 20 kHz down to 8 kHz.

A spectrum display gives you live visual feedback on the resulting filter curves and the processed sound.

The Output control applies gain to the processed signal and is there to make up for any level change the EQ moves introduce.

### 28.7.1 Channel EQ Tips

Drop Channel EQ later in a device chain and it can further tailor what comes out of a reverb.

It also works for tone-shaping a lone drum or a full kit — just place a Channel EQ instance on one Drum Rack pad or several.

Chain a [Saturator](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#saturator) after Channel EQ and you can mimic the analog nonlinearities of a console channel strip. Push the low end hard in that setup and you will also get more distortion, much as a real analog desk would respond.

### 28.8 Chorus-Ensemble

The Chorus-Ensemble Effect.

Chorus-Ensemble delivers a vintage two-delay-line chorus, with a third delay line available as an extra mode. Its reach is broad — from gentle thickening, through flanging and vibrato, all the way to lush string-ensemble chorus textures.

Active delay lines appear as waveforms in the device’s display, tracking whichever effect mode and settings you have dialed in. Three buttons in that display let you switch the device among its modes: Chorus, Ensemble, or Vibrato.

Chorus-Ensemble’s Display and Modes.

By folding two time-modulated delayed copies into the input, Chorus mode fattens the sound. Reach for it when you want that familiar chorus shimmer that brings a little movement to your signal.

Modeled on a fat three-delay-line chorus pedal from the ‘70s, Ensemble mode builds on Chorus mode and shares its controls, yet it yields a fuller, silkier, and more pronounced chorus by running three delayed copies whose modulation phases are spread out evenly.

Rather than blending in a delayed copy, Vibrato mode pushes the signal’s pitch further than either Chorus or Ensemble does. The result is a marked pitch wobble instead of the thickening the other modes give. Its modulation waveform can glide smoothly between a sine and a triangle, which lets you conjure the familiar “police siren” effect.

Every mode offers an optional high-pass filter. Switched on, it pulls back the modulation on anything below the cutoff set by the High-Pass Frequency slider, which spans 20.0 Hz to 2.00 kHz.

Beyond that filter, Chorus and Ensemble modes add the Width parameter, governing the stereo width of the wet signal and thus the chorus balance between the mid and side channels. At 0.0% the output is mono, at 100% the two are even, and at 200% the chorus runs twice as hot in the sides as in the center. Width helps you hold the effect’s level steady across the stereo image, which can pay off when mixing.

Two further controls belong to Chorus mode: Delay Time and Tap Count. The Delay Time chooser lets you opt for either a dynamic or a fixed delay. On Auto, the delay scales per tap in direct proportion to how much modulation is applied. Set to a fixed figure, it holds steady instead of riding the modulation amount, making it simpler to land a solid chorus free of stray phasing or pitch wobble — handy for bass or guitar. The Taps toggles flip between a one- or two-tap delay; the single tap leans toward plainer, wider chorus textures reminiscent of old hardware pedals.

Offset and Shape controls accompany Vibrato mode. Offset sets how much phase separates the left- and right-channel waveforms; at 180° the two sit fully out of phase. Shape reworks the modulation waveform — 0.0% gives a sine wave, 100% gives a triangle wave.

Chorus-Ensemble supplies modulation parameters for sculpting the overall character of the tone.

Modulation Controls in Chorus-Ensemble.

In Hertz, Rate fixes the modulation rate; adjust it with the dial or by dragging up and down inside the display. Crank Rate for a wilder chorus, or hold it low for softer phasing.

Amount controls the amplitude of the modulation signals acting on the delay times. The more you add, the further the time strays from its unmodulated setting.

Feedback dictates how much of each channel’s output loops back into its own input. Pushing it higher gets more extreme, builds up upper harmonics, and leaves audible echoes lingering after playback halts. You can flip the polarity of that signal with the Feedback Invert toggle, which produces a “hollow” character when paired with heavy feedback. Be aware that this control is greyed out in Vibrato mode.

The global parameters of Chorus-Ensemble hand you command over its output level, tonal warmth, and the blend of processed against dry sound.

Global Parameters in Chorus-Ensemble.

Output determines how much gain lands on the processed signal.

Warmth lays in a touch of distortion and filtering for a cozier tone. Push it up when you want things to sound grittier.

Dry/Wet balances the processed sound against the dry one. Dial it to 100% whenever Chorus-Ensemble lives on a return track. As elsewhere, this control is greyed out in Vibrato mode.

### 28.8.1 Chorus-Ensemble Tips

A couple of pointers for working with Chorus-Ensemble: - Run Ensemble mode with a rate of 1 Hz to 1.8 Hz and 100% Amount over dry guitars for that classic surf-rock tone. - Automate the Feedback Invert toggle while Feedback sits above 90% to unleash huge swells of decaying oscillation.

### 28.9 Compressor

The Compressor Effect.
