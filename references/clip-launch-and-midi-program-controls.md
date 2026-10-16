# Clip Launch And MIDI Program Controls

Open when you need guidance on Clip Launch And MIDI Program Controls in Ableton Live.

Context: [Extended Clip Properties](clip-view.md#83-extended-clip-properties).

<a id="source-831-follow-action-and-launch-controls"></a>
### 8.3.1 Follow Action and Launch Controls

A track may hold any number of groups, set apart by empty slots. With the Follow Action controls you spell out the way one clip after another in a group gets triggered.

By way of the launch controls you state how clips respond to mouse, computer keyboard, or MIDI note interactions. There are likewise settings for tuning the clip launch timing, scrubbing clips, and governing how MIDI note velocity bears on the clip’s volume.

Full coverage of both the Follow Action and launch controls lives in the [Launching Clips](https://www.ableton.com/en/live-manual/12/launching-clips/#launching-clips) chapter.

<a id="source-832-midi-clip-bank-and-program-change-controls"></a>
### 8.3.2 MIDI Clip Bank and Program Change Controls

For MIDI clips, the Extended Clip Properties panel carries settings that let Live dispatch MIDI bank/program change messages to outboard devices and plug-ins able to handle MIDI program change messages.

The Bank and Program Controls.

These controls let you fire off a bank/program change message as a clip launches. When Live is feeding MIDI to your synth, that lets every MIDI clip in your Live Set call up a separate sound on the synth. Live supplies messages spanning 128 banks holding 128 sub-banks apiece, with each sub-bank carrying 128 programs. Consult the manual that shipped with your synthesizer to learn how many of these messages it accepts.

Should you prefer that your clip send neither program nor bank change messages, just leave the bank/program choosers at “—.“
