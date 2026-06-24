# Live Audio Effect Reference (part 4)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Delay offers two extra modes, reachable through Delay’s [context menu](https://www.ableton.com/en/live-manual/12/live-keyboard-shortcuts/#using-lives-context-menu) or by way of the Show Options menu found in the [device title bar](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#device-title-bar): _Hi-Quality_ and _Dry/Wet - Equal-Loudness_.

Turning on Hi-Quality switches the delay lines to a finer interpolation whenever the Repitch or Fade smoothing mode is active. On top of that, with Repitch mode any shifts in delay time receive a smoothing that emulates the behavior of analog tape.

The Dry/Wet - Equal-Loudness option toggles the output between linear and equal-loudness response. With it active, the apparent volume of both the unprocessed and processed paths remains steady as you move the Dry/Wet control. As a result, a 50/50 blend comes across as having equal loudness across the majority of signals.

### 28.11.2 Delay Tips

Below you’ll find suggestions for producing a variety of effects using Delay.

#### 28.11.2.1 Glitch Effect

Switch on Stereo Link and dial the delay time to 6 while in Sync mode. Bring Feedback up to 50%. Activate the band-pass filter, take the filter frequency to 2.86 kHz, and move the Width slider to 2.50. For the LFO waveform, pick S&H, then set its Rate to 0.93 Hz. Push the Delay slider to 66% and move the Filter slider to 19%. Choose the Fade smoothing mode and confirm that Ping Pong stays off. Position the Dry/Wet control anywhere from 50% - 80% according to the sound you’re after.

#### 28.11.2.2 Chorus Effect

Turn off Stereo Link, dial the left channel’s delay time to 12.0 ms, and bring the right channel’s delay time to 30.0 ms. Take Feedback down to 0.0%. Activate the band-pass filter, dial its filter frequency up to 2.56 kHz, then push the Width slider to 8.50. Pick the Triangle LFO waveform and set the Rate to 0.65 Hz. Move the Delay slider to 58% and keep the Filter slider parked at 0.0%. Choose the Repitch smoothing mode and switch on Ping Pong. Place the Dry/Wet control anywhere from 45% - 65% according to the result you want.

### 28.12 Drum Buss

The Drum Buss Effect.

Drum Buss is an analog-style drum processor built to lend weight and personality to a collection of drums, all while binding them into a cohesive, tight mix.

Use the Trim slider to lower the incoming level ahead of any processing being applied to the signal.

Switching on the Comp toggle inserts a fixed compressor ahead of the distortion stage on the input signal. That compressor is tuned for evening out drum groups, featuring a fast attack, a medium release and a moderate ratio, plus generous makeup gain.

The input signal can be routed through one of three distortion types. Every type ramps up the amount of distortion while contributing its own flavor to the resulting tone:

- Soft: waveshaping distortion
- Medium: limiting distortion
- Hard: clipping distortion with bass boost

When you want more bite, you can push the input harder before it hits the distortion stage. The Drive control governs how much drive gets applied to the input signal.

Drum Buss bundles together the drum-processing tools people reach for most when sculpting the mid-high range and bolstering the low end, both of which the next sections explore.

#### 28.12.0.1 Mid-High Frequency Shaping

The tools for shaping mid-high frequencies are meant to bring clarity and presence to drums like snares and hi-hats.

The Crunch parameter governs how much sine-shaped distortion is applied across the mid-high frequencies.

A low-pass filter sits behind the Damp control, stripping out unwanted high frequencies that may surface once distortion has been introduced.

The Transients knob accentuates or softens the transients of frequencies sitting above 100 Hz. Pushing it positive adds attack and lengthens sustain, producing a full, “punchy” character. Moving it negative likewise adds attack yet trims sustain. That tightens the drums up, delivering a sharper, crisper tone with reduced room and rattle.

#### 28.12.0.2 Low-End Enhancement

The low-end enhancement in Drum Buss relies on a pair of tools: a resonant filter that strongly lifts bass frequencies, plus a Decay control that lets you set the decay rate for both the source audio and the audio passing through the resonant filter. Together these help you bolster the low end of your drums.

