# Live Audio Effect Reference (part 3)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Whenever a signal climbs past a threshold you choose, a compressor pulls its gain back down. Because the loudest peaks get tamed, additional headroom appears, which lets you raise the level of the whole track. The result is a higher average loudness, and the ear tends to perceive that as a fuller, more forceful sound compared to material left uncompressed.

The Threshold and the compression Ratio rank as the two settings that matter most on any compressor.

Where compression kicks in is governed by the Threshold slider. Anything louder than that point gets pulled down by a degree that the Ratio parameter controls, since Ratio fixes the relationship between input and output. Take a compression ratio of 3 as an example: a 3 dB rise on an input that sits above the threshold yields only a 1 dB rise at the output. Likewise, a 6 dB input rise above the threshold produces just 2 dB more at the output. Set the ratio to 1 and you get no compression at all, whatever the threshold happens to be.

At any instant, the orange Gain Reduction meter reports the current amount of gain being pulled down. Heavier reduction makes the processing more obvious; pushing past roughly 6 dB of gain reduction may hit the loudness you wanted, yet it noticeably reshapes the tone and can wreck the dynamic structure. Once that damage is done, no later stage of production will bring it back. Bear that in mind in particular if you place a compressor, limiter, or loudness-maximizing device on the Main track. Restraint usually pays off in those situations.

Since compression trims the loud parts and frees up headroom, the Output (Out) control lets you push the peaks back up to the top of the available headroom. Output level is displayed on the Output meter. Switch on the Makeup button and Live will adjust the output level for you whenever you change the threshold or ratio.

The blend of processed and unprocessed audio is set by Dry/Wet. Set it to 100% and you hear only the compressed signal; pull it to 0% and the device essentially does nothing.

How smoothly or sharply compression sets in as the signal nears the threshold is shaped by the Knee control. At 0 dB, nothing below the threshold is touched and anything reaching or passing it is compressed in full. Paired with steep ratios, this so-called ”hard knee” response can come across as harsh. Raise the knee toward ”soft” values and compression eases in progressively as the signal approaches the threshold. Picture a 10 dB knee combined with a -20 dB threshold: gentle compression starts around -30 dB and ramps up so that, by -10 dB, the signal is being fully compressed.

Using the switches tucked into the lower corners of the display, you can flip Compressor’s display among several modes:

- The _Collapsed_ view exposes nothing but the core controls.
  Compressor’s Collapsed View.
- The _Transfer Curve_ plots input level across the horizontal axis and output level up the vertical one. It comes in handy for dialing in the Knee parameter, which appears as two dotted lines flanking the threshold.
  Compressor’s Transfer Curve.
- The _Activity_ view draws the incoming signal’s level in light gray. Here the GR and Output switches let you swap between displaying gain reduction in orange and showing the output level in a darker shade of gray. Such views help you picture how the signal evolves moment to moment.
  Compression Activity Display, Showing Input and Output.

By setting how quickly Compressor responds to shifts in the input level, the Attack and Release controls govern its timing behavior, which makes them critical parameters.

Once a signal passes the threshold, Attack governs the time needed to reach full compression, whereas Release governs how long the compressor takes to ease back to its resting state after the signal drops under the threshold. Switch on Auto Release and the release time recalibrates on its own according to the audio coming in.

Giving the attack a modest value (10-50 ms) lets peaks slip through untouched, which preserves dynamics by emphasizing the leading edge of each sound. Should those peaks trigger overloads, shortening the attack can help, though very brief settings drain the ”life” out of the audio and can introduce a faint “buzziness” from distortion. Brief release values can bring on ”pumping” while the compressor wavers over whether or not to clamp down; usually treated as a flaw, this is nonetheless something some engineers deliberately apply to full drum kits for odd ”sucking” textures. Dialing attack and release in carefully really matters when you are compressing rhythmic material. New to compressors? Loop a drum part and experiment for a while with Attack, Release, Threshold and Gain. The process can be a lot of fun!

