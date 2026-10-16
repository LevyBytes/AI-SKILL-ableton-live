# Roar Modulation Feedback And Global Controls

Open when you need guidance on Roar Modulation Feedback And Global Controls in Ableton Live.

Context: [Roar](redux-resonators-reverb-and-roar-routes.md#2833-roar).

<a id="source-28333-modulation-section"></a>
### 28.33.3 Modulation Section

Clicking the toggle in the Modulation panel reveals Roar’s modulation parameters and opens up the Mod Sources and Matrix tabs.

Roar’s Modulation Toggle.Roar’s Modulation Section.

Four modulation sources sit in the Mod Sources tab: _LFO 1_, _LFO 2_, _Env_ (Envelope), and _Noise_. Every one of these sources arrives with its own signal-visualizing display plus its own dedicated set of parameters.

Each LFO offers a pick of five waveforms: sine, triangle, square, up, or down.

Through the Mode chooser you can put the LFO rate into Free, Synced, Triplet, Dotted, or Sixteenth mode. The Rate slider then sets that rate, in Hertz under Free mode or as tempo-synced beat divisions in the rest. You can dial the Morph control by hand or modulate it to further shape the LFO. Adding smoothing to the LFO signal is handled by the Smooth control, which helps tame abrupt jumps during modulation.

Drawing on Roar’s input, the envelope follower in the Env tab produces a modulation signal. The tab’s parameters let you tune how that follower reacts to the incoming signal.

How fast the envelope tracks the input is shaped by the Attack and Release controls. The Envelope Hold toggle also governs the move from attack into release: switch it on and the envelope runs its full attack phase before the release phase begins.

Sensitivity and strength of the envelope are set by the Threshold and Gain controls, while Frequency and Width pin down a particular frequency band for the signal feeding the envelope follower.

Switch on the Envelope Input Listen toggle to monitor only the input signal.

Within Roar’s Modulation Matrix, the envelope follower really shines as a source. Point it at a snare in a drum loop, for instance, and let it drive Roar’s Dry/Wet balance or Shaper Amount on every snare hit.

Four noise flavors live in the Noise modulation source: Simplex, Wander, S & H, and Brown. Like Roar’s LFO curves, noise curves can run in Hertz or tempo-synced, and they accept smoothing too.

Both Simplex and Wander put out smoothed random signals, each relying on a different interpolation algorithm to give the signal its own dynamics. Simplex draws on interrate modulation, so its value intervals come out more erratic than Wander’s. Such noise types are great for sneaking small, random, organic-feeling motion into Roar’s output, especially at low rates.

S & H (Sample and Hold) holds a random value steady, then jumps to a fresh random value on an interval set by the Noise Rate. It’s handy for building stepped random modulation in Roar’s output.

Brown delivers low-pass filtered white noise, useful for laying down a steady noise floor or sprinkling crackle and hiss across Roar’s output.

Through the Matrix tab you wire modulation sources to modulation targets inside the device. With the Matrix tab open, clicking any parameter marks it as a target. The sources run along the horizontal axis and the targets down the vertical one. Drag a cell up or down to set the modulation between two parameters.

Drag the Global Modulation Amount slider up or down to raise or lower how much modulation is applied across the board. Hitting the X button wipes out every modulation the Modulation Matrix has applied.

You can also expand the Modulation Matrix from the toggle in the device header. Expanded, the device shows all its gain stages together, along with the full set of sources and targets in the Modulation Matrix.

Roar’s Expanded Matrix.

Beyond the visualization displays, LEDs in the Modulation column also flag modulation signals. Every LED takes on a color tied to a particular modulation source. That lets you tell at a glance whether a source is active, and get a feel for its setup, without opening the Modulation Matrix.

<a id="source-28334-feedback-section"></a>
### 28.33.4 Feedback Section

Roar’s Feedback Section.

Among Roar’s standout traits is the Feedback section. Routing Roar’s signal back through itself layers in fresh ringing, otherworldly tones and textures.

Five feedback modes are available from the Feedback Mode drop-down: Time, Synced, Triplet, Dotted, and Note. Pick Synced or Time to run Roar’s Feedback as a delay. Choose Note to pin the feedback’s ring to a chosen pitch.

How much signal loops back into Roar’s input is set by the Feedback Amount knob. Since a compressor sits inside Roar’s feedback loop, loud material momentarily pulls the generated feedback down as the compressor applies gain reduction.

Switch the Feedback Invert toggle on and Roar’s feedback signal has its phase flipped. When that inverted signal meets the original, the resulting phase cancelation opens up yet another avenue to explore in Roar’s signal path.

With the Feedback Gate toggle engaged, Roar’s feedback fades away on its own once the device stops receiving an input. Leave it off and the feedback carries on without end.

The center frequency of the band-pass filter that treats Roar’s feedback is set with the Feedback Filter Frequency slider, while the Feedback Filter Width slider sets how wide that filter’s band is.

<a id="source-28335-global-section"></a>
### 28.33.5 Global Section

Roar’s Global Section.

How much compression lands on the output — and therefore on whatever loops back into Roar — is set by the Compression Amount knob.

<a id="source-live-audio-effect-reference-part-9"></a>

Activating the Compressor Sidechain HP Filter toggle routes a high-pass filter onto the detection signal that feeds the compressor’s sidechain. The benefit here is reducing how much gain reduction occurs when the compressor reacts to low frequency content.

Positioned ahead of a hard clipping stage that then passes into the Dry/Wet stage, the Output Gain knob determines the output level of the wet signal. Reach for this parameter whenever you need to offset level shifts caused by the Drive or Shaper Amount knobs.

Use the Dry/Wet slider to set how the dry and wet portions of Roar’s output are balanced against each other.
