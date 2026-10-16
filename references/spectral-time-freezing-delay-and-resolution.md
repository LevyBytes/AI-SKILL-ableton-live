# Spectral Time Freezing Delay And Resolution

Open when you need guidance on Spectral Time Freezing Delay And Resolution in Ableton Live.

Context: [Spectral Time](spectral-analysis-utility-and-vocoder-routes.md#2837-spectral-time).

<a id="source-28371-freezer-section"></a>
### 28.37.1 Freezer Section

Spectral Time’s Freezer Section.

Whichever of the Manual/Retrigger Mode buttons is engaged governs how the Freezer section fires the freeze and which timing traits of the captured audio get shaped. Keep in mind that, in either mode, the Freeze button must also be engaged for anything to happen.

Under Manual mode, a click on the Freeze button captures the audio. The Fade In and Fade Out duration of that captured signal is also adjustable in milliseconds.

Retrigger mode hands you extra controls for tightening the timing of the frozen audio, which it can capture on its own at each transient (onset) or on a steady schedule.

With Onsets mode, the audio freezes once a transient shows up in the signal. Tune how readily onsets are caught using the Sensitivity knob — it peaks at 100% and bottoms out at 0%.

Sync mode captures the audio on a steady schedule governed by the Interval control. Flipping the Freezer Time Unit buttons lets the Interval control read in either milliseconds or beat-time values.

Across both Onsets and Sync modes, the Freezer Fade Shape buttons switch among two fade shapes on offer: Crossfade and Envelope. Each shape carries its own controls dictating how a fresh freeze fades in and back out.

With the Crossfade shape chosen, the incoming freeze rises while the previous freeze (or dry signal) drops away. Its length comes from the X-Fade control, which precisely sets the time in milliseconds during which a new freeze rises, expressed as a portion of the sync interval defined by the Interval control.

With the Envelope shape chosen, a fresh freeze fades up and down following the millisecond durations entered in the Fade In and Fade Out parameters. Here, as many as eight freezes can pile up simultaneously, one over the next.

<a id="source-28372-delay-section"></a>
### 28.37.2 Delay Section

Spectral Time’s Delay Section.

Spectral Time’s Delay section switches on or off via the Delay toggle button and lets you spawn delayed copies of the spectral data. Whenever the Freezer section is running, the Freezer’s output feeds straight into the Delay section.

How long the spectral delay lines wait is governed by the Time parameter. Which kind of value appears depends on the unit type picked in the “Mode” drop-down chooser:

- Time mode adjusts the delay time in milliseconds.
- Notes adjusts delay time in beat divisions.
- 16th, 16th Triplet, and 16th Dotted peg the delay to a count of whichever 16th notes variety you picked.

Feedback governs how much of the output returns to the delay input. Raising it makes the signal’s echoes more pronounced.

Shift moves the frequency of the delayed copies. Every following delay gets nudged higher or lower by the chosen frequency amount.

Stereo scales the spread of the Tilt and Spray controls.

Balance between the dry and delayed signals is handled by the Dry/Wet control. Bear in mind it touches only the device’s Delay section.

Tilt tilts the delay timing across frequencies. A positive setting holds high frequencies back more than low ones, whereas a negative setting holds low frequencies back more than high ones.

Spray scatters the delay timing for various frequencies at random inside the supplied time span.

Mask confines the reach of the Tilt and Spray controls to either the high or the low end. Positive settings restrict the action to high frequencies, and negative settings restrict it to low frequencies.

<a id="source-28373-resolution-section"></a>
### 28.37.3 Resolution Section

Spectral Time’s Resolution Control.

Tucked into the spectrogram display’s top-right corner is the Resolution control, which dictates the resolution applied when processing the incoming signal. Dropping it down trims total latency but sacrifices precision and fidelity. Because raising it adds to overall latency, lowering the Resolution while tracking is often worthwhile.

<a id="source-28374-global-controls"></a>
### 28.37.4 Global Controls

Spectral Time’s Global Controls.

Input Send trims the gain of the signal coming in.

A pair of radio buttons, Frz > Dly and Dly > Frz, flip the order in which the effects run.

The overall Dry/Wet control balances the dry signal against the processed one. Push it to 100% whenever Spectral Time sits on a return track.
