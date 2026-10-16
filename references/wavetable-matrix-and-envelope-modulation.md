# Wavetable Matrix And Envelope Modulation

Open when you need guidance on Wavetable Matrix And Envelope Modulation in Ableton Live.

Context: [Wavetable](tension-and-wavetable-routes.md#3013-wavetable).

<a id="source-30135-matrix-tab"></a>
### 30.13.5 Matrix Tab

By way of the Modulation Matrix you route modulation coming from Envelopes and LFOs — collectively the “internal modulation sources” — onto the instrument’s parameters, otherwise called the “modulation targets.”

Wavetable’s Matrix Tab.

Across the grid, modulation sources lie along the horizontal axis and modulation targets along the vertical one. Drag inside the grid to set how much modulation the chosen source sends to the chosen parameter.

Be aware that some parameters act as additive modulation targets while others act as multiplicative ones.

A parameter receives additive modulation according to this formula:

1. The outputs of a parameter’s modulation sources are summed together.
2. The summed modulation value is added to the current parameter value.

With additive modulation the values revolve around 0, where 0 is the “neutral” point. These values may run negative or positive. A source putting out both negative and positive values is a “bipolar” source, whereas one limited to positive values only is a “unipolar” source.

A parameter receives multiplicative modulation according to this formula:

1. The outputs of a parameter’s modulation sources are multiplied together.
2. The multiplied modulation value is multiplied with the current parameter value.

Here the neutral point is 1 and the floor is 0. The Wavetable manual flags multiplicative-modulation parameters wherever they occur.

Clicking a parameter on the instrument drops it into the matrix temporarily. Apply any modulation to it and it sticks around; leave it unmodulated and it vanishes again the moment you click a different parameter. Note as well that the Matrix tab and the MIDI tab draw on the same set of rows.

Clicking any of the modulation source headers sitting above the matrix whisks you straight to that source’s panel over in the Mod Sources tab.

The Time slider rescales the timing of every modulator at once. Negative settings speed up the envelopes and LFOs, positive ones slow them down. Modulating this value with an envelope or LFO won’t touch the modulator doing the assigning, yet that modulator continues to scale toward its other destinations.

Every source feeding the modulation matrix has its combined depth governed by the Amount slider, which itself behaves as a multiplicative modulation destination.

<a id="source-30136-mod-sources-tab"></a>
### 30.13.6 Mod Sources Tab

On the Mod Sources tab you tweak the Envelope and LFO settings, each covered in greater depth below.

Wavetable’s Mod Sources Tab.

Envelopes

The three Wavetable envelopes (Amp, Env 2 and Env 3) respond to Time and Slope parameters, and Env 2 and Env 3 add their own Value controls on top. You can also set the Time, Slope and Value parameters directly by dragging on the envelope display.

Attack is the time taken to climb from the initial value up to the Peak value, and the contour of that segment follows the Attack Slope value.

Decay is the time taken to fall from the Peak value down to the Sustain level, with the segment’s contour set by the Decay Slope value.

Sustain fixes the level held once the Decay stage finishes. The envelope lingers there until a Note Off comes in — unless you’ve chosen Trigger or Loop for the Loop mode, whereupon it presses on to the Release stage the moment that level is reached. Note that this is a multiplicative modulation destination.

Release is the time taken to reach the Final value once a Note Off occurs, the contour of that segment being set by the Release Slope value.

As noted earlier, Wavetable’s envelopes additionally give you parameters for adjusting the slope of each segment. A positive slope makes the envelope race ahead early on and ease off later; a negative slope holds it flat longer before accelerating toward the end. Set the slope to zero for a linear shape, where the envelope advances at a steady rate across the whole segment.

The Initial slider fixes the value the envelope departs from at the moment of triggering. Bear in mind it serves as a multiplicative modulation destination. You won’t find this control on the amp envelope.

The Peak slider fixes the value that caps off the Attack stage and kicks off the Decay stage. The amp envelope omits this control.

The Final slider fixes the value reached when the Release stage ends. Again, the amp envelope has no such control.

Three options await you in the Loop Modes drop-down:

- None keeps the Sustain stage active until a Note Off arrives, and no looping occurs.
- Trigger runs through every segment a single time as soon as a Note On comes in.
- Loop cycles through the whole envelope, skipping any Sustain hold, right up until the voice finishes.
