# Clip Loop Meter Groove And Scale

Open when you need guidance on Clip Loop Meter Groove And Scale in Ableton Live.

Context: [Main Clip Properties Panel](clip-view.md#82-main-clip-properties-panel).

<a id="source-821-clip-and-loop-region-settings"></a>
### 8.2.1 Clip and Loop Region Settings

The clip’s region and loop controls determine which portion of the clip sounds once a clip is launched. A clip without looping runs from its start point through to its end point, or until you halt it.

Tweak the clip start and end position through the matching value fields. The Set Start and Set End buttons let you fix the start and end positions mid-playback; pressing a Set button snaps the field to wherever the playhead currently sits. Defining clip start and end positions this way follows global quantization.

Use the Clip Start and End Controls to Change Clip Length.

Bear in mind that warped audio clips show the start and end position fields as bars-beats-sixteenths, whereas unwarped audio clips present those values in minutes-seconds-milliseconds.

For the clip to run as a loop, switch on the Clip Loop toggle. Define the loop region by typing the values you want into the Loop Position and Length fields. Keep in mind that the Loop Length field defaults to the clip’s full length.

The Loop Controls.

Bear in mind that with audio clips, the Warp toggle has to be on in the [Audio Utilities panel](https://www.ableton.com/en/live-manual/12/clip-view/#audio-utilities-panel) before you can enable the Clip Loop toggle, since unwarped audio clips don’t support looping.

The Loop Position and Length fields come fitted with the Set buttons, handy for building loops on the spot while playback runs.

Run the clip and then press the Set Loop Position button to drop the loop’s start at the present playback position (snapped to the global quantization setting) and turn the loop on. After that, pressing the Set Loop Length button shifts the loop’s end to the present playback position. With this you grab the music into a loop as it goes.

When the loop is still off, pressing the Set Loop Length button ends the loop at the present playback position while keeping its preset length intact. That move also turns looping on at the same moment.

Several elements — the Set buttons, plus the Clip Loop toggle, along with the loop region and the start/end positions — all support being [mapped to MIDI controls](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control). For instance, a rotary encoder could nudge the loop across a sample in steps matching the chosen quantization interval.

<a id="source-822-clip-time-signature"></a>
### 8.2.2 Clip Time Signature

Set the time signature for a MIDI or audio clip through the Clip Time Signature fields. Keep in mind that this setting matters for display alone; it leaves playback unaffected.

A clip’s time signature stands entirely apart from the project’s time signature and may be assigned per clip on its own. That makes it simple to spot which clips lend themselves to rich polymetric textures when you fire clips with differing meters and/or loop lengths together.

The Clip Time Signature Fields.

<a id="source-823-clip-groove"></a>
### 8.2.3 Clip Groove

Through the Clip Groove chooser you pick which groove drives the clip, drawing from the grooves on hand in the [Groove Pool](https://www.ableton.com/en/live-manual/12/using-grooves/#groove-pool).

The Clip Groove Chooser.

The Hot-Swap Groove button on the clip lets you trade the groove now loaded for a fresh groove chosen from Live’s browser. Either double-click a selected groove or press the Enter key to bring the groove onto the clip. Keep in mind this action swaps out the groove previously loaded in both the Groove Pool and the clip.

Sitting beneath the Clip Groove chooser, the Commit button “writes“ the present groove settings into the clip and switches off the assigned groove. Where grooves carry positive velocity values, committing one to an audio clip produces a volume [clip envelope](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) so that the groove’s velocity data translates into audio volume changes. Keep in mind this overwrites whatever volume clip envelope the clip already had.

<a id="source-824-clip-scale"></a>
### 8.2.4 Clip Scale

Toggling the Scale button turns Scale Mode on or off for a clip. Assign a clip’s scale via the Root Note and Scale Name choosers.

The Scale Controls.

Choosing a scale within an audio clip leaves playback unchanged (just as the clip time signature setting has no bearing on playback); rather, scale settings get passed along to [scale aware](https://www.ableton.com/en/live-manual/12/live-concepts/#scale-awareness) devices sitting on the device chain.

Once Scale Mode is on for a MIDI clip, the keys tied to the notes within the chosen scale light up across the MIDI Note Editor piano ruler. That comes in handy when composing melodies inside a given scale. Fuller coverage of scale controls for MIDI clips appears in the [Folding and Scales](https://www.ableton.com/en/live-manual/12/editing-midi/#folding-and-scales) part of the Editing MIDI chapter.
