# Corpus Resonance Modulation And Output

Open when you need guidance on Corpus Resonance Modulation And Output in Ableton Live.

Context: [Corpus](compressor-corpus-and-delay-routes.md#2810-corpus).

<a id="source-28101-resonator-parameters"></a>
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

<a id="source-28102-lfo-section"></a>
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

<a id="source-28103-filter-section"></a>
### 28.10.3 Filter Section

Corpus’s Filter Section.

You may route the processed signal through a band-pass filter, switching it on or off with the Filter switch.

The filter’s center frequency is set by the Freq knob, while its bandwidth is set by Bdwidth.

<a id="source-28104-global-parameters"></a>
### 28.10.4 Global Parameters

Corpus’s Global Parameters.

Bleed folds some of the untouched signal back in with the resonated one. Raise it and a greater share of the original comes through. That helps bring back high frequencies, which often get damped once the tuning or quality sit at low settings. The Pipe and Tube resonators turn this parameter off.

Gain lifts or lowers the level of the processed signal. A limiter built into Corpus kicks in by itself whenever the audio runs too hot, signaled by the LED beside the Gain knob.

How the dry input signal balances against the audio routed into Corpus’s processing is set by the Dry/Wet control. Pulling Dry/Wet down won’t silence resonances already ringing out; instead it keeps fresh input signals from being processed.