The Boom knob controls how much low-end enhancement the resonant filter generates. The Bass Meter gives you a visual readout of Boom’s influence on the signal, which is especially handy when you can’t hear it.

The Freq knob sets the frequency at which the low-end enhancer operates. Force To Note lets you pitch the low-end enhancer by snapping its frequency to the nearest MIDI note’s value.

The Decay control governs how fast the low frequencies decay. With the Boom amount at 0%, the decay acts on the source (post-drive and distortion) signal alone. Once the “Boom Level” is pushed past 0%, the decay applies to both the source and processed signals.

You can monitor the low-frequency enhancer’s output in isolation by switching on Boom Audition through the headphone icon.

#### 28.12.0.3 Output

The balance between the processed signal and the dry signal is set by the Dry/Wet control.

How much gain gets added to the processed signal is determined by the Output Gain slider.

### 28.13 Dynamic Tube

The Dynamic Tube Effect.

The Dynamic Tube effect imbues sounds with the quirks of tube saturation. A built-in envelope follower produces dynamic shifts in tone that track the input signal’s level.

A trio of tube models — A, B and C — deliver a spread of distortion behaviors drawn from genuine amplifier tubes. With Bias kept low, Tube A stays clean, but it springs to life once the input signal climbs past a given threshold, generating bright harmonics. Tube C is a thoroughly low-grade tube amp that distorts constantly. Tube B sits in the middle ground between those two extremes.

The Tone control determines how the distortions are distributed across the spectrum, steering them up into the higher registers or down through the midrange and lower.

How much signal feeds the tube is set by the Drive control; more Drive produces a grittier result. The tube’s intensity rides on the Bias dial, which drives the signal into the prized territory of nonlinear distortion. At very large Bias settings, the signal genuinely begins to disintegrate.

An envelope follower, governed by the Envelope knob, can modulate the Bias parameter either upward or downward. The deeper the envelope’s reach, the more the input signal’s level sways the Bias point. Negative Envelope settings produce expansion by easing distortion on loud passages, whereas positive settings make loud material grittier.

Attack and Release are the envelope traits that set how rapidly the envelope responds to level changes at the input. In combination, they mold the dynamic behavior of the distortions. Keep in mind that with Envelope at zero, neither one does anything.

Trim or lift the device’s final output level using the Output dial.

You can cut down on aliasing by switching on Hi-Quality mode, found through the context menu in the device title bar. Doing so refines the audio quality, especially on high-frequency content, though it brings a modest rise in CPU usage.

### 28.14 Echo

The Echo Effect.

Echo is a modulation delay effect that lets you assign the delay time across two separate delay lines, all while handing you control over envelope and filter modulation.

The Channel Mode buttons give you a choice among three modes: Stereo, Ping Pong and Mid/Side.

The Left and Right delay line controls set the delay time, expressed either in beat divisions or in milliseconds based on how the Sync switch is set. Keep in mind that with the Mid/Side channel mode active, the Left and Right delay line controls give way to Mid and Side knobs.

The Sync Mode choosers let you pick from any of these beat-synced options: Notes, Triplet, Dotted and 16th. Bear in mind that the changes from switching between Sync Modes are only heard while the Sync switch sits in the Sync position.

With Stereo Link active, altering either channel’s delay line control, Sync switch or Sync Mode setting carries the change across to both sides.

Adjusting the Delay Offset sliders trims or lengthens the delay time by small fractions, which creates the ”swing” timing feel associated with drum machines. Note that even with Stereo Link active, the Delay Offset remains separately adjustable for each of the two delay lines.

The Input knob governs how much gain is applied to the dry signal. Hit the “D” button to add distortion to that dry signal.

The Feedback parameter sets how much of each channel’s output is routed back into the delay lines’ inputs. Pressing the “Ø“ button flips the polarity of each channel’s output before it’s fed back into the inputs.

### 28.14.1 Echo Tab

A visual readout and control surface for the delay lines and filter parameters is provided by the Echo tab.

Echo’s Tunnel Visualization.

The circular rings of the Echo Tunnel stand for the individual repeats, moving inward from the tunnel’s outer edge toward its center. How far apart the rings sit reflects the gap in time between repeats, and the white dots at the center make up a fixed 1/8th note grid that serves as a reference. You can set the delay times per delay line by clicking and dragging within the display.

