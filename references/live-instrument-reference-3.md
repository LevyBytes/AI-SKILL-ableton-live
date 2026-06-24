# Live Instrument Reference (part 3)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

_Mono_ sounds a single note at any moment, yet that note draws on four voices to build a unison character governed by the Mono Thickness setting. With the Mono Thickness slider, you balance the relative loudness of the four voices tied to each individual note. Set Thickness to 0 and a note sounds through a lone voice. Push Mono Thickness upward and the remaining three voices grow louder until each note carries them audibly. Whenever a fresh note arrives, it cuts off the prior note that is still sounding, assuming you continue to hold it.

_Stereo_ assigns two voices to each note and spreads them toward the left and right channels. The Stereo Spread slider controls the degree of panning spread distributed among the separate voices. Raise the amount and the voices separate further, which yields a broadening result.

_Unison_ gently detunes each note's four voices, treating them as independent of one other. With the Unison Strength slider, you set the extent of pitch deviation spread among the separate voices. Crank it up and each voice receives a greater degree of variation.

To cap how many voices may sound at once, choose a value from the Voices drop-down menu. Some Voice Modes draw on a larger voice count than the notes you actually trigger, so the resulting polyphony shifts based on whichever Voice Mode is active. As an illustration, with the Voices amount set to 32 voices:

- Poly mode applies 1 voice per note, giving a ceiling of 32-note polyphony.
- Stereo mode applies 2 voices per note, giving a ceiling of 16-note polyphony.
- Unison mode applies 4 voices per note, giving a ceiling of 8-note polyphony.

The Drift slider introduces a touch of variation into every voice, touching assorted facets of how that voice sounds, including pitch and filter cutoff. In Drift, each voice gets its own randomization applied to the oscillators and to filter frequency; turning the Drift control up or down scales that individual randomization. Push the amount higher and the spread between the oscillators and the filter grows wider, pulling the sound further out of tune.

With the Voice Mode set to Mono, you may switch on the Legato toggle so that starting a new voice shifts its pitch while leaving its envelopes untouched. The Glide slider governs how long overlapping notes take to glide their pitch toward the next arriving pitch whenever notes play legato.

The Volume knob fixes the instrument's overall loudness, whereas the Vel > Vol slider controls the degree to which volume responds to incoming MIDI note velocity.

With the Transpose slider you shift the global pitch by semitones across a span of -48 to 48 st. Turn on the Note PB toggle to activate per-note pitch bend. Turning Note PB off allows an MPE controller to work without pitch shifting according to finger placement. The PB Range slider establishes the global pitch bend span measured in semitones.

### 30.4 Drum Sampler

The Drum Sampler Instrument.

Drum Sampler is an instrument built for triggering one-shot samples inside Drum Racks. It provides core sampler capabilities including start and length controls, an AHD amplitude envelope, plus pitch controls. On top of that, Drum Sampler bundles a filter section, modulation choices, and a suite of purpose-built playback effects that reshape samples in many ways.

### 30.4.1 Sample Controls Section

Drum Sampler’s Sample Controls Section.

Within the Sample Controls section, you can edit the sample's envelope, pitch, and volume, and also exchange whatever sample is loaded.

You load a sample into Drum Sampler by double-clicking a file in the browser, or by dragging and dropping it onto the waveform display.

The Sample Start slider fixes where playback of the sample starts, expressed as a percentage of the sample's length. Holding Shift as you drag the slider nudges the start position in fine steps, and at the same time the display zooms into the waveform.

The Sample Length slider determines the duration of the played region, again expressed as a percentage of the sample's overall length.

With the Sample Gain slider you tune the sample's loudness, ranging from -70 to 24 dB.

Tweaking the Sample Start, Sample Length, and Sample Gain controls likewise refreshes the waveform shown in the display.

The Attack, Hold, and Decay controls let you shape the sample's envelope.

Attack establishes how long it takes to move from the envelope's starting level up to its peak.

Hold establishes how long the envelope's amplitude stays at the peak after the attack time elapses in Trigger mode. Setting the Hold time to inf (i.e., infinite) lets the sample play across its full length. Keep in mind this parameter is greyed out whenever the device's Envelope Mode is switched to Gate.

