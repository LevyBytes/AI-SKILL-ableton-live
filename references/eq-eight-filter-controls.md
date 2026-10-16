# EQ Eight Filter Controls

Open when you need guidance on EQ Eight Filter Controls in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2815-eq-eight"></a>
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