Echo’s Filter.

The Filter toggle switches on both a high-pass and a low-pass filter. The HP slider sets the cutoff of the high-pass filter while the Res slider beside it sets that high-pass filter’s resonance. The LP slider sets the cutoff of the low-pass filter, and the Res slider over on the right lets you set the low-pass filter’s resonance.

Visualizing the filter curves is made possible by the Filter Display. Toggle the Filter Display on or off with the triangular toggle button. You can likewise tweak the filter parameters by clicking and dragging either of the filter dots inside the Filter Display.

### 28.14.2 Modulation Tab

The Modulation tab in Echo holds an LFO that modulates both filter frequency and delay time, together with an envelope follower that can be mixed in with the LFO.

Echo’s Modulation Tab.

There are six modulation waveforms to pick from, namely sine, triangle, sawtooth up, sawtooth down, square, and noise. Whichever waveform you select shows up in the display, which you can drag to set the modulation frequency.

With Sync turned on, the modulation locks to the song tempo. The Rate slider then lets you set the modulation oscillator’s frequency in beat divisions. With Sync turned off, the Freq slider lets you set the modulation oscillator’s frequency in Hertz.

Phase sets how much offset there is between the left and right channel waveforms. Set to 180°, the two channels end up completely out of phase.

Mod Delay sets how much modulation reaches the delay time. Modulation x4 multiplies the delay time modulation depth fourfold. At short delay times, this yields deep flanging textures.

Mod Filter sets how much modulation is applied to the filter.

Env Mix crossfades between the modulation oscillator and an envelope follower. At 100%, you hear nothing but the envelope’s modulation. At 0%, you hear nothing but the LFO’s modulation.

### 28.14.3 Character Tab

The Character tab in Echo holds parameters that govern dynamics and introduce imperfections into your sound.

Echo’s Character Tab.

Gate switches on a gate at Echo’s input. It silences any signal portions falling beneath its threshold. Threshold sets the level that incoming audio has to surpass before the gate will open. Release sets how much time passes before the gate shuts once the signal has fallen below the threshold.

With Ducking active, the wet signal is scaled back in proportion for as long as an input signal is present. Ducking starts acting on the output once the input level rises past the chosen Threshold. Release sets how long it takes ducking to let go after the input signal drops beneath the threshold.

Once enabled, Noise mixes in noise to mimic the quality of vintage gear. You can set the Amount of noise blended in, and Morph among different noise types.

Once enabled, Wobble layers in an erratic modulation of the delay time to imitate tape delays. You can set the Amount of wobble blended in, and Morph among different types of wobble modulation.

Repitch produces a pitch shift as the delay time is changed, much like how hardware delay units behave. With Repitch off, altering the delay time instead crossfades between the old and the new delay times.

Keep in mind that to conserve CPU, the Echo device powers down no sooner than eight seconds after its input goes silent. That said, Echo won’t power down whenever both the Noise and Gate parameters are on.

### 28.14.4 Global Controls

The Reverb knob sets how much reverb is mixed in, and the Reverb Location chooser dictates where in the processing chain the reverb sits: pre delay, post delay, or inside the feedback loop. The Decay slider lets you stretch or trim the reverb tail.

The Stereo control sets how wide the wet signal’s stereo image is. A value of 0% gives a mono signal, while anything above 100% produces a broadened stereo spread.

The Output determines how much gain is applied to the processed signal. The balance between the processed and dry signals is governed by the Dry/Wet control. Set it to 100 percent whenever Echo runs on a return track. The Dry/Wet parameter’s context menu lets you switch Equal-Loudness on or off. With it active, a 50/50 blend will come across as equally loud for most signals.

### 28.15 EQ Eight

The EQ Eight Effect.

The EQ Eight effect is an equalizer that offers as many as eight parametric filters for each input channel, handy for reshaping a sound’s timbre.

You can run the input signal through any of three modes: Stereo, L/R and M/S. Stereo mode applies one shared curve so that both channels of a stereo input are filtered identically. In L/R mode, each of a stereo input’s left and right channels gets its own independently tweakable filter curve; M/S mode (Mid/Side) offers the equivalent for material captured with M/S encoding. Across every mode, the output’s frequency spectrum appears behind the filter curves whenever the Analyze switch is enabled.

