# MIDI Clip Cropping Time And Loops

Open when you need guidance on MIDI Clip Cropping Time And Loops in Ableton Live.

Context: [Editing MIDI Clips](midi-scales-and-clips-routes.md#107-editing-midi-clips).

<a id="source-1071-cropping-midi-clips"></a>
### 10.7.1 Cropping MIDI Clips

Any MIDI data sitting beyond the loop brace can be removed with the Crop Clip command. When a time selection exists, you can instead clear the MIDI data lying outside that selection through the Crop to Time Selection command. Just right-click a MIDI clip within the Session or Arrangement View and pick the appropriate option, or press the Ctrl+Shift+J (Win) / Cmd+Shift+J (Mac) keyboard shortcut.

Be aware that, in contrast to [cropping samples in audio clips](https://www.ableton.com/en/live-manual/12/clip-view/#cropping-clips), cropping a MIDI clip writes no new file to disk.

<a id="source-1072-the-time-commands-in-the-midi-note-editor"></a>
### 10.7.2 The …Time Commands in the MIDI Note Editor

The usual clipboard actions such as Cut, Copy and Paste touch only the notes currently selected (or those inside a time selection). However, just like in [Arrangement editing](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-time-commands), a set of “… Time” commands operates on the whole MIDI clip by adding and removing time.

Keep in mind that these actions leave the clip start/end position and the loop brace settings untouched.

- _Duplicate Time_ drops a copy of the chosen timespan into the clip, together with whatever notes it holds.
- _Delete Time_ removes a span of time from the MIDI clip, which pulls the notes on each side of the cleared region nearer together along the timeline.
- _Insert Time_ adds an amount of empty time matching the current selection into the clip, ahead of the selection.

<a id="source-1073-looping"></a>
### 10.7.3 Looping

While editing MIDI, you may decide to loop a particular stretch of a clip so you can fine-tune it while hearing that part play over and over. For that purpose you can rely on [the loop markers](https://www.ableton.com/en/live-manual/12/clip-view/#looping-clips).

To mark out a looping region, drag the loop start and end markers to new positions. Keep in mind that the looping region can be reshaped even while playback is running.

Pick a Particular Stretch of the Clip for Playback With the Loop/Region Markers.

If you click the loop brace inside a MIDI clip and then press Ctrl+D (Win) / Cmd+D (Mac), the loop brace’s length is doubled, the notes held within the original brace are copied, and the view zooms out far enough to reveal the whole loop. Whatever notes sit to the loop’s right are shifted as well, keeping their distance relative to where the loop ends.

By default MIDI clips loop. To stop an individual clip from looping, use the Clip Loop toggle found in the Main Clip Properties panel of the Clip View. Once looping is off, the loop brace appears grayed out.

Looping Switched Off for a Clip.
