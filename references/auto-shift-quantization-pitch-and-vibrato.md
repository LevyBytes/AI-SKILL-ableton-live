# Auto Shift Quantization Pitch And Vibrato

Open when you need guidance on Auto Shift Quantization Pitch And Vibrato in Ableton Live.

Context: [Auto Shift](pitch-rhythm-tone-and-compression-routes.md#284-auto-shift).

<a id="source-2842-quantizer-tab"></a>
### 28.4.2 Quantizer Tab

Auto Shift’s Quantizer Tab.

Working from the notes of a chosen scale, the Quantizer pulls your incoming audio into tune. The Quantizer tab gathers both the controls for watching how the signal gets handled and the ones for fine-tuning the correction itself.

In cents, the Pitch Correction Meter shows the degree to which the arriving signal is being nudged toward the target note named just under the meter. That target note comes from whichever scale you have set.

Dial in how aggressive the correction is with the Correction Strength slider — raise it and the audio is pulled harder toward the target note. The Smooth toggle flips smoothing on or off; once on, the jumps between notes are eased and a more lifelike vibrato survives. Smoothing duration runs from 0 to 200 milliseconds via the Smoothing Time slider. Together, the Correction Strength and Smoothing parameters set the character of the tuning, spanning everything from delicate and organic to stiff and heavily quantized.

Which notes feed the correction is decided by the Included Notes in Scale display. Build a scale of your own by clicking notes there, or define the key and scale through the Root and Scale choosers. The Pitch Shift slider transposes the pitch by scale degrees in either direction, and that shift lands after the correction has been applied.

Scale awareness is supported too: flip on the Use Current Scale toggle in the title bar and the Quantizer tracks the clip’s active scale. On top of that, the Included Keys in Scale display tints the chosen scale’s notes purple, and the Root and Scale choosers go dim.

<a id="source-2843-midi-tab"></a>
### 28.4.3 MIDI Tab

Auto Shift’s MIDI Tab.

Once [MIDI input](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#midi-input) is switched on, the MIDI tab takes the place of the Quantizer tab and lets you tailor how arriving MIDI behaves.

As notes stream in from the source track, the piano visualization shows them; the device then leans on those notes to tune the incoming audio.

Using MIDI Notes to Pitch Correct Audio.

Keep in mind that scale awareness drops out the moment you switch to MIDI input. If you still want notes confined to a particular scale, drop the [Scale MIDI effect](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#scale) onto the source track. Just be sure Auto Shift’s Tapping Point chooser sits at Post FX or Post Mixer, so that effect gets picked up.

Spanning 0 to 1,000 milliseconds, the Attack Time slider governs the attack of the note’s envelope. Its Release Time counterpart sets the envelope’s release across a 0 to 5 seconds range.

Flip on the Note Latch toggle and MIDI notes sustain right up until the next Note On message arrives. The device’s bend span, from 0 to 48 semitones, is dialed in with the Pitch Bend Range control.

Within the Mod Routing section, MIDI or MPE data can drive four targets: Pitch, Formant, Volume, and Pan. Six sources are available to drive any of them: Velocity, Pressure, Mod Wheel, Pitch Bend, Note PB, or Slide. Pick the source from each target’s own Mod Source drop-down menu, then dial in how deep the effect goes using its matching Mod Depth slider.

<a id="source-2844-lfo-tab"></a>
### 28.4.4 LFO Tab

Auto Shift’s LFO Tab.

The onboard LFO lets you push modulation onto the pitch, formants, volume, and panning of the audio coming in.

Re-triggering of the LFO is governed by the LFO Reset toggle. With it on, the LFO’s phase restarts at each note onset. Under the Quantizer, an onset registers whenever a pitch surfaces following a stretch of unpitched sound. Every time the phase restarts, the Onset Indicator LED blinks. Switch to MIDI input and an onset instead marks the beginning of a fresh note, with the Onset Indicator turning into the Trigger Indicator.

Across a 0 to 1.5 seconds window, the LFO Delay slider holds off the attack phase. Its companion LFO Attack slider, ranging from 0 to 2 seconds, governs how long the LFO takes to climb to full level. Adjust either one and the waveform shown in the display updates to match.

Nine modulation shapes sit in the LFO Waveform drop-down menu. The choices are Sine, Triangle, Triangle 8 and Triangle 16, followed by Saw Up, Saw Down, Rectangle, then Random and Random S&H.

Whether the LFO Rate slider is read in milliseconds or as tempo-locked beat divisions depends on how the LFO Sync toggles are set; the slider sets the LFO’s speed either way.

The same four destinations — Pitch, Formant, Volume, and Pan — can be driven by the LFO from within the Mod Routing section. Each one has its own Mod Depth slider that fixes how much modulation reaches that parameter.

It is worth noting that the LFO modulates the arriving signal whether or not pitch correction is happening at the time.

<a id="source-2845-pitch-section"></a>
### 28.4.5 Pitch Section

Auto Shift’s Pitch Section.

The Pitch section gives you controls for laying both pitch and formant shifting onto whatever signal arrives.

In semitones, the Pitch Shift control fixes how far the material is transposed, while the Pitch Shift Fine slider lets you trim that transposition in cents.

Formants — the resonant frequencies that lend a sound its tonal character — are moved with the Formant Shift control over a -100% to 100% span. Crank it up and pitches read brighter and more resonant; bring it down and they turn darker and thinner. Moving the formants is a way to push a sound higher or lower without ever transposing the actual pitch.

How closely formant shifting trails the pitch shifting is set by the Formant Follow slider; the more you raise it, the more natural the resulting transposition sounds.

Keep in mind that the Pitch Shift and Formant Shift controls work whether or not you are correcting the signal’s pitch.

<a id="source-2846-vibrato-section"></a>
### 28.4.6 Vibrato Section

Auto Shift’s Vibrato Section.

Controls for adding vibrato to the arriving audio, plus the overall blend of dry against processed sound, live in the Vibrato section.

Three core vibrato controls are on hand:

- Vibrato Amount: sets the vibrato depth across a 0 to 200 cents range.
- Vibrato Rate: sets the vibrato speed, anywhere from 2 to 15 Hz.
- Vibrato Fade In: sets, in milliseconds, how long the vibrato takes to fade in.

Turn on the Natural Vibrato toggle and slight fluctuations enter the vibrato’s rate and depth, lending it a more believable feel.

As before, these vibrato controls function with or without pitch correction engaged.

Blend between the dry and processed signals with the Dry/Wet slider. Hold it at 0% and no correction is heard; push it to 100% and only the corrected sound remains. Park it at 50% for a doubler-style effect, since that splits the original and corrected signals evenly.