A compressor has nothing to act on until the input signal actually arrives. Because it also has to impose an attack/release envelope, its response inevitably lands slightly behind the beat. The digital fix is straightforward: hold the incoming signal back by a tiny margin. Compressor provides three Lookahead settings to do this: zero ms, one ms and ten ms. Depending on which you pick, the outcome can sound noticeably different.

Three core operating modes are available on Compressor. Choose Peak and Compressor responds to brief spikes inside a signal. Being sharper and more exact, this mode suits limiting jobs where you must guarantee nothing whatsoever exceeds the threshold you set. Pick RMS and Compressor grows less reactive to fleeting peaks, clamping down only after the level has stayed over the threshold for a marginally longer stretch. Since RMS tracks loudness more like the human ear does, it is generally felt to be more musical. With Expand mode you dial in the expansion ratio between input and output. As an illustration, a 1 to 2 ratio means each 1 dB the input sits above the threshold turns into a 2 dB rise at the output. Set it to 1 to 1 and no expansion takes place. To read more about the different categories of dynamics processing, refer to the [Multiband Dynamics](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#multiband-dynamics) section.

Beyond those modes, Compressor lets you pick between two envelope-follower shapes, giving you extra say over how the device gauges and tracks signal levels. Under linear (Lin) mode, the Attack and Release values alone dictate how fast compression responds. Switch to logarithmic (Log) mode and heavily compressed peaks recover faster than gently compressed passages. The upshot can be smoother, less obtrusive compression than Lin offers. Keep in mind that the Lin/Log switch stays hidden while Compressor is collapsed.

### 28.9.1 Sidechain Parameters

The Compressor Device With Sidechain Section.

In the usual case, the audio being compressed and the source that triggers the compressor are one and the same. Through _sidechaining_, though, you can drive compression on one signal from the level of a different signal or even a particular frequency component. Reach the Sidechain parameters by expanding the Compressor window via the button on its title bar.

Two halves make up the sidechain parameters. The external controls sit on the left side. Switch that part on with the Sidechain button and you can pick any of Live’s [internal routing points](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#internal-routing-points) from the choosers underneath. The chosen source then becomes what triggers the compressor, in place of the audio currently being compressed.

Level of the external sidechain’s input is handled by the Gain knob, and the Dry/Wet knob lets you blend the sidechain with the original signal as the compressor’s trigger. Push Dry/Wet to 100% and only the sidechain source drives the compressor. Drop it to 0% and the sidechain is essentially out of the picture. Bear in mind that turning up the gain does _not_ make the source signal louder in the mix. That sidechain audio merely triggers the compressor; it is never heard on its own.

Keep in mind that automatic Makeup cannot be used together with an external sidechain.

The sidechain EQ controls occupy the right portion of the external section. Switch this part on and the compressor responds to a chosen band of frequencies rather than the whole signal. Those frequencies may live within the compressed signal itself, or — when you pair the EQ with an external sidechain — within the audio of a different track.

Sitting between the external and EQ sections, the headphones button lets you monitor the sidechain input alone while muting the compressor’s output. Because that sidechain audio never reaches the output and only serves to trigger the compressor, this brief monitoring mode makes it far simpler to dial in sidechain parameters and hear exactly what is driving the compressor.

### 28.9.2 Compressor Tips

What follows are a few pointers for getting the most out of Compressor, with special attention to the sidechain features.

#### 28.9.2.1 Mixing a Voiceover

A frequent use of sidechaining is to create what people call ”ducking” effects. Suppose, for instance, that one track holds a voiceover while another holds background music. Because the voiceover should stay the loudest element in the mix, the music has to step aside whenever the narrator talks. You can automate that by placing a Compressor on the music track and choosing the narration track’s output as the external sidechain source.

#### 28.9.2.2 Sidechaining in Dance Music

For dance music producers, sidechaining/ducking is something of a hidden trick, since it lets basslines — or even entire mixes — consistently clear space for the kick drum. Drop a compressor onto the bass (or Main) track, feed it the kick drum’s track as the sidechain input, and you gain a way to tame troublesome low end that could otherwise muddy the kick drum’s attack.

Bringing the sidechain EQ into this approach lets you produce ducking even when all you have is a mixed drum track rather than a kick drum on its own. Here, place the Compressor on whichever track you intend to duck. Next, pick the drum track for the external sidechain source. After that, switch on the sidechain EQ and choose the low-pass filter. Tweak the Frequency and Q settings with care and you ought to be able to pull the kick drum apart from the rest of the drum mix. The sidechain listen mode is handy for fine-tuning the EQ until the settings sit right with you.

It is worth noting that Compressor’s internal algorithms got an overhaul for Live 9, a joint effort with Dr. Joshua D. Reiss, who works at the Centre for Digital Music, Queen Mary University of London.

### 28.10 Corpus

The Corpus Effect.

As an effect, Corpus recreates the acoustic behavior of seven kinds of resonant objects. Built together with Applied Acoustics Systems, Corpus relies on physical-modeling technology to offer a broad set of parameters along with modulation choices.

### 28.10.1 Resonator Parameters

Corpus’s Resonator Parameters.

From the Resonance Type chooser you pick one of seven physically modeled resonant objects:

- Beam recreates how beams of assorted materials and dimensions resonate.
- Marimba is a tailored offshoot of the Beam model that reproduces the distinctive overtone tuning of marimba bars, a quality born from the deep arch carved into the underside of each bar.
- String mimics the tone made by strings of various materials and dimensions.
- Membrane represents a rectangular membrane, like a drum head, whose size and build can be varied.
- Plate reproduces the sound coming from a rectangular plate — a flat surface — across different materials and dimensions.
- Pipe models a cylindrical tube open all the way at one end and adjustably open at the other, which you set with the Opening parameter.
- Tube models a cylindrical tube left fully open at each end.

By cutting back how many overtones get computed, the Resonator Quality chooser balances resonator sound quality against performance. Eco draws the least CPU, whereas High yields richer resonances. The Pipe and Tube resonators ignore this parameter.

How much internal damping the resonator has — and therefore its decay time — is set by the Decay slider.

The Material slider governs how the damping changes across frequencies. Keep it low and low-frequency content rings out longer than high-frequency content, mimicking objects of wood, nylon or rubber. Push it high and the high frequencies linger longer instead, mimicking objects of glass or metal. The Pipe and Tube resonators ignore this parameter.

Only the Pipe and Tube resonators offer the Radius slider, which takes the spot otherwise held by the Material parameter described above. Radius sets the radius of the pipe or tube. Widening the radius lengthens both the decay time and the high-frequency sustain. At especially large sizes, the resonator’s fundamental pitch shifts as well.

You can also drive the Decay and Material/Radius parameters from the X-Y controller.

The amplitude of the assorted frequency components is set by the Bright knob. Crank it up and the higher frequencies grow louder. The Pipe and Tube resonators ignore this parameter.

Pitch of the resonator’s harmonics is shaped by Inharm (Inharmonics). Negative settings squeeze the frequencies together, adding more lower partials. Positive settings spread them apart, adding more upper partials. The Pipe and Tube resonators ignore this parameter.

Available only on the Pipe resonator, Opening sweeps from a closed pipe to an open one. At 0% the pipe is sealed on one side, and at 100% it stands open at both ends.

Offered only for the Membrane and Plate resonators, Ratio sets the proportion of the membrane/plate between its x and y axes.

Where the object gets struck or otherwise excited on the resonator is set by the Hit knob. At 0% the strike lands dead center. Larger values push the excitation point toward the rim. The Pipe and Tube resonators ignore this parameter.

The stereo balance between the left and right resonators is handled by the Width slider. At 0% both resonators feed each side equally for a mono result. At 100% each resonator goes to just one channel.

Where the vibrations are picked up on the left and right resonator is set by the Pos. L and Pos. R controls. At 0% the resonance is sensed at the object’s center. Larger values shift the pickup point toward the rim. The Pipe and Tube resonators ignore these parameters, since they are always sensed at the midpoint of their permanently open end.

Frequency of the resonator in Hertz is set by the Tune knob. Once MIDI Frequency is switched on in Corpus’s Sidechain section, that knob handles the coarse tuning of the MIDI modulation.

When sidechain MIDI Frequency is active, the Fine knob handles fine tuning of MIDI modulation in cents.

The two resonators are detuned against one another by Spread. Positive settings push the left resonator’s pitch up and the right one’s down; negative settings reverse that. At 0% both resonators share the same tuning.

### 28.10.2 LFO Section

Corpus’s LFO Section.

Inside Corpus sits a Low Frequency Oscillator (LFO) for modulating the resonant frequency. How strongly the LFO shifts that frequency is governed by the Amount control.

LFO speed is governed by the Rate control. You may dial it in Hertz or lock it to the song tempo, which makes measured rhythmic modulation possible.

The LFO waveform options are sine — which yields gentle modulations with rounded crests and troughs — plus square, triangle, sawtooth up, sawtooth down, and a pair of noise types (stepped and smooth).

Even though you see just one bank of LFO controls, two LFOs are really at work, one per stereo channel. How those two LFOs relate is defined by the Phase and Spin controls.

Phase holds both LFOs at a matching frequency yet can push their waveforms ”out of phase,” producing stereo movement. Dial it to 180 and the two LFO outputs sit 180 degrees apart, so one peaks exactly as the other bottoms out. Set Phase to 360 or 0 and the pair run together in sync.

Once the LFOs follow the song tempo, an extra Offset knob appears, nudging where the LFO begins along its waveform.

Spin, on offer only while the LFOs run in Hertz mode, detunes the speeds of the two LFOs from one another. Each stereo channel then modulates at its own frequency, governed by the Spin amount.

While the LFOs are in Hertz mode, you select either Phase or Spin through the LFO Stereo mode icons.

The LFO Stereo Mode Icons.

With the noise waveforms, the Phase and Spin controls carry no meaning and leave the sound untouched.

### 28.10.3 Filter Section

Corpus’s Filter Section.

You may route the processed signal through a band-pass filter, switching it on or off with the Filter switch.

The filter’s center frequency is set by the Freq knob, while its bandwidth is set by Bdwidth.

### 28.10.4 Global Parameters

Corpus’s Global Parameters.

Bleed folds some of the untouched signal back in with the resonated one. Raise it and a greater share of the original comes through. That helps bring back high frequencies, which often get damped once the tuning or quality sit at low settings. The Pipe and Tube resonators turn this parameter off.

Gain lifts or lowers the level of the processed signal. A limiter built into Corpus kicks in by itself whenever the audio runs too hot, signaled by the LED beside the Gain knob.

How the dry input signal balances against the audio routed into Corpus’s processing is set by the Dry/Wet control. Pulling Dry/Wet down won’t silence resonances already ringing out; instead it keeps fresh input signals from being processed.

### 28.10.5 Sidechain Parameters

Corpus’s Sidechain Parameters.

You can MIDI-modulate the resonance’s frequency and/or decay rate by switching on the Frequency and/or Off Decay switches within the Sidechain section. Reach the Sidechain parameters by toggling the button on Corpus’s title bar. That button glows whenever the sidechain is running.

From the MIDI From choosers you pick the MIDI track and the tapping point that supplies the MIDI note information.

Switch Frequency on and the incoming MIDI note dictates the resonance’s tuning. Should several notes sound at once, the Last/Low switch decides whether priority falls to the last note or the lowest one. The Transpose and Fine knobs over in the [Resonator](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#resonator-parameters) section provide coarse and fine offset for the MIDI-modulated tuning. PB Range fixes how many semitones the pitch bend modulation spans.

Turn Frequency off and the Tune control in the Resonator section sets the resonance’s base frequency in Hertz. Below it you’ll see the matching MIDI note number plus the fine-tuning offset in cents.

Switching on Off Decay makes MIDI Note Off messages silence the resonance. How strongly those Note Off messages cut the resonance is governed by the slider beneath the switch. At 0% the Note Offs are disregarded, and decay time rests solely on the Decay parameter value, which you can change with the X-Y controller or the Decay slider. That mirrors the behavior of actual mallet instruments like marimbas and glockenspiels. At 100% the resonance stops the instant a Note Off arrives, no matter the Decay time.

### 28.11 Delay

The Delay Effect.

Each stereo channel in Delay gets its own separate delay line, and the device adds a band-pass filter plus LFO modulation features.

You may dial the delay time in tempo-locked beat divisions (Sync) or in milliseconds (Time). The Delay Time Mode toggles let you flip between the two.

Under Sync, the numbered buttons let you set the delay time in sixteenth notes. Pick 4, for instance, and the input is held back by four sixteenth notes, which works out to one beat — a quarter note — of delay. The Offset sliders nudge the sixteenth-note timing by fractional steps. Negative settings tighten the timing so the delay lands a little ahead of the sixteenth-note division, while positive settings loosen it so the delay arrives a touch later. Offset is a good way to fold gentle swing into the delay.

Under Time, you can hold the input back by anything from 1.00 millisecond out to 5.00 seconds.

Switch on the Stereo Link toggle to tie the delay settings of the left and right channels together. With the link active, any change you make to one channel’s delay time carries over to both. Offset still adjusts per channel on its own, even while Stereo Link is on.

How much of each channel’s output gets routed back into that channel’s delay line input is set by the Feedback control. These feedback loops stay separate per channel, so the left channel’s signal never crosses into the right channel and the reverse holds true as well.

Hit the Freeze button and the audio sitting in the device’s buffer at that instant loops forever. Fresh input gets disregarded until you switch Freeze back off.

Ahead of the delay signal sits a band-pass filter you can turn on or off with the Filter toggle. Within the display, drag along the X-axis to move the filter’s center frequency and drag along the Y-axis to set its bandwidth. The Freq and Width sliders adjust these same values too.

An LFO can modulate the delay time and the filter frequency, opening up everything from chorus-style textures to chopped-up glitches.

Out of the box, the full LFO section stays folded away and only the delay-time and filter modulation controls appear under the band-pass display. The LFO Controls toggle unfolds the LFO section to reveal the extra modulation options.

Expanding the LFO Section via the LFO Controls Toggle.Delay’s LFO Modulation Options.

How much LFO modulation reaches the delay time is set by the Delay slider, while the modulation depth for the filter frequency is set by the Filter slider.

The Rate drop-down menu offers these LFO rate modes: Rate, Time, Synced, Triplet, Dotted, and Sixteenth. As playback runs, the LED beside the LFO Controls toggle blinks in step with the active LFO rate.

The Wave drop-down holds these LFO waveform choices: Sine, Triangle, Ramp Up, and Ramp Down, plus Square, S&H (Sample and Hold), or Wander. The Morph slider lets you reshape whichever waveform you chose.

Changing the delay time while Delay is working on audio — during playback, say — can throw sudden shifts into the delayed sound. To control how Delay manages those timing transitions, you can pick among three smoothing modes:

- _Repitch_ shifts the pitch when you alter the delay time, much like vintage tape delay units behave. It is the default mode.
- _Fade_ crossfades from the old delay time to the new one. The effect can resemble granular synthesis, particularly when you move the delay time slowly.
- _Jump_ snaps straight to the new delay time. That can throw audible clicks if you change the delay time while an earlier delay is still ringing out.

Which smoothing mode you select also changes how the LFO modulation of delay time and filter colors the end result. Try tweaking the modulation under each mode to hear the delay’s sound shift.

Switch on the Ping Pong toggle and the delayed signal bounces back and forth across the left and right channels.

The Dry/Wet control sets how the dry and processed signals balance out. If you run Delay on a return track, push this control to 100% so the return track passes along only the processed signal.

### 28.11.1 Context Menu Options for Delay