Decay establishes how long it takes to fall from the peak back down to zero once the Hold time passes in Trigger mode, or as soon as the note releases in Gate mode.

The Transpose slider fixes the global transposition figure, spanning -48 to 48 semitones, and the Detune slider fixes the global detune figure, spanning -50 to 50 cents.

Drum Sampler provides two envelope modes, Trigger and Gate. Under Trigger mode, the sample keeps sounding for the length of the configured Hold time once a note releases. Under Gate mode, the sample tapers off following the configured Decay time after a note releases.

Moving the cursor over the waveform display surfaces extra controls for handling the sample that is loaded.

The Similar Sample Swapping and Hot-Swap Controls.

Click the Swap to Next Similar Sample button to step through samples that [sound similar](https://www.ableton.com/en/live-manual/12/live-concepts/#sound-similarity) to your original file. To move backward among the choices, click the Swap to Previous Similar Sample button. Alternatively, right-click the display and pick Show Similar Files, which opens a browser list of comparable samples.

While stepping through samples, you can jump back to the file you first loaded by right-clicking the waveform display and choosing _Return to Reference_. To mark the file presently loaded as a fresh reference for swapping, choose the _Save as Similarity Reference_ option.

The hot-swap button launches the Hot-Swap Browser, letting you switch the loaded sample for another. To swap Drum Sampler out for a different instrument, click the hot-swap button located in the device's title bar.

### 30.4.2 Playback Effects Section

Drum Sampler’s Playback Effects Section.

A sample's sound can be shaped further with any one of nine playback effects. The first four are Stretch, Loop, Pitch Env, and Punch; the rest comprise 8-Bit, FM, Ring Mod, Sub Osc, and Noise.

Every playback effect carries two parameters, controllable through their own knobs or through the X/Y pad. Drag up and down on the X/Y pad for the first parameter, then drag side to side for the second.

The Playback Effect On toggle switches this whole section on or off. Once it is on, pick an effect through the Playback Effect Type drop-down menu.

_Stretch_ alters the sample's duration while leaving pitch intact. The outcome is granular artifacts that lend a lo-fi quality to the sound. The Factor control determines how much time-stretching occurs, given as a multiple of the original playback speed. The Grain Size control determines, in milliseconds, the grain size used when time-stretching the sample.

_Loop_ repeats a segment of the sample. The Loop Offset control positions the loop start relative to where the sample starts. The Loop Length control sets, in milliseconds, how long the loop lasts.

_Pitch Env_ drives the sample's pitch over time through an envelope. The Pitch Envelope Amount control sets how much pitch modulation occurs, ranging from -100 to 100%. Positive figures push the pitch up, whereas negative figures pull it down. The Pitch Envelope Decay control sets how long the pitch takes to settle back to the base value established by the device's global pitch controls.

_Punch_ imposes ducking using a fixed attack alongside an envelope tailored to accentuate the sample's transient. The Punch Amount control sets how much ducking is imposed. The Punch Release control sets how long the gain reduction needs to climb back to zero following the initial trigger.

_8-Bit_ blends filtering with bit reduction and sample rate reduction to evoke how 8-bit CPU chips sound. Playback sample rate for the sample is governed by the 8-Bit Sample Rate control. How quickly the effect's built-in low-pass filter decays is governed by the 8-Bit Decay Time control.

_FM_ employs a sine wave to drive the sample's pitch. The Amount control sets how strong the frequency modulation is, and the FM Frequency control sets the frequency that modulates the sample's pitch.

_Ring Mod_ imposes ring modulation upon the sample. The Amount control sets how much modulation occurs. The Ring Mod Frequency control sets the frequency that modulates the sample's amplitude. Low figures yield a tremolo effect, whereas high figures yield artifacts characteristic of ring modulation.

_Sub Osc_ stacks a sub oscillator on top of the sample. The Sub Oscillator Amount knob sets that oscillator's level. For its envelope, the device's attack plus decay settings are reused. The oscillator's frequency, ranging across 30 to 120 Hz, is set by the Sub Oscillator Frequency.

_Noise Osc_ stacks a noise oscillator on top of the sample. The Noise Amount knob sets that oscillator's level. For its envelope, the device's attack plus decay settings are reused. The frequency that filters the oscillator is set by the Noise Color control.

Keep in mind that the time-based and frequency-related controls within the Stretch, Loop, FM, Ring Mod, Sub Osc, and Noise Osc effects respond to the device's global pitch controls together with the MIDI note triggered. Because of this, each effect's pitch tracks the sample's pitch as you trigger different notes or transpose the sample.

On top of that, the global decay time governs the modulation decay of the FM and Ring Mod effects. As an example, when decay times are short, modulation reaches only the sample's transient.

### 30.4.3 Filter Section

Drum Sampler’s Filter Section.

The Filter On toggle switches the filter on or off.

You can pick from four filter types. Two are low-pass varieties, namely a 12 dB low-pass filter and a 24 dB low-pass filter; the remaining pair is a 24 dB high-pass filter together with a peak filter.

Both the low-pass and high-pass filters carry their own Resonance and Filter Frequency controls. With the peak filter active, the Peak Filter Gain and Filter Frequency controls let you raise or lower a particular frequency range.

### 30.4.4 Global Section

Drum Sampler’s Global Section.

Within the Global Section, you can set the output volume, panning, velocity-to-volume ratio, and modulation parameters.

The Volume control sets the device's global output level, spanning -36 to 36 dB, and the Pan slider places the signal in the stereo field.

The Velocity to Volume slider governs how strongly incoming MIDI note velocity modulates the device's volume.

The Modulation Source toggle flips between a pair of modulation sources, Velocity or Slide (MPE). After that, pick a modulation target through the Modulation Destination drop-down menu.

The Filter target drives the filter cutoff frequency.

Each separate envelope stage can be modulated through the Attack, Hold, and Decay targets.

FX1 and FX2 modulate the two parameters belonging to whichever playback effect is currently chosen.

The Modulation Amount slider sets how much modulation reaches the target.

### 30.4.5 Context Menu Options for Drum Sampler

Beyond the standard device [context menu](https://www.ableton.com/en/live-manual/12/live-keyboard-shortcuts/#using-lives-context-menu) entries, a couple of choices belong specifically to Drum Sampler.

_Enable Per-Note Pitch Bend_ — This lets Drum Sampler take in per-note pitch bend messages, and it is on by default.

_Envelope Follows Pitch_ — This sizes the amplitude envelope according to the sample's pitch. With it on, the envelope keeps affecting the identical part of the sample even as the pitch gets transposed.

_Drum Sampler > Simpler_ — This swaps Drum Sampler for Simpler while keeping the sample's start and length positions.

While working with [Drum Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#drum-racks), the _Save as Default Pad_ option on a pad's context menu makes Drum Sampler the default for incoming samples.

The Save as Default Pad Option.

As a result, whenever a sample drops onto an empty drum pad, a Drum Sampler instance loads on its own.

### 30.5 Electric

The Electric Instrument.

Electric is a software electric piano created together with Applied Acoustics Systems. Drawing on the iconic instruments of the seventies, every component was modeled with state-of-the-art physical modeling technology to deliver lifelike, expressive sounds.

Physical modeling applies the laws of physics to mimic how an object behaves. Put differently, Electric works out, on the fly, the mathematical equations that describe how each of its components operates. Electric relies on neither sampling nor wavetables; instead the CPU computes the sound on the fly from the value of every parameter. Electric goes beyond a plain copy of vintage gear; you can dial its parameters to settings the real instruments could never reach, producing genuinely striking new sounds that still hold onto a warm acoustic character.

### 30.5.1 Architecture and Interface

The workings of the electric piano are in fact fairly straightforward. Striking a key on the keyboard sets off a hammer that strikes a fork. A magnetic coil pickup then amplifies that fork's sound and routes it to the output, much as happens with an electric guitar. Two pieces make up the fork, named the tine bar and tone bar. The hammer strikes the fork at the tine bar, whereas the tone bar acts as a tuned metal resonator, dimensioned to yield the right pitch. After the fork starts up, it keeps ringing by itself for quite a while. Releasing the key, however, brings a damper against the fork and silences it sooner.

The Electric interface splits into four primary sections: Hammer, Fork, Damper/Pickup, holding parameters tied to the instrument's tone and sound; plus the Global section, holding parameters that govern overall behavior and performance, including pitch bend and polyphony.

Clicking an individual section opens up every parameter it holds, or you can click the Hammer, Fork, or Damper/Pickup icons to flip among those sections.

Electric’s Hammer, Fork, and Damper/Pickup Icons.

### 30.5.2 Hammer Section

Electric’s Hammer Section.

The Hammer section holds the parameters that concern the hammer's own physical properties, along with how your playing influences it.

The Stiffness knob sets how hard the hammer's striking surface is. Higher figures emulate a firmer surface, giving a brighter sound, while lower figures give a softer surface and a mellower sound. Velocity and note pitch can also shape Stiffness by way of the Vel and Key sliders located in the display's lower half.

The Noise knob sets the level of impact noise produced as the hammer strikes the fork. Inside the Noise section in the display's lower half, the Pitch slider sets the center frequency of the noise pitch, and the Decay slider sets how long the noise needs to die away to silence. The Key slider sets the degree to which note pitch governs the noise volume.

The Force section sets how forceful the hammer's strike on the fork is. Low Amount figures emulate a gentle strike, while high figures give a forceful strike. Velocity and note pitch can also shape Force through the Vel and Key sliders.

### 30.5.3 Fork Section

Electric’s Fork Section.

The Fork section carries knobs for the Tine and Tone parameters alike, which form the core of Electric's sound-producing mechanism.

Tine governs the part of the fork that the hammer strikes directly.

The Color slider governs the relative loudness of the high and low partials within the tine's spectrum. Low figures yield lower harmonics, and higher figures yield higher harmonics.

The Decay knob sets how long the tine's sound takes to fade away while a note remains held. Note pitch can modulate the tine's volume level by way of the Key slider.

Tone governs the fork's secondary resonance.

The Release slider covers both Tine and Tone, governing how long the fork's sound takes to decay once a key releases. The Decay parameter behaves just as it does within the Tine subsection.

### 30.5.4 Damper/Pickup Section

Electric’s Damper/Pickup Section.

#### 30.5.4.1 Pickup Parameters

Within Electric, the Pickup mimics how the magnetic coil pickup behaves as it amplifies the resonating fork's sound.

The Symmetry knob together with the Distance slider set the pickup's physical placement against the tine. Symmetry mimics the pickup's vertical placement. Set to 50%, the pickup sits squarely in front of the tine, giving a brighter sound. Lower figures shift the pickup beneath the tine, and higher figures shift it above. Distance sets how far the pickup sits from the tine. Higher figures widen that gap, while lower figures draw the pickup nearer. Be aware that the sound grows more overdriven the closer the pickup gets to the tine.

The Type R and W buttons toggle between two distinct pickup types. With R selected, Electric mimics electro-dynamic pickups, whereas W draws on an electro-static model.

You use the Input slider to set how much of the fork's signal reaches the pickup, which in turn governs how much distortion lands on the overall signal. The Output slider sets how much signal the pickup section puts out. Mixing these two parameters in various ways can produce markedly different outcomes. As an example, a small input paired with a large output yields a cleaner sound than a large input paired with a small output. Note pitch can further modulate the output level by way of the Key slider.

#### 30.5.4.2 Damper Parameters

An electric piano's metal forks are built to ring on for a long stretch while a key stays held. The component that governs that sustain is termed the damper. Pressing a key lifts that note's damper off its fork. Releasing the key brings the damper back against the fork to halt its vibration. The dampers, though, generate a faint sound of their own, both as they engage and as they release. The Damper parameters reproduce this distinctive noise.

The Tone slider sets how stiff the dampers are. Lower figures emulate soft dampers and give a mellower sound. Higher figures stiffen the dampers and give a brighter sound. The Level slider sets the overall quantity of damper noise.

The Att/Rel slider sets whether damper noise appears as the dampers engage the fork or as they release. Set to -100, damper noise sounds solely throughout the note's attack phase. Set to 100, the noise sounds solely throughout the release phase. At the midpoint, equal noise appears across both attack and release.

### 30.5.5 Global Section

Electric’s Global Section.

The Global section holds the parameters governing Electric's overall behavior and performance.

The Volume knob fixes Electric's overall output level.

The Voices chooser fixes the polyphony on offer. Because every active voice draws extra CPU, you might have to try out this setting to strike a sensible balance between playability and performance.

The Semi and Detune sliders serve as coarse and fine tuners. Semi shifts the whole instrument up or down by semitone steps, while the Detune slider moves in one-cent steps (reaching a maximum of 50 cents either up or down).

Stretch reproduces a method called stretch tuning, a widespread adjustment applied to both electric and acoustic pianos that forms an essential part of their distinctive sound. Set to 0%, Electric performs in equal temperament, where two notes lie an octave apart once the higher note's fundamental pitch is precisely double that of the lower note. Yet because a vibrating tine or string resonates differently from the theoretical ideal, equal temperament has a way of sounding “wrong“ on pianos. Stretch tuning aims to fix this by raising the pitch of higher notes and lowering the pitch of lower notes, producing a more brilliant sound. Negative figures reproduce “negative“ stretch tuning, where higher notes flatten while lower notes sharpen.

Pitch Bend fixes, in semitones, the span of global pitch bend modulation, while Note PB fixes, in semitones, the MPE per-note pitch bend span.

### 30.6 External Instrument

The External Instrument.

The External Instrument device is not actually an instrument; it is a routing helper that makes it simple to fold external (hardware) synthesizers and multitimbral plug-ins into your projects. It dispatches MIDI outward and brings audio back.

The two MIDI To choosers pick the destination where the device sends its MIDI data. The upper chooser picks either a physical [MIDI port](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#midi-port-inputs-and-outputs) or a multitimbral plug-in. Pick a MIDI port (for an external synthesizer) and the lower chooser then offers MIDI channel numbers.

Should a different track in your Set hold a multitimbral plug-in, you can pick that track from the upper chooser. Here the lower chooser lets you target a particular MIDI channel inside the plug-in.

The Audio From chooser supplies choices for bringing audio back from the hardware synth or plug-in device. When routing to a hardware synth, use this chooser to pick the ports on your audio interface wired to your synth's output. Which choices appear hinges on what is configured in the Audio Settings.

When routing to a multitimbral plug-in sitting on another track in your Live Set, the Audio From chooser presents the plug-in's auxiliary outputs. Bear in mind the main outputs come through on the track that holds the instrument.

The Gain knob sets the level of audio arriving back from the sound source. Set this level with care so that clipping is avoided.

Because external devices may add latency that Live cannot detect on its own, you can offset any delays by hand using the Hardware Latency slider. The button beside this slider lets you express your latency compensation either in milliseconds or in samples. When your external device links to Live over a digital connection, you should configure latency in samples, so that the sample count you enter holds even as you change the sample rate. When your external device links to Live over an analog connection, you should configure latency in milliseconds, so that the time you enter holds as you change the sample rate. Bear in mind that working in samples affords finer control, so even with analog devices you might choose to “fine tune“ latency in samples to reach the lowest latency achievable. If you do, remember to switch back to milliseconds ahead of changing your sample rate. Live compensates automatically for any latency that its own internal devices add, so the slider is disabled whenever the External Instrument Device routes internally.

Note: Should you leave the [Delay Compensation](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#device-delay-compensation) option unticked within the Options menu, then the Hardware Latency slider becomes unavailable.

For fuller details on routing setups involving the External Instrument device, consult the [Routing and I/O](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) chapter.

### 30.7 Impulse

The Impulse Instrument.

Impulse is a drum sampler offering sophisticated modulation features. The eight drum samples placed in Impulse's sample slots can be time-stretched, filtered, and shaped by envelope, saturation, pan, and volume components, almost all of which respond to random and velocity-driven modulation.

### 30.7.1 Sample Slots