In the L/R and M/S modes, both curves show at once for reference, though only the currently active channel can be edited. The Edit switch shows which channel is active and serves to flip between the two curves.

Every filter comes with a chooser letting you select from among eight responses. Reading the choosers top to bottom, they are:

- 48 or 12 dB/octave Low cut (removes anything beneath the chosen frequency);
- Low shelf (boosts or cuts frequencies lower than the specified frequency);
- Peak (boosts or cuts over a range of frequencies);
- Notch (sharply cuts frequencies within a narrow range);
- High shelf (boosts or cuts frequencies higher than the specified frequency);
- 12 or 48 dB/octave High cut (removes anything over the chosen frequency).

Each filter band carries its own activator switch beneath the chooser for switching it on or off. Disable any bands you aren’t using to conserve CPU power. For genuinely extreme filtering, apply identical parameters across two or more filters.

You shape the filter curve by clicking and dragging the filter dots within the display. Drag a box around several filter dots to move them all at once, using either the mouse or your computer keyboard’s arrow keys. Moving horizontally changes the filter frequency, whereas moving vertically changes the filter band’s gain. To set the filter Q (otherwise known as resonance or bandwidth), keep the Alt (Win) / Option (Mac) modifier held down as you drag the mouse. Bear in mind that gain isn’t adjustable for the low cut, notch and high cut filters. In those modes, dragging vertically sets the filter Q instead.

For an even clearer view, the display’s location can be moved back and forth — from the device chain over to Live’s main window — using the button found within EQ Eight’s title bar. With this larger view in use, every one of the eight filters can be edited at the same time in the Device View.

EQ Eight’s Controls With the Display Expanded.

EQ Eight shows its output spectrum in the display by default. Should you rather work strictly “by ear,” you can switch off the Analyze button to hide the spectrum view.

When Adaptive Q is on, the Q amount grows as the level of boost or cut grows. The result is a steadier output volume, modeled on the way vintage analog EQs behave.

For a momentary solo of a single filter, switch on Audition mode via the headphone icon. While in Audition mode, clicking and holding a filter dot lets you listen to just that filter’s contribution to the output.

You can additionally pick a band for editing by clicking close to its number and then changing parameter values via the Freq, Gain and Q dials (or by typing values into the number fields beneath each dial).

Because boosting raises levels while cutting lowers them, use the global Gain slider to dial in the loudest output possible without introducing distortion.

The Scale field adjusts the gain across every filter that supports gain (all but low cut, notch and high cut).

#### 28.15.0.1 Context Menu Options for EQ Eight

A handful of EQ Eight’s controls can only be found through the device title bar’s context menu. They are:

- Oversampling - turning this on makes EQ Eight run its internal processing at twice the present sample rate, yielding smoother filter behavior when working on high frequencies. CPU usage rises slightly when Oversampling is on.

### 28.16 EQ Three

The EQ Three Effect.

Anyone who has worked with a decent DJ mixer will recognize this: an EQ that lets you independently set the level of the low, mid and high frequencies.

The gain controls let you set each band anywhere from -infinite dB up to +6 dB. That makes it possible to fully strip out, say, the bass drum or bassline of a track while keeping the rest of the frequencies intact.

You can also switch each band on or off via the On/Off buttons sitting beneath the gain controls. Those buttons come in especially handy when mapped to computer keys.

EQ Three offers a visual cue for whether a signal is present in each frequency band through three LEDs. Even with a band switched off, you can still spot whether anything is happening in it. The LEDs’ internal threshold is fixed at -24 dB.

Two crossover controls, FreqLo and FreqHi, set the frequency span of each band. With FreqLo at 500 Hz and FreqHi at 2000 Hz, the low band spans 0 Hz to 500 Hz, the mid band spans 500 Hz to 2000 Hz, and the high band runs from 2000 Hz on up to whatever ceiling your soundcard or sample rate allows.

The 24 dB/48 dB switch is a particularly significant control. It governs how steeply the filters cut the signal at the crossover frequency. Choosing the higher setting gives more aggressive filtering but demands more CPU.

