# Impulse Sample Shaping And Outputs

Open when you need guidance on Impulse Sample Shaping And Outputs in Ableton Live.

Context: [Impulse](drift-drums-electric-and-external-routes.md#307-impulse).

<a id="source-3072-start-transpose-and-stretch"></a>
### 30.7.2 Start, Transpose and Stretch

The Start control sets the point at which Impulse starts playing a sample, and you can push it as far as 100 ms beyond where the sample truly begins. The Transp (Transpose) control shifts the sample’s transposition across a range of +/- 48 semitones, and you can drive it with the velocity of incoming notes or with a random value, both configured in the relevant fields.

The Stretch control runs from -100 to 100 percent. With negative values the sample contracts, and with positive ones it lengthens. You get a choice of two stretching algorithms here: Mode A suits low material such as toms or bass, whereas Mode B works better for high material like cymbals. MIDI note velocity can also drive the Stretch value.

<a id="source-3073-filter"></a>
### 30.7.3 Filter

The Filter section supplies a wide selection of filter types, and each one stamps a distinct sonic flavor onto the sample by stripping away particular frequencies. Where along the harmonic spectrum the filter takes effect is governed by the Frequency control, while the Resonance control lifts the frequencies sitting close to that point. A random value or MIDI note velocity can drive Filter Frequency.

<a id="source-3074-saturator-and-envelope"></a>
### 30.7.4 Saturator and Envelope

The Saturator lends the sample a thicker, warmer, more analog quality, and you can toggle it on or off whenever you like. Boosting the signal and introducing distortion is the job of the Drive control. As a side effect, this tends to make most signals considerably louder, so you’ll generally want to offset it by pulling down the sample’s volume control. Pushing Drive to extremes on low-pitched material yields those classic, overdriven analog synth drum tones.

To shape the envelope, use the Decay control, whose ceiling is 10.0 seconds. Two decay modes ship with Impulse: Trigger Mode lets the sample decay alongside the note, whereas Gate Mode holds the envelope until a Note Off message arrives before it starts decaying. That latter mode comes in handy whenever you want decay lengths to vary, which is exactly what hi-hat cymbal sounds call for.

<a id="source-3075-pan-and-volume"></a>
### 30.7.5 Pan and Volume

Every sample comes with Volume and Pan controls, governing amplitude and stereo placement respectively. You can modulate them both: Pan responds to velocity and a random value, while Volume responds to velocity alone.

<a id="source-3076-global-controls"></a>
### 30.7.6 Global Controls

Sitting to the right of the sample slots, these parameters act as global controls covering every sample under Impulse’s control. The instrument’s overall level is set by Volume, while Transp shifts the transposition across all samples. Time-stretching and decay for the whole set of samples fall under the Time control, which lets you morph between short and stretched drum sounds.

<a id="source-3077-individual-outputs"></a>
### 30.7.7 Individual Outputs

Drop a fresh instance of Impulse onto a track and its signal blends in with the other instruments and effects that feed that track’s audio chain. There are plenty of times when it’s preferable to pull the instrument, or just one of its drum samples, off on its own and route that signal to a track of its own. For instructions on doing this with Impulse’s combined signal or with its separate sample slots, consult the [Routing and I/O](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#tapping-individual-outs-from-an-instrument) chapter.
