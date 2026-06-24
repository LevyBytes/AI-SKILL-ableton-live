# Mixing

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 18. Mixing

### 18.1 The Live Mixer

A mixer section is built into Live, and you can reach it from either Session or Arrangement View:

The Arrangement View Mixer.

Mixer controls for a single track can also be reached in Arrangement View through that track's Track Controls section.

The Arrangement View Track Controls.

Under Session View, the mixer area sits directly beneath the scenes belonging to each track.

The Session View Mixer.

The mixer view control, tucked into the lower-right corner of Live's window, lets you reveal or conceal the mixer.

The Mixer View Control.

Beside that control sits a drop-down menu toggle, which reveals or hides the individual mixer components.

The Mixer View Control's Options Menu.

Now consider each of the mixer controls:

The Mixer Controls.

1. The Meter displays the track's peak and RMS output levels. During monitoring, though, it presents peak and RMS input levels instead. Sudden jumps in level are revealed by peak meters, whereas RMS meters convey a more accurate sense of perceived loudness.
2. Adjusting a track's output level is the job of the Volume control. When several tracks are selected, changing the volume on one of them changes it on the rest too.
3. Two distinct modes are offered by the Pan control: the default Stereo Pan Mode and the Split Stereo Pan Mode. Under Stereo Pan Mode, the Pan control places the track's output somewhere within the stereo field. Clicking the triangle next to the control returns the Pan control to center. Under Split Stereo Pan Mode, separate sliders allow you to set the placement of the track's left and right input channels independently. Reset these sliders by double-clicking them. The Pan control's context menu is where you toggle between the two pan modes. When several tracks are selected, turning the pan knob on one of them turns it on the others as well.
4. Silencing a track's output is done by switching off the Track Activator switch. When several tracks are selected, flipping one of their Track Activators flips the rest too.
5. Pressing the Solo switch (or hitting the S shortcut key) solos that track by silencing every other track, though it can also serve for [cueing](https://www.ableton.com/en/live-manual/12/mixing/#soloing-and-cueing). When several tracks are selected, hitting any of their Solo switches solos them all. In other cases, only one track may be soloed at a time, unless you hold the Ctrl (Win) / Cmd (Mac) modifier or have turned off the Exclusive Solo option in the Record, Warp & Launch Settings.
6. When the Arm Recording button is enabled, that track becomes [record-enabled](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips). When several tracks are selected, hitting any of their Arm switches arms them all. In other cases, only one track may be armed at a time, unless you hold the Ctrl (Win) / Cmd (Mac) modifier or have turned off the Exclusive Arm option in the Record, Warp & Launch Settings. While Exclusive Arm is active, dropping an instrument onto a fresh or empty MIDI track will arm that track automatically.

### 18.1.1 Additional Mixer Features

Additional Mixer Possibilities.

A number of extra capabilities live in the Mixer section that stay hidden by default. Since the mixer can be resized, dragging the top edge of the mixer upward stretches the track meters taller, which brings in tick marks, a numeric volume field and resettable peak level indicators. Widening a track while in this state adds a decibel scale next to the tick marks of the meter.

While these additions suit conventional mixing workflows, they remain accessible whenever the Mixer section is on screen.

Thanks to the vast headroom of Live's 32-bit floating point audio engine, the audio and MIDI tracks in Live can be pushed well “into the red“ before the signals begin to clip. Signals exceeding 0 dB only become a concern when audio departs Live and enters the outside world. Some instances are:

- While routing into or out of physical inputs and outputs, such as the ones on your sound card.
- Signal carried on the Main track, which nearly always feeds a physical output.
- While saving audio to a file or exporting it.

Even so, Live offers this optional visual cue for any signal in a track that climbs past 0 dB.

### 18.2 Audio and MIDI Tracks

In Live, audio and MIDI tracks exist to hold and play back clips, a topic covered in the [Live Concepts](https://www.ableton.com/en/live-manual/12/live-concepts/#live-concepts) chapter.

Fresh audio and MIDI tracks can be brought into your Live Set through the relevant Create menu commands, or via the shortcuts CtrlT (Win) / CmdT (Mac) for an audio track and CtrlShiftT (Win) / CmdShiftT (Mac) for a MIDI track.

You can also make tracks by double-clicking or hitting Enter on browser files to load them, or by dragging items out of the browser into the area to the right of Session View tracks or beneath Arrangement View tracks. Devices or files brought into Live this way generate tracks matching their type (for instance, dragging in a MIDI file or effect produces a MIDI track).

Pulling one clip, or several, from an existing track into the area to the right of Session View tracks or beneath Arrangement View tracks builds a new track holding those clips along with the original track's devices.

Each track is shown by its _track title bar_.

Tracks are Represented by Track Title Bars.

Clicking a track title bar selects the track, after which an Edit menu command can be run on it to make changes. Rename is one such command that is available. A whole series of tracks can be renamed quickly by running this command, or the Rename shortcut CtrlR (Win) / CmdR (Mac), then pressing Tab to jump from one title bar to the next.

If a name begins with a # symbol, the track receives a number that refreshes on its own as the track gets moved. Each extra # symbol pads the track number with another leading zero. You may also supply your own [info text](https://www.ableton.com/en/live-manual/12/first-steps/#info-view) for a track through the Edit Info Text command found in the Edit menu or in that track's context menu.

To reorder tracks, drag them by their title bars; to alter their width (in Session View) or height (in Arrangement View), click and drag along their edges.

Several adjacent or nonadjacent tracks may be picked at the same time by Shift-clicking or Ctrl-clicking, respectively. Dragging a group of nonadjacent tracks causes them to merge together upon being dropped. To shift nonadjacent tracks while keeping them apart, rely on Ctrl + arrow keys rather than the mouse.

While more than one track is selected, modifying one of their mixer controls modifies that same control across the others. Should the tracks in the multi-selection hold different values for some knob or slider parameter (volume, say), that gap stays intact as you move the parameter.

Dragging a track's title bar onto a folder within the Places section of the browser stores it as a new Set. When a track holds audio clips, Live handles copying the referenced samples into this fresh location according to the choice made in the [Collect Files on Export](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#collect-files-on-export) chooser. You may then enter a name for the new Set or accept the one Live proposes by pressing Enter.

To remove tracks, use the Delete command in the Edit menu.

### 18.3 Group Tracks

Any quantity of separate audio or MIDI tracks can be merged into a special summing container known as a Group Track. Building a Group Track is a matter of selecting the tracks you want included and running the Group Tracks command in the Edit menu. The same command also nests one or more existing Group Tracks inside a new Group Track.

Although a Group Track can't hold clips of its own, it resembles an audio track in having mixer controls and the ability to host audio effects.

A fast route to building [submixes](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#creating-submixes) is also provided by Group Tracks. As tracks enter a group, their Audio To [routing choosers](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#internal-routings) get pointed at their Group Track automatically, unless a custom routing was already in place, i.e. aimed at somewhere other than Main. A Group Track can equally serve simply as a “folder“ track by sending the outputs of its member tracks elsewhere.

A group's tracks can be revealed or concealed through the Unfold Group button on the title bar. This is useful for tidying up large Sets by tucking away tracks you have no need to view.

An Unfolded Group Track in Session View.

After a Group Track exists, tracks may be dragged into it or out of it. Removing a Group Track wipes out everything inside it, yet a group can be turned back into separate tracks by running the Ungroup Tracks command in the Edit Menu.

Within Arrangement View, Group Tracks present a summary of the clips held in their member tracks.

A Folded Group Track in Arrangement View

Inside Session View, slots within Group Tracks carry launch and stop buttons as soon as a single clip exists somewhere in a scene. Pressing this button to launch or stop has the same result as launching or stopping every clip it contains. In the same way, picking a Group Slot acts as a shortcut for picking all of the clips inside.

To push a Group Track's color onto every track and clip it contains, run the Assign Track Color to Grouped Tracks and Clips command from the context menu of that Group Track's header.

Keep in mind that, within Session View, invoking the Assign Track Color to Grouped Tracks and Clips command recolors only the Session clips. In the same way, running either command in Arrangement View recolors only the Arrangement clips.

When a Group Track holds a soloed track or a nested Group Track, its Solo button shows up half colored.

Solo Button of a Group Track Containing a Soloed Nested Group Track.

### 18.4 Return Tracks and the Main track

Beyond Group Tracks and the tracks that play clips, every Live Set has a _Main track_ together with _return tracks_; while these can't play clips, they enable more versatile signal processing and routing.

Both the return tracks and the Main track sit along the right edge of the Session mixer view and at the lower portion of the Arrangement View.

Keep in mind that the return tracks can be shown or hidden through the _Return Tracks_ entry found in the Mixer Controls submenu of the View menu.

Just like ordinary clip tracks, return tracks are able to host effects devices. The difference is that an effect on a clip track works only on that track's own audio, while return tracks can work on audio routed to them from many tracks at once.

Imagine, for instance, that you wish to produce rhythmic echoes via a delay effect. Drop the effect onto a clip track and only the clips played in that track get echoed. Put that same effect on a return track and it can take in audio from any number of tracks and apply echoes to them.

The Send Controls and Pre/Post Toggles.

A clip or group track's Send control sets how much of that track's output is fed into the input of the linked return track. Beyond that, even a return track's own output can be sent back to its input, which lets you build feedback. Since runaway feedback can spike the level loudly and without warning, the Send controls on Return tracks come disabled by default. Turn them on by right-clicking a Return track's Send knob and choosing Enable Send or Enable All Sends.

A Pre/Post toggle exists on every return track, deciding whether the signal a clip track feeds it is taken before or after the mixer stage (that is, the pan, volume and track-active controls). With the “Pre“ setting, you can build an auxiliary mix that gets processed in the return track, separate from the main mix. Because the return track can be sent to its own output, this works for setting up a dedicated monitor mix for one player in a band.

Signals from all other tracks default to the Main track as their destination. Drag effects onto it to treat the combined signal before it reaches the Main output. Effects placed on the Main track typically handle _mastering_-style tasks like compression and/or EQ.

Several return tracks can be made through the Insert Return Track command in the Create menu, but there is, by definition, just a single Main track.

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

### 18.7 Track Delays

Every track in Live comes with a Track Delay control. It lets you delay or pre-delay a track's output by some number of milliseconds, so as to make up for human, acoustic, hardware and other real-world delays.

Track Delays are reached through the Track Options entry in the Mixer Controls submenu of the View menu, or through the menu options under the mixer view control in the lower right of Live's window.

The Track Delay Control and Selector.

Altering track delays during a live performance isn't advised, as it may produce unwanted clicks or pops in the audio signal. Tiny offsets on Session View clips can instead be done with the [Nudge Backward/Forward](https://www.ableton.com/en/live-manual/12/launching-clips/#clip-offset-and-nudging) buttons in the Clip View, whereas track delays can serve for such offsets in the Arrangement View.

Bear in mind that [delay compensation](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#device-delay-compensation) for plug-ins and Live devices is a distinct feature that runs automatically by default. Track Delay values that are unusually high, or large reported latencies from plug-ins, may make the software feel noticeably sluggish. If latency problems crop up while recording and playing back instruments, you might try switching off device delay compensation, though that is not usually advised. Tweaking the individual track delays can also prove helpful in such cases. Note that with device delay compensation turned off, the Track Delay controls become unavailable.

### 18.8 Keep Monitoring Latency in Recording Track Toggles

With monitoring set to “In” or “Auto,” the “Keep Monitoring Latency in Recording” option is turned on by default.

The Keep Latency in Recording Track Toggles.

This shifts the timing of the recording so that it lines up with what you hear through Live's monitoring. As a rule, it's best to keep this option on when recording software instruments or effects, and to turn it off when recording acoustic instruments or using external monitoring.

To manually flip “Keep Monitoring Latency in Recorded Audio” on or off, use the toggles or right-click the In or Auto track monitor buttons.

### 18.9 Performance Impact Track Indicators

Within the mixer section, the Performance Impact indicators let you observe how much each track contributes to the CPU load. These indicators can be revealed or hidden through the Mixer Controls submenu of the View menu or the menu options under the mixer view control in the lower right of Live's window.

The Performance Impact Indicators.

Every track carries its own CPU meter made of six rectangles that illuminate to signal that track's relative share of the current Set's CPU level. [Freezing](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#track-freeze) whichever track has the biggest share, or stripping devices off it, will normally bring the CPU load down.
