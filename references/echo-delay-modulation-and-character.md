# Echo Delay Modulation And Character

Open when you need guidance on Echo Delay Modulation And Character in Ableton Live.

Context: [Echo](delay-drum-drive-and-eq-routes.md#2814-echo).

<a id="source-28141-echo-tab"></a>
### 28.14.1 Echo Tab

A visual readout and control surface for the delay lines and filter parameters is provided by the Echo tab.

Echo’s Tunnel Visualization.

The circular rings of the Echo Tunnel stand for the individual repeats, moving inward from the tunnel’s outer edge toward its center. How far apart the rings sit reflects the gap in time between repeats, and the white dots at the center make up a fixed 1/8th note grid that serves as a reference. You can set the delay times per delay line by clicking and dragging within the display.

Echo’s Filter.

The Filter toggle switches on both a high-pass and a low-pass filter. The HP slider sets the cutoff of the high-pass filter while the Res slider beside it sets that high-pass filter’s resonance. The LP slider sets the cutoff of the low-pass filter, and the Res slider over on the right lets you set the low-pass filter’s resonance.

Visualizing the filter curves is made possible by the Filter Display. Toggle the Filter Display on or off with the triangular toggle button. You can likewise tweak the filter parameters by clicking and dragging either of the filter dots inside the Filter Display.

<a id="source-28142-modulation-tab"></a>
### 28.14.2 Modulation Tab

The Modulation tab in Echo holds an LFO that modulates both filter frequency and delay time, together with an envelope follower that can be mixed in with the LFO.

Echo’s Modulation Tab.

There are six modulation waveforms to pick from, namely sine, triangle, sawtooth up, sawtooth down, square, and noise. Whichever waveform you select shows up in the display, which you can drag to set the modulation frequency.

With Sync turned on, the modulation locks to the song tempo. The Rate slider then lets you set the modulation oscillator’s frequency in beat divisions. With Sync turned off, the Freq slider lets you set the modulation oscillator’s frequency in Hertz.

Phase sets how much offset there is between the left and right channel waveforms. Set to 180°, the two channels end up completely out of phase.

Mod Delay sets how much modulation reaches the delay time. Modulation x4 multiplies the delay time modulation depth fourfold. At short delay times, this yields deep flanging textures.

Mod Filter sets how much modulation is applied to the filter.

Env Mix crossfades between the modulation oscillator and an envelope follower. At 100%, you hear nothing but the envelope’s modulation. At 0%, you hear nothing but the LFO’s modulation.

<a id="source-28143-character-tab"></a>
### 28.14.3 Character Tab

The Character tab in Echo holds parameters that govern dynamics and introduce imperfections into your sound.

Echo’s Character Tab.

Gate switches on a gate at Echo’s input. It silences any signal portions falling beneath its threshold. Threshold sets the level that incoming audio has to surpass before the gate will open. Release sets how much time passes before the gate shuts once the signal has fallen below the threshold.

With Ducking active, the wet signal is scaled back in proportion for as long as an input signal is present. Ducking starts acting on the output once the input level rises past the chosen Threshold. Release sets how long it takes ducking to let go after the input signal drops beneath the threshold.

Once enabled, Noise mixes in noise to mimic the quality of vintage gear. You can set the Amount of noise blended in, and Morph among different noise types.

Once enabled, Wobble layers in an erratic modulation of the delay time to imitate tape delays. You can set the Amount of wobble blended in, and Morph among different types of wobble modulation.

Repitch produces a pitch shift as the delay time is changed, much like how hardware delay units behave. With Repitch off, altering the delay time instead crossfades between the old and the new delay times.

Keep in mind that to conserve CPU, the Echo device powers down no sooner than eight seconds after its input goes silent. That said, Echo won’t power down whenever both the Noise and Gate parameters are on.

<a id="source-28144-global-controls"></a>
### 28.14.4 Global Controls

The Reverb knob sets how much reverb is mixed in, and the Reverb Location chooser dictates where in the processing chain the reverb sits: pre delay, post delay, or inside the feedback loop. The Decay slider lets you stretch or trim the reverb tail.

The Stereo control sets how wide the wet signal’s stereo image is. A value of 0% gives a mono signal, while anything above 100% produces a broadened stereo spread.

The Output determines how much gain is applied to the processed signal. The balance between the processed and dry signals is governed by the Dry/Wet control. Set it to 100 percent whenever Echo runs on a return track. The Dry/Wet parameter’s context menu lets you switch Equal-Loudness on or off. With it active, a 50/50 blend will come across as equally loud for most signals.
