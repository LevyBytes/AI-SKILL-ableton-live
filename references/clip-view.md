# Clip View (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 8. Clip View

In the _Clip View_, you configure clip properties and also inspect and modify what a clip holds — audio waveforms, MIDI notes, envelopes, or MPE data.

The Clip View.

This panel opens in several ways: double-click any clip within the Session or Arrangement View, press the Clip View Selector, or trigger the Clip View Toggle positioned beside that selector.

The Clip View Toggle and Selector.

Keep in mind that triggering the Clip View Toggle while [the Device View](https://www.ableton.com/en/live-manual/12/live-concepts/#devices) is showing causes the Clip View to appear [stacked](https://www.ableton.com/en/live-manual/12/live-concepts/#clip-and-device-view) above the Device View.

A keyboard shortcut also toggles the Clip View: CtrlAlt3 (Win) / CmdOption3 (Mac).

Dragging the top border of the Clip View resizes it. Pull that border all the way down to the bottom edge of Live’s window and the view shuts on its own; any of the approaches outlined earlier will bring it back.

If you run Live with a second window and open the Clip View, it appears in whichever window currently holds focus. Send the Clip View to the opposite window by pressing the F12 key. When the _Use Tab Key to Navigate_ option is turned off under Live’s Settings, the ShiftTab shortcut likewise shifts the view from one window to the other.

Keep in mind that the Clip View consistently reflects whatever clip is presently selected. So, with two windows in play, picking a clip in the window lacking an open Clip View causes that clip to surface in the Clip View over in the second window. Such behavior lets you, say, reserve one window for fine-grained clip editing while the other handles your Session or Arrangement work.

Within the Session View, a click on a Track Status Display brings up the Clip View so you can edit whichever clip is presently sounding in that track.

The Track Status Display for a Looping Clip.

### 8.1 Clip View Layout

A title bar plus two regions make up the Clip View: clip panels sit on the left while an editor occupies the right. Whether you handle an audio clip or a MIDI clip determines which panel options appear and which editor takes the stage: the Sample Editor accompanies audio clips and [the MIDI Note Editor](https://www.ableton.com/en/live-manual/12/editing-midi/#the-midi-note-editor-layout) accompanies MIDI clips.

The Clip View shown with an Audio Clip.The Clip View shown with a MIDI Clip.

### 8.1.1 Clip Title Bar

Found in the clip title bar are the Clip Activator toggle and, with audio clips, the Save Default Clip button. The name and color of whichever clip is selected also show up here.

#### 8.1.1.1 Clip Activator Toggle

The Clip Activator toggle lets you switch a clip off so it stays silent when launched within the Session View or as Arrangement playback runs. Deactivation is also reachable straight from the Session or Arrangement via the clip’s context menu, or simply by hitting the 0 key.

The Clip Activator Toggle.

With several clips selected at once, switching the Clip Activator off deactivates every one of them together.

#### 8.1.1.2 Clip Name

Initially, the name of a clip mirrors that of the file it points to, though you may alter it. Picking the _Rename_ option from the title bar context menu lets you rename a clip.

Another route is to select a clip in the Session grid or Arrangement View and invoke the Rename command via the Edit menu or the clip’s context menu. From either the Edit menu or the clip’s context menu, you can also supply your own descriptive note for the clip through the Edit Info Text command.

Bear in mind that giving an audio clip a new name leaves the referenced sample file untouched. Renaming a file instead means selecting it inside Live’s browser, then reaching for the Edit menu’s Rename command.

With more than one clip selected, the title bar shows how many clips are selected. Renaming every selected clip together is still possible, yet the fresh name won’t appear in the Clip View’s title bar.

#### 8.1.1.3 Clip Color

A freshly made clip inherits the color of the track where it was created, although you may pick a clip color by hand: open the color palette either via the Clip View’s title bar context menu or through the clip’s context menu.

Should you recolor a track’s clips, restoring the track’s color to each of them is fast: just use the Assign Track Color to Clips command found in the track header’s context menu. Likewise, a [Group Track’s](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks) color can be pushed onto all the tracks and clips it holds through the Assign Track Color to Grouped Tracks and Clips command in that Group Track header’s context menu.

Keep in mind that running either the Assign Track Color to Clips command, or its sibling Assign Track Color to Grouped Tracks and Clips, within the Session View recolors only the Session clips. By the same token, using either one in the Arrangement View touches only the color of the Arrangement clips.

With several clips selected, the title bar shows a striped pattern drawn from Live’s UI colors. Choosing a fresh color for all selected clips remains possible, but the title bar won’t mirror that change unless only one clip is selected.

#### 8.1.1.4 Saving Default Audio Clip Settings with the Sample

For audio clips, the clip title bar carries the Save Default Clip button as well, letting you store the present clip’s settings alongside the loaded sample. With several clips selected, pressing the button stores the clip settings across every sample at once.

The Save Default Clip Button.

After a clip’s settings are stored, Live brings them back each time you drag the sample into a Set. That proves particularly handy where [Warp Markers](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-markers) need to sit correctly so Live can keep lengthy files synced. Bear in mind that the Save Default Clip button has no retroactive effect: those settings serve as the default solely for new clips drawing on the same sample. Clips already built from this sample won’t pick up the settings.

This clip data folds into the [analysis file](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#analysis-files-asd) that travels with the sample.

Note that keeping default clip settings with the sample isn’t the same as storing the clip as a [Live Clip](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-clips), which captures devices and device settings too.

### 8.1.2 Clip Panels

Clip panels sit along the left edge of the Clip View.

Clip Panels.

Across both audio and MIDI clips, the [Main](https://www.ableton.com/en/live-manual/12/clip-view/#main-clip-properties-panel) and [Extended](https://www.ableton.com/en/live-manual/12/clip-view/#extended-clip-properties) Clip Properties panels hold core clip settings — clip or loop start and end points, time signature, [groove](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves), or [scale](https://www.ableton.com/en/live-manual/12/live-concepts/#scale-awareness) settings — plus [clip launch properties](https://www.ableton.com/en/live-manual/12/launching-clips/#launching-clips) (while you view Session View clips).

Since MIDI clips and audio clips carry distinct property sets in Live, each one also brings controls tailored to its kind of content. Such controls reside in extra panels: ([Audio Utilities](https://www.ableton.com/en/live-manual/12/clip-view/#audio-utilities-panel) and [Audio Transformation Tools](https://www.ableton.com/en/live-manual/12/clip-view/#transform-and-generate-panels)) panels serving audio clips, and ([Pitch and Time Utilities](https://www.ableton.com/en/live-manual/12/clip-view/#pitch-and-time-utilities-panel), plus [MIDI Transformation and Generative Tools](https://www.ableton.com/en/live-manual/12/clip-view/#transform-and-generate-panels)) serving MIDI clips.

You may lay out the Clip View panels in a horizontal or a vertical fashion. There’s also an option to flip between horizontal and vertical layouts on its own, based on the height of the Clip View region.

For a vertical layout, drag the right border of the Clip View panel (beside the Sample Editor/MIDI Note Editor) toward the left; dragging rightward returns it to a horizontal layout. As an alternative, the Arrange Clip View Panels Vertically/Horizontally options in the View menu let you pick the Clip View layout you want. For automatic switching, reach for the Arrange Clip View Panels Automatically option in either the View menu or the clip title bar context menu. Live keeps track of the Clip View layout so it returns next time you open it.

Clip View Arranged Horizontally.Clip View Arranged Vertically.

Collapsing the Clip View panels is done by double-clicking the clip title bar or by picking the Fold option from the title bar context menu.

### 8.1.3 Editor View Modes

An editor fills the right portion of the Clip View. Which editor view modes you get hinges on whether an audio clip or a MIDI clip is loaded. Switch among the modes by clicking their dedicated tabs, choosing the appropriate mode in the View menu, or by [using keyboard shortcuts](https://www.ableton.com/en/live-manual/12/live-keyboard-shortcuts/#clip-view-editor-view-modes). For audio clips, you move between the Sample Editor and the Envelope Editor; for MIDI clips, you move among the MIDI Note Editor, the Envelope Editor, and the MPE Editor.

The MIDI Note Editor.

Within the Sample Editor you can inspect the sample’s waveform and steer Live’s [sample-warping](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping) capabilities.

In the Envelope Editor you handle the [clip’s envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes), which serve to automate or modulate the effects, mixer, and clip or MIDI controls.

Through the MIDI Note Editor you manage [editing and creating MIDI notes and velocities](https://www.ableton.com/en/live-manual/12/editing-midi/#editing-midi).

With the MPE Editor you can [edit different dimensions of MIDI Polyphonic Expression (MPE)](https://www.ableton.com/en/live-manual/12/editing-mpe/#editing-mpe) for every note in a clip.

The AltTab (Win) / OptionTab (Mac) shortcut offers a quick way to flip among the editor view modes.

### 8.2 Main Clip Properties Panel

The panel furthest left in the Clip View carries settings for clip region, loop, time signature, groove, and scale.

The Main Clip Properties Panel.

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

### 8.2.2 Clip Time Signature

Set the time signature for a MIDI or audio clip through the Clip Time Signature fields. Keep in mind that this setting matters for display alone; it leaves playback unaffected.

A clip’s time signature stands entirely apart from the project’s time signature and may be assigned per clip on its own. That makes it simple to spot which clips lend themselves to rich polymetric textures when you fire clips with differing meters and/or loop lengths together.

The Clip Time Signature Fields.

### 8.2.3 Clip Groove

Through the Clip Groove chooser you pick which groove drives the clip, drawing from the grooves on hand in the [Groove Pool](https://www.ableton.com/en/live-manual/12/using-grooves/#groove-pool).

The Clip Groove Chooser.

The Hot-Swap Groove button on the clip lets you trade the groove now loaded for a fresh groove chosen from Live’s browser. Either double-click a selected groove or press the Enter key to bring the groove onto the clip. Keep in mind this action swaps out the groove previously loaded in both the Groove Pool and the clip.

Sitting beneath the Clip Groove chooser, the Commit button “writes“ the present groove settings into the clip and switches off the assigned groove. Where grooves carry positive velocity values, committing one to an audio clip produces a volume [clip envelope](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) so that the groove’s velocity data translates into audio volume changes. Keep in mind this overwrites whatever volume clip envelope the clip already had.

### 8.2.4 Clip Scale

Toggling the Scale button turns Scale Mode on or off for a clip. Assign a clip’s scale via the Root Note and Scale Name choosers.

The Scale Controls.

Choosing a scale within an audio clip leaves playback unchanged (just as the clip time signature setting has no bearing on playback); rather, scale settings get passed along to [scale aware](https://www.ableton.com/en/live-manual/12/live-concepts/#scale-awareness) devices sitting on the device chain.

Once Scale Mode is on for a MIDI clip, the keys tied to the notes within the chosen scale light up across the MIDI Note Editor piano ruler. That comes in handy when composing melodies inside a given scale. Fuller coverage of scale controls for MIDI clips appears in the [Folding and Scales](https://www.ableton.com/en/live-manual/12/editing-midi/#folding-and-scales) part of the Editing MIDI chapter.

### 8.3 Extended Clip Properties

Within the Extended Clip Properties panel you find the clip launch controls together with the MIDI bank/program controls.

The Extended Clip Properties Panel.

Keep in mind that because Arrangement clips aren’t launched but instead sound according to where they fall on the timeline, this panel surfaces the clip launch controls only with a Session View clip selected. As a result, the panel is absent from the Clip View entirely when an Arrangement audio clip is selected, and offers just the MIDI bank/program controls when an Arrangement MIDI clip is selected.

### 8.3.1 Follow Action and Launch Controls

A track may hold any number of groups, set apart by empty slots. With the Follow Action controls you spell out the way one clip after another in a group gets triggered.

By way of the launch controls you state how clips respond to mouse, computer keyboard, or MIDI note interactions. There are likewise settings for tuning the clip launch timing, scrubbing clips, and governing how MIDI note velocity bears on the clip’s volume.

Full coverage of both the Follow Action and launch controls lives in the [Launching Clips](https://www.ableton.com/en/live-manual/12/launching-clips/#launching-clips) chapter.

### 8.3.2 MIDI Clip Bank and Program Change Controls

For MIDI clips, the Extended Clip Properties panel carries settings that let Live dispatch MIDI bank/program change messages to outboard devices and plug-ins able to handle MIDI program change messages.

The Bank and Program Controls.

These controls let you fire off a bank/program change message as a clip launches. When Live is feeding MIDI to your synth, that lets every MIDI clip in your Live Set call up a separate sound on the synth. Live supplies messages spanning 128 banks holding 128 sub-banks apiece, with each sub-bank carrying 128 programs. Consult the manual that shipped with your synthesizer to learn how many of these messages it accepts.

Should you prefer that your clip send neither program nor bank change messages, just leave the bank/program choosers at “—.“

### 8.4 Audio Utilities Panel

For audio clips, the Audio Utilities panel holds [warping](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping) tools, ways to reverse and edit the sample, controls that set the sample’s tempo, gain, or transposition, plus toggles that let you build crossfades, pull the sample into memory, or apply high-quality interpolation as the sample plays.

The Audio Utilities Panel.

### 8.4.1 Warp Controls

Live provides several controls for fine-tuning the time-warping engine toward [optimal stretching quality](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes).

The Warp Controls.

With the Warp toggle off, Live sounds the sample at its native tempo, paying no mind to the present Live Set tempo. That suits samples lacking any built-in rhythmic structure: percussion hits, atmospheres, sound effects, spoken word and similar material. Flip the Warp toggle on to keep rhythmically structured samples (sample loops, music recordings, full music pieces, and so on) locked to the present song tempo. The speed of a warped sample tracks the tempo as you adjust the Control Bar’s Tempo control.

The Control Bar’s Tempo Field.

To warp accurately, Live has to understand the sample’s metrical structure. With loops that are prepared well, tempo and duration come out automatically; usually that’s precise enough for the sample to be ready for use in Live right away. Other samples may need a few hints from you.

### 8.4.2 Reversing Samples

Pressing the Reverse button produces a fresh sample by flipping the sample that the current clip points to.

The Reverse Button.

Take this route and Live reapplies the former clip’s settings (following the rules laid out below) and swaps the original sample for a new, reversed one inside the Clip View. After you save the Live Set, that new sample lives in the Set’s Project folder, under Samples/Processed/Reverse. Before the Set is saved, new samples sit at whatever spot is named as the Temporary Folder in Live’s Settings.

A handful of rules govern the reversing process. First, any Warp Markers stay pinned to their spots _in the sample_. So a Warp Marker on the downbeat of a clip’s second bar lands on the downbeat of the second-to-last bar once reversed. Clip loop/region settings flip in much the same way. Second, clip envelopes hold their place _in time_. Hence a mixer volume envelope that pulls down the volume across a clip’s first half keeps doing precisely that following reversal.

Reversing runs fairly quickly (roughly as quick as copying), though very long samples may take a moment. Should that happen, a progress bar appears in Live’s Status Bar, and further actions in the program lock up briefly (although clips already playing keep going). The instant Live starts drawing a new waveform into the Sample Editor, you can play the reversed clip and carry out other actions in the program. After a sample has been reversed, Live retains data on both the original and reversed versions right up until the program is shut. Consequently, flipping the sample back to the original and then reversing it once more happens instantly.

Reversing several clips at once isn’t possible in the Session View. Within the Arrangement View, though, you can reverse a chunk of material even if it spans multiple clips. To pull this off, mark the time range you wish to reverse and pick the Reverse Clip(s) command from the clip’s context menu, or tap the R shortcut key.

Reversing clips during a live performance isn’t advised, since a faint audio glitch may now and then crop up while Live reapplies the warp and loop settings.

### 8.4.3 Destructive Sample Editing

Pressing the Edit button launches the sample in an outside sample editing application, the one you designate under the File & Folder Settings.

The Launch Sample Editor Button.

Working a sample in an external program means you must halt Live’s playback. Upon returning to Live, the edited rendition of the sample plays back. The present set of Warp Markers survives only when the sample length stays identical to what it was before editing.

Keep in mind that edits to one sample can ripple through other clips that draw on the same sample.

### 8.4.4 Clip Start and End Fades

Switched on, the Clip Fade toggle lays a brief fade across the clip start and end to head off clicks at the clip edges. How long that fade lasts depends on the signal and spans 0-4 milliseconds.

The Clip Fade Toggle.

Keep in mind the toggle exists solely for clips in Session View. Over in Arrangement View, [clip fades](https://www.ableton.com/en/live-manual/12/arrangement-view/#audio-clip-fades-and-crossfades) get tuned through envelopes.

For every new clip, the Clip Fade toggle sits on by default whenever the Create Fades on Clip Edges option is switched on under the Record, Warp & Launch Settings.

Automatically Create Short Fades At Clip Edges.

### 8.4.5 Clip RAM Mode

Switching on the RAM Mode toggle has Live pull the audio that the clip points to into the computer’s memory instead of streaming it off disk as it plays.

The RAM Mode Toggle.

RAM Mode can address these situations:

- Your computer’s hard disk runs too slowly to feed audio across as many tracks as you’d like in real time. For deeper detail on disk-related trouble, head to [Managing the Disk Load](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#managing-the-disk-load).
- You run into audio dropouts while playing clips in [Legato Mode](https://www.ableton.com/en/live-manual/12/launching-clips/#legato-mode).

Your computer leans on the hard disk to swap out RAM contents left idle for a stretch. The greater the count of clips you keep in RAM Mode, the likelier they are to be swapped out. Live copes with disk overloads more gracefully than with swapped-out audio that shows up late: a disk overload brings unwanted mutes, while a RAM overload brings both mutes and rhythmic “hiccups.“

### 8.4.6 High Quality Interpolation

With the High Quality toggle switched on, Live applies a sophisticated sample-rate conversion algorithm that yields finer sound quality while drawing more CPU load.

The High Quality Toggle.