Note: The filters inside this device are voiced to act less like a clean digital filter and more like a robust, capable analog filter cascade. In particular, the 48 dB Mode doesn’t reach a perfectly linear transfer quality, so a touch of coloration enters the input signal even with every control parked at 0.00 dB. That’s normal for a filter of this sort and forms part of what gives EQ Three its distinctive sound. Should you require more linear behavior, opt for 24 dB Mode or turn to the EQ Eight.

### 28.17 Erosion

The Erosion Effect.

Erosion applies digital degradation to the input signal by modulating a brief delay with a mix of a sine wave and filtered noise. The outcome can range from noisy artifacts all the way to distortions reminiscent of downsampling.

During playback the input signal’s frequency spectrum appears in the display, accompanied by a visual depiction of the modulation. That display doubles as an X-Y controller you can use to set the Freq and Amount controls. Drag horizontally along the X-axis to alter the sine wave frequency and the noise filter’s center frequency. Drag vertically along the Y-axis to govern the modulation amount. Holding Alt (Win) / Option (Mac) instead lets you set the filter width of the noise modulation on the Y-axis. Note that the filter width does nothing when only sinusoidal modulation is in use.

Noise Blend sets how the sinusoidal and noise modulation carriers get mixed. At 0%, the input signal is modulated by a sine wave alone, whereas at 100%, only noise does the modulating. The sine wave and noise icons under the display shift in brightness as you change the blend, signaling which modulation carrier dominates. Within the display, the sinusoidal modulation appears as a solid vertical line while the noise modulation appears as horizontal dotted lines.

The Filter Width control sets the bandwidth of the noise filter. Smaller values yield a tighter frequency range, whereas larger values stretch it over a broader slice of the spectrum. Note that with Noise Blend at 0%, the Filter Width control is grayed out, since it does nothing to the sinusoidal modulation.

The Stereo Width control lets you shift the modulation source from mono (0.0%) toward stereo (100%). Larger values introduce a gentle stereo widening to the modulation.

Any Sets built before 12.4 containing Erosion will open the older form of the device, which now goes by Erosion Legacy.

### 28.18 External Audio Effect

The External Audio Effect.

The External Audio Effect stands somewhat apart from Live’s other effect devices. Rather than processing audio on its own, it lets you bring _external_ (hardware) effects processors into a track’s device chain.

The Audio To chooser picks which outputs on your computer’s audio hardware feed your external device, while the Audio From chooser picks which inputs carry the processed signal back into Live. Just as with the track inputs and outputs, which inputs and outputs are available hinges on the Audio Settings, reachable through the ”Configure…” option at the foot of each chooser.

Each chooser has a Peak level indicator below it that reports the highest audio level reached. Click the indicators to clear them.

The Gain knobs beside the choosers govern the levels leaving and re-entering Live. Set these carefully to keep from clipping, both inside your external hardware and as the audio returns to your computer.

The balance between the processed and dry signals is set by the Dry/Wet control. Take it to 100 percent whenever you use the External Audio Effect on a return track.

The Invert button reverses the phase of the processed signal as it comes back into Live.

Because hardware effects add latency that Live has no way to detect on its own, you can offset any delays by hand using the Hardware Latency slider. The button beside that slider lets you express your latency compensation amount in either milliseconds or samples. When your external device links to Live through a digital connection, set your latency in samples, which guarantees the sample count you enter stays put even after a sample rate change. When your external device links to Live through an analog connection, set your latency in milliseconds, which guarantees the time amount you enter stays put after a sample rate change. Keep in mind that working in samples affords finer control, so even with analog devices you might choose to ”fine tune” your latency in samples to reach the lowest achievable latency. Just remember to flip back to milliseconds before you change your sample rate.

Note: Should the [Delay Compensation](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#device-delay-compensation) option sit unchecked within the Options menu, then the Hardware Latency slider becomes unavailable.

For step-by-step guidance on dialing in accurate latency compensation for your hardware, please consult the [Driver Error Compensation FAQ article](https://help.ableton.com/hc/en-us/articles/115000234830-Driver-Error-Compensation-FAQ) in the Knowledge Base.

### 28.19 Filter Delay

The Filter Delay Effect.
