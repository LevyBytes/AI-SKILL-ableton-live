# Crossfading Cueing And Track Latency

Open when you need guidance on Crossfading Cueing And Track Latency in Ableton Live.

Context: [Mixing](mixing.md#18-mixing).

<a id="source-185-using-lives-crossfader"></a>
### 18.5 Using Live's Crossfader

A crossfader is part of Live, capable of producing smooth transitions between clips on separate tracks. The crossfader in Live behaves like the crossfader on an ordinary DJ mixer, except it can crossfade not just two tracks but any number of them — the returns included.

The Crossfader.

You can reach the crossfader through the Mixer Controls submenu of the View menu, or through the menu options under the mixer view control in the lower right of Live's window. There are seven different crossfade curves on offer, letting you pick whichever best matches your style. Switch the curve by right-clicking the crossfader and then choosing an entry from the context menu.

Choose from Seven Crossfader Curves.

The table below lays out the power level and response for each crossfader curve.

Crossfader Curve Properties.

Any [continuous MIDI controller](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) (absolute or incremental) can be assigned to the crossfader. Apart from the crossfader's central slider, its extreme left and right positions are individually available for MIDI or keyboard mapping. Two unusual cases apply to remote control of the crossfader:

- A key assigned to one of the three mappable crossfader positions (left, center or right) will switch the crossfader between its extreme left and right positions.
- Assigning to two of the three fields produces a “snapping back“ effect when one assigned key is held and the other is pressed then released.
  Crossfade Assign Buttons.

Two Crossfade Assign buttons, A and B, sit on each track. Relative to the crossfader, a track can be in one of three states:

- With neither Assign button enabled, the crossfader has no effect on the track whatsoever.
- With A enabled, the track plays at full level as long as the crossfader stays in the left half of its range. As the crossfader travels rightward past the center point, the track fades down. With the crossfader all the way right, the track is silenced.
- In the same way, with B enabled, the track's volume changes only as the crossfader travels left past its center point.

It's worth grasping that the Crossfade Assign buttons leave the signal routing untouched; the crossfader simply changes the signal level at the gain stage of each track. A track can still be routed to its own output bus no matter what its crossfade assignment is. In studio terms, picture the crossfader as an on-the-fly VCA group.

As with nearly everything in Live, the moves you make with the crossfader can be [recorded into the Arrangement](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#automation-and-editing-envelopes) for detailed editing afterward. To edit a given track's crossfade assignment, pick “Mixer“ in the Envelope Device chooser and “X-Fade Assign“ in the Control chooser. You can reach the crossfader's automation curve by picking “Mixer“ from the Main track's Device chooser and “Crossfade“ from its Control chooser.

<a id="source-186-soloing-and-cueing"></a>
### 18.6 Soloing and Cueing

Normally, soloing a track just silences all the other tracks (apart from certain cases where tracks are [feeding other tracks](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#internal-routings)). The signal coming from the soloed tracks is heard via their own outputs, keeping each track's pan setting intact. Soloing a clip track keeps any return tracks audible, as long as the Solo in Place option is turned on in the Solo button's context menu. You can also make Solo in Place the default by choosing the entry in the Options menu.

Soloing a return track silences the main output of every other track, while still letting you hear any signals that reach the return through track sends.

Live lets you swap the standard soloing behavior for a cueing behavior that allows you to preview tracks much as you would cue a record on a DJ mixer. With this you can choose clips and tweak effects out of the audience's earshot, before easing tracks into the mix.

To prepare Live for cueing, you need an audio interface offering at least four dedicated outputs (or two dedicated stereo outputs). You'll find the relevant settings on the Main track. Be sure the mixer section and the In/Out controls are showing.

The Cueing-Related Session Mixer Controls.

1. The Main Out chooser picks the output on your interface that will act as the main output.
2. The Cue Out chooser picks the output on your hardware interface that will be used for cueing. It must be set to an output different from the one chosen for Main. Should the outputs you want fail to appear in these choosers, check the Audio Settings.
3. Turn on cueing by flipping the Solo/Cue Mode switch to “Cue.“
4. The Solo switches on the tracks are now swapped for Cue switches bearing headphone icons. Pressing a track's Cue switch routes that track's output signal to the output picked in the Cue Out chooser. Bear in mind that the Track Activator switch on the same track still governs whether that track is heard at the Main output.
5. The Cue Volume control sets the level of the cueing output.

Bear in mind that once cueing is configured and on, audio files you preview in the browser are also heard through the Cue Out.

<a id="source-187-track-delays"></a>
### 18.7 Track Delays

Every track in Live comes with a Track Delay control. It lets you delay or pre-delay a track's output by some number of milliseconds, so as to make up for human, acoustic, hardware and other real-world delays.

Track Delays are reached through the Track Options entry in the Mixer Controls submenu of the View menu, or through the menu options under the mixer view control in the lower right of Live's window.

The Track Delay Control and Selector.

Altering track delays during a live performance isn't advised, as it may produce unwanted clicks or pops in the audio signal. Tiny offsets on Session View clips can instead be done with the [Nudge Backward/Forward](https://www.ableton.com/en/live-manual/12/launching-clips/#clip-offset-and-nudging) buttons in the Clip View, whereas track delays can serve for such offsets in the Arrangement View.

Bear in mind that [delay compensation](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#device-delay-compensation) for plug-ins and Live devices is a distinct feature that runs automatically by default. Track Delay values that are unusually high, or large reported latencies from plug-ins, may make the software feel noticeably sluggish. If latency problems crop up while recording and playing back instruments, you might try switching off device delay compensation, though that is not usually advised. Tweaking the individual track delays can also prove helpful in such cases. Note that with device delay compensation turned off, the Track Delay controls become unavailable.

<a id="source-188-keep-monitoring-latency-in-recording-track-toggles"></a>
### 18.8 Keep Monitoring Latency in Recording Track Toggles

With monitoring set to “In” or “Auto,” the “Keep Monitoring Latency in Recording” option is turned on by default.

The Keep Latency in Recording Track Toggles.

This shifts the timing of the recording so that it lines up with what you hear through Live's monitoring. As a rule, it's best to keep this option on when recording software instruments or effects, and to turn it off when recording acoustic instruments or using external monitoring.

To manually flip “Keep Monitoring Latency in Recorded Audio” on or off, use the toggles or right-click the In or Auto track monitor buttons.

<a id="source-189-performance-impact-track-indicators"></a>
### 18.9 Performance Impact Track Indicators

Within the mixer section, the Performance Impact indicators let you observe how much each track contributes to the CPU load. These indicators can be revealed or hidden through the Mixer Controls submenu of the View menu or the menu options under the mixer view control in the lower right of Live's window.

The Performance Impact Indicators.

Every track carries its own CPU meter made of six rectangles that illuminate to signal that track's relative share of the current Set's CPU level. [Freezing](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#track-freeze) whichever track has the biggest share, or stripping devices off it, will normally bring the CPU load down.
