# Clip Launch Modes Quantization And Offset

Open when you need guidance on Clip Launch Modes Quantization And Offset in Ableton Live.

Context: [Launching Clips](launching-clips.md#16-launching-clips).

<a id="source-161-the-launch-controls"></a>
### 16.1 The Launch Controls

Keep in mind that Session View clips get fired off via their [Clip Launch buttons](https://www.ableton.com/en/live-manual/12/session-view/#session-view-clips) or through [remote control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control). You will locate the relevant launch parameters in each clip's [clip panel](https://www.ableton.com/en/live-manual/12/clip-view/#follow-action-and-launch-controls). These launch parameters are relevant solely to Session View clips; Arrangement View clips aren't launched at all but instead sound according to where they sit in the Arrangement.

You reach these launch parameters by opening a Session View clip's Clip View — double-click the clip — and then selecting the clip tab/panel marked with the Clip Launch button icon.

The Clip Launch Settings in a Clip Tab.

Keep in mind that several clips' launch parameters can be adjusted together: select all the clips you want first, then bring up the Clip View.

<a id="source-162-launch-modes"></a>
### 16.2 Launch Modes

The Clip Launch Chooser.

Several choices appear in the Launch Mode chooser, each governing how a clip reacts to mouse clicks, presses on the computer keyboard, or incoming MIDI notes:

- Trigger: _down_ sets the clip going; _up_ has no effect.
- Gate: _down_ sets the clip going; _up_ halts it.
- Toggle: _down_ sets the clip going; _up_ has no effect. A further down press will halt the clip.
- Repeat: while you hold the mouse switch/key down, the clip retriggers over and over at the clip quantization rate.

<a id="source-163-legato-mode"></a>
### 16.3 Legato Mode

The Legato Mode Switch.

Imagine you've collected several looping clips on a single track and would like to switch between them while keeping everything in sync. One route is a coarse quantization value (a bar or more), but that approach can hem in what you're able to play.

A different route, one that holds up even when quantization is switched off entirely, is turning on Legato Mode for those clips. Launching a clip that has Legato Mode active makes it inherit the play position held by whichever clip ran on that track just before. As a result, switching between clips at any time and tempo never breaks the sync.

For building breaks, Legato Mode comes in very handy, since you can briefly drop into other loops and then return to whatever the track had been playing.

You may encounter dropouts when launching clips in Legato Mode unless every clip in question uses the identical sample (varying only in clip settings). The cause is that you've suddenly landed at a spot in the sample that Live had no opportunity to stream from disk ahead of time. The fix is to switch on [Clip RAM Mode](https://www.ableton.com/en/live-manual/12/clip-view/#clip-ram-mode) for those clips.

<a id="source-164-clip-launch-quantization"></a>
### 16.4 Clip Launch Quantization

The Clip Quantization Chooser.

Use the Clip Quantization chooser to set a correction for when triggered clips actually begin. Picking “None“ switches clip quantization off entirely.

If you'd rather follow the Control Bar’s Global Quantization value, pick “Global.“ You can rapidly alter global quantization through the Ctrl+6, 7, 8, 9, and 0 (Win) / Cmd+6, 7, 8, 9, and 0 (Mac) shortcuts.

Bear in mind that anything besides “None“ also quantizes a clip's launch whenever [Follow Actions](https://www.ableton.com/en/live-manual/12/launching-clips/#follow-actions) fire it.

<a id="source-165-velocity"></a>
### 16.5 Velocity

The Velocity Amount Field.

With the Velocity Amount control you dial in how strongly MIDI note velocity shapes a clip’s volume: a value of zero means no effect at all, while at 100 percent the quietest notes will trigger the clip with no sound. To learn more about driving clips from MIDI, see the [MIDI and Key Remote Control chapter](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control).

<a id="source-166-clip-offset-and-nudging"></a>
### 16.6 Clip Offset and Nudging

The Nudge Backward/Forward buttons let you leap around inside a clip that's playing, with each step equal to the global quantization period.

Using the Nudge Backward/Forward Buttons to Jump Through a Clip.

You can likewise assign these buttons to [keys or MIDI controllers](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#the-mapping-browser). While in MIDI Map Mode, a scrub control shows up between the Nudge Backward/Forward buttons, ready to be linked to a rotary encoder wheel so you can scrub continuously.

The Scrub Control in MIDI Map Mode.

When quantization sits below one bar, shifting a clip's playback away from Live’s master clock becomes straightforward — just launch clips, work the Nudge Backward/Forward buttons, or do some [scrubbing within the clip](https://www.ableton.com/en/live-manual/12/clip-view/#playing-and-scrubbing-clips).
