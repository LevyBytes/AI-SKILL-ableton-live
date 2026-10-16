# Corpus MIDI Sidechain

Open when you need guidance on Corpus MIDI Sidechain in Ableton Live.

Context: [Corpus](compressor-corpus-and-delay-routes.md#2810-corpus).

<a id="source-28105-sidechain-parameters"></a>
### 28.10.5 Sidechain Parameters

Corpus’s Sidechain Parameters.

You can MIDI-modulate the resonance’s frequency and/or decay rate by switching on the Frequency and/or Off Decay switches within the Sidechain section. Reach the Sidechain parameters by toggling the button on Corpus’s title bar. That button glows whenever the sidechain is running.

From the MIDI From choosers you pick the MIDI track and the tapping point that supplies the MIDI note information.

Switch Frequency on and the incoming MIDI note dictates the resonance’s tuning. Should several notes sound at once, the Last/Low switch decides whether priority falls to the last note or the lowest one. The Transpose and Fine knobs over in the [Resonator](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#resonator-parameters) section provide coarse and fine offset for the MIDI-modulated tuning. PB Range fixes how many semitones the pitch bend modulation spans.

Turn Frequency off and the Tune control in the Resonator section sets the resonance’s base frequency in Hertz. Below it you’ll see the matching MIDI note number plus the fine-tuning offset in cents.

Switching on Off Decay makes MIDI Note Off messages silence the resonance. How strongly those Note Off messages cut the resonance is governed by the slider beneath the switch. At 0% the Note Offs are disregarded, and decay time rests solely on the Decay parameter value, which you can change with the X-Y controller or the Decay slider. That mirrors the behavior of actual mallet instruments like marimbas and glockenspiels. At 100% the resonance stops the instant a Note Off arrives, no matter the Decay time.
