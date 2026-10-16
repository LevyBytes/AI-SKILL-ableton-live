# Shifter Tuning Modulation And Sidechain

Open when you need guidance on Shifter Tuning Modulation And Sidechain in Ableton Live.

Context: [Shifter](roar-saturator-shifter-spectral-resonator-routes.md#2835-shifter).

<a id="source-28351-tuning-and-delay-section"></a>
### 28.35.1 Tuning and Delay Section

Shifter’s Tuning and Delay Section.

Depending on the active shift mode (covered in the [Shifter Mode](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#shifter-mode-section) section), the Coarse and Fine knobs move the pitch or the frequency by the amount you dial in.

Switching on the Wide button flips the polarity of the Spread value for the right channel, yielding a stereo effect. In practice, raising the Spread value drives the frequency downward in the right channel and upward in the left. Bear in mind that Wide does nothing when the Spread value sits at 0.

While in Pitch mode, the Window slider controls the size of the window the algorithm employs. Longer window sizes tend to suit low frequency signals, whereas shorter ones tend to favor high frequencies. Tone trims the highs from the delay’s feedback path.

Switching on the Delay button introduces delay time, which the slider control lets you specify either in Hertz or in beat-synced divisions according to the Delay Mode button you pick. How much of the output is routed back into the delay’s input is governed by the Delay Feedback knob.

<a id="source-28352-lfo-section"></a>
### 28.35.2 LFO Section

Shifter’s LFO Section.

Shifter’s LFO gives you a way to modulate both the left and right stereo channels.

Within the LFO waveform display sit the Duty Cycle and Phase/Spin/Width controls. Duty Cycle determines the duty cycle of the LFO waveform. Phase sets the offset separating the left- and right-channel waveforms; at 180° the two LFOs end up exactly out of phase. According to the LFO waveform in use or the Rate parameter, a Spin or Width control may take the place of Phase, as described further on.

Should the Rate parameter (detailed more fully below) be set to beat-synced time divisions, an Offset parameter appears alongside the Phase parameter, nudging the point at which each LFO begins along its waveform.

The LFO drop-down menu holds a number of LFO waveforms to pick from. The first group covers Sine, Triangle, Triangle Analog, Triangle 8, and Triangle 16; the rest are Saw Up, Saw Down, Rectangle, Random, and Random S&H.

The option of Spin in place of Phase is available for these waveforms: Sine, Triangle, and Triangle Analog, together with Triangle 8, Triangle 16, Saw Up, Saw Down, and Rectangle. Spin pushes the two LFO speeds slightly apart from each other.

By contrast, the Random and Random S&H waveforms allow only Phase and Width, respectively. Width controls the Stereo width of the random LFO waveform. At 0%, both the left and right channels share an identical waveform. At 100%, the waveform becomes fully stereo, so a peak on the left lines up with a trough on the right and the reverse as well.

The Rate parameter steers LFO modulation and may be specified in Hertz or locked to the song tempo in meter subdivisions (for example, sixteenth notes). How strongly that LFO modulation hits the incoming signals is set by the Amount parameter.

<a id="source-28353-envelope-follower-section"></a>
### 28.35.3 Envelope Follower Section

Shifter’s Envelope Follower.

Taking the amplitude of an incoming audio signal, Shifter’s envelope follower converts it into a modulation source.

The Envelope Attack governs how fast the envelope follower reacts as input levels climb, and the Envelope Release governs how fast it reacts as those levels fall.

Shifter’s envelope follower is turned on with the Env Fol button. The Amount dials in the strength of the envelope follower’s modulation. You can specify the Amount value in semitones while in Pitch mode, or in Hertz when using the Freq and Ring modes.

<a id="source-28354-shifter-mode-section"></a>
### 28.35.4 Shifter Mode Section

The Shifter Mode Section.

You can choose among three Shifter Mode button switches: Pitch, Freq, and Ring.

In Pitch mode, the incoming audio is shifted up or down by an amount you set in semitones (Coarse tuning) and cents (Fine tuning).

Freq mode displaces the frequencies of the incoming audio up or down by an amount you specify in Hertz. Modest shifts can yield gentle tremolo or phasing, whereas large ones can generate clashing, metallic timbres.

Within Ring mode, the frequency amount you specify in Hertz gets both added to and subtracted from the input.

Drive switches on a distortion effect, with the slider beneath it setting the distortion level. Note: Drive is offered only within Ring mode.

How the dry and processed signals balance out at Shifter’s output is determined by the Dry/Wet knob.

<a id="source-28355-sidechain-parameters"></a>
### 28.35.5 Sidechain Parameters

Shifter’s Sidechain Parameters.

Reach the Sidechain parameters by expanding the Shifter window via the triangle button at the left edge of the title bar. Two Pitch Modes control how the pitch or frequency gets established: Internal and MIDI. Under Internal mode, Shifter’s Coarse and Fine knobs set the pitch or frequency, while under MIDI mode an incoming MIDI note does so.

While in MIDI mode, a drop-down menu appears for picking an external MIDI source. A Glide parameter is also present, setting the time in milliseconds it takes for notes to glide their pitch toward the next incoming pitch. Using the PB slider, you can establish a pitch bend range from 0-24 semitones that determines how MIDI pitch bend messages behave.

<a id="source-28356-shifter-tips"></a>
### 28.35.6 Shifter Tips
