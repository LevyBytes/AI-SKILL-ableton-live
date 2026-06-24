# Editing Midi (part 3)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

The initial folding choice, Fold to Notes, lets you instantly conceal any key tracks that hold no MIDI notes. It comes in handy for percussion kits in particular, since those are frequently laid out across a keyboard in zones grouped by percussion category (for instance, snares clustered a pair of octaves beneath the hi-hat cymbals). A MIDI file built from that kind of layout often relies on just one or two sounds per percussion category, so showing the full span of the keyboard serves no purpose.

You can switch on Fold to Notes through the Fold button in the Clip View header, by tapping the F shortcut key while focus rests on the MIDI Note Editor, or through the View menu entry.

The Fold Button Extracts Key Tracks Containing Notes.

When Fold to Notes is turned on for a track that holds a [Drum Rack](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#drum-racks), the editor shows only the rows that carry MIDI notes. With the option switched off, key tracks for any drum pads holding devices appear in the MIDI Note Editor.

With [Scale Mode](https://www.ableton.com/en/live-manual/12/clip-view/#clip-scale) turned on for a clip, the piano ruler highlights the notes that fall within the chosen scale. That makes it simple to recognize at a glance which notes the scale contains, so writing melodies that stay inside your selected scale becomes effortless. A dedicated button in either the Main Clip Properties panel of the Clip View or the Control Bar toggles Scale Mode. Just beside the Scale Mode button sit the Root Note and Scale Name choosers, which let you assign a root note and scale to the selected clip(s).

A MIDI Clip’s Scale Mode Settings.

Out of the box, the key tracks that belong to the chosen scale appear as a highlight across the keys of the piano ruler. Should you want a stronger visual cue for which key tracks fall inside the active scale, turn on the Highlight Scales option. With it enabled, the scale’s key tracks are emphasized in the MIDI Note Editor in addition to the highlighted piano ruler keys, and the root note stands out through a bold highlight on the piano ruler. You toggle scale highlighting through the Highlight Scale button in the Clip View header, by tapping the K shortcut key while the MIDI Note Editor holds focus, or via the Highlight Scales context menu and Options menu entry. The highlighting setting takes effect globally.

Key Tracks Belonging to the Selected Scale Are Highlighted.

Where several clips carrying distinct scale settings are selected at once, whichever clip is in the foreground governs the scale settings applied to freshly created clips. With Scale Mode turned off, a new MIDI clip adopts the scale setting from the clip selected most recently, though that scale stays inactive.

Through the piano ruler’s context menu you can choose whether a clip’s notes are spelled using flats, sharps, or a mix of both. While Scale Mode is off, that choice covers every note, but once Scale Mode is on, the preference governs only the notes lying outside the chosen scale; notes inside the scale keep their correct accidentals. There is also an “Auto” choice, which picks flats or sharps on its own according to where the root note sits within the circle of fifths. Keep in mind that you can also show the notes as MIDI note numbers rather than as pitches.

Setting a Preference for Spelling a Clip’s Notes.

Once a clip has an active scale, one more folding choice appears: Fold to Scale, which you toggle through the Scale button in the Clip View header, by tapping the G shortcut key while focus is on the MIDI Note Editor, or via the View menu entry. Turning on Fold to Scale instantly conceals every key track that lies outside the scale assigned to the clip. Be aware that any key tracks where you have already placed notes outside the active scale stay visible even with Fold to Scale switched on.

The option works well as a melodic-composition guide when you are picking complementary notes. It is particularly handy if your grasp of music theory is shaky and you would rather build melodies without endlessly nudging note placement until things “feel right.”

The Scale Button, Once Pressed, Reveals Key Tracks That Belong to the Current Scale.

### 10.7 Editing MIDI Clips

Beyond editing the individual notes inside a clip, there are also actions that affect the whole MIDI clip. Quite a few of these are described in the [Clip View](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view) chapter, yet further methods of handling MIDI clips appear below.

### 10.7.1 Cropping MIDI Clips

Any MIDI data sitting beyond the loop brace can be removed with the Crop Clip command. When a time selection exists, you can instead clear the MIDI data lying outside that selection through the Crop to Time Selection command. Just right-click a MIDI clip within the Session or Arrangement View and pick the appropriate option, or press the CtrlShiftJ (Win) / CmdShiftJ (Mac) keyboard shortcut.

Be aware that, in contrast to [cropping samples in audio clips](https://www.ableton.com/en/live-manual/12/clip-view/#cropping-clips), cropping a MIDI clip writes no new file to disk.

### 10.7.2 The …Time Commands in the MIDI Note Editor

The usual clipboard actions such as Cut, Copy and Paste touch only the notes currently selected (or those inside a time selection). However, just like in [Arrangement editing](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-time-commands), a set of “… Time” commands operates on the whole MIDI clip by adding and removing time.

Keep in mind that these actions leave the clip start/end position and the loop brace settings untouched.

- _Duplicate Time_ drops a copy of the chosen timespan into the clip, together with whatever notes it holds.
- _Delete Time_ removes a span of time from the MIDI clip, which pulls the notes on each side of the cleared region nearer together along the timeline.
- _Insert Time_ adds an amount of empty time matching the current selection into the clip, ahead of the selection.

### 10.7.3 Looping

While editing MIDI, you may decide to loop a particular stretch of a clip so you can fine-tune it while hearing that part play over and over. For that purpose you can rely on [the loop markers](https://www.ableton.com/en/live-manual/12/clip-view/#looping-clips).

To mark out a looping region, drag the loop start and end markers to new positions. Keep in mind that the looping region can be reshaped even while playback is running.

Pick a Particular Stretch of the Clip for Playback With the Loop/Region Markers.

If you click the loop brace inside a MIDI clip and then press CtrlD (Win) / CmdD (Mac), the loop brace’s length is doubled, the notes held within the original brace are copied, and the view zooms out far enough to reveal the whole loop. Whatever notes sit to the loop’s right are shifted as well, keeping their distance relative to where the loop ends.

By default MIDI clips loop. To stop an individual clip from looping, use the Clip Loop toggle found in the Main Clip Properties panel of the Clip View. Once looping is off, the loop brace appears grayed out.

Looping Switched Off for a Clip.

### 10.8 Multi-Clip Editing

The MIDI Note Editor lets you see and reach notes across several MIDI clips simultaneously. That makes the melodic and rhythmic links between clips visible as you build and polish musical ideas, and it speeds up editing material spread over different tracks and scenes. Alongside editing notes across multiple clips, you can also adjust a range of parameters for the chosen clips.

Although multi-clip editing helps when viewing clips spanning different tracks, it is equally handy when you want to compare and edit several clips that share one track. You might, for instance, build evolving pattern progressions by adding notes to a clip, then crafting a variation in the next scene, and so forth, all while keeping the rest of the track’s clips in sight.

Once several MIDI clips are selected:

- These clips’ notes appear together inside the MIDI Note Editor. You can pick and edit notes drawn from multiple selected clips simultaneously, or turn to [Focus Mode](https://www.ableton.com/en/live-manual/12/editing-midi/#focus-mode) to work on notes in one clip while the other clips’ notes stay visible.
- Loop bars show up above the MIDI Note Editor. Every loop bar stands for a separate clip in the current selection, with each bar’s color matching its clip. Clicking a clip’s note or loop bar switches editing over to that clip.
  Multi-Clip Loop Bars in the MIDI Note Editor.
- The loop length of any single clip can be changed by clicking and dragging that clip’s loop bar marker. You may likewise pick and edit loop bars belonging to several of the selected clips at once by clicking or dragging their loop markers while holding the Ctrl (Win) / Cmd (Mac) key. Holding Shift lets you select adjacent loop bars. Note: When Focus Mode is on, only a single loop bar can be selected at a time, and any prior multi-selection is disregarded.
- Selected loop bars can be duplicated through the context menu option or with the CtrlD (Win) / CmdD (Mac) keyboard shortcut.
- The clip chosen for editing has its name shown in the title bar. That proves especially handy when telling apart clips that share a color. Note: When a clip carries no name, the title bar instead shows the name of the track that holds the clip.
- A number of controls in [the Clip View panels](https://www.ableton.com/en/live-manual/12/clip-view/#clip-panels) can be edited for every selected clip. Those controls cover loop, time signature, groove, and scale settings.
- Both Fold to Notes and Fold to Scale apply across every one of the selected clips.
- Actions in the Velocity or Chance Editor only ever apply to one clip at a time. The velocity and probability markers shown belong to the foreground clip rather than every clip. You cannot alter velocity or probability for all of the notes across all selected clips.
- The height of the loop bars can be changed by clicking and dragging up or down right above the scrub area of the multi-clip title bar.

Keep in mind that multi-clip editing behaves differently depending on whether you work in [the Session View](https://www.ableton.com/en/live-manual/12/editing-midi/#multi-clip-editing-in-the-session-view) or in [the Arrangement View](https://www.ableton.com/en/live-manual/12/editing-midi/#multi-clip-editing-in-the-arrangement-view).

### 10.8.1 Focus Mode

Focus Mode lets you pick one clip to edit while several clips remain in view. You toggle Focus Mode through the Focus button or with the N keyboard shortcut. Holding N as you edit with the mouse switches Focus Mode on temporarily. How multi-clip editing behaves changes according to whether Focus Mode is on or off.

The Focus Button Toggles Focus Mode.

While Focus Mode is on:

- The notes of the active clip appear in that clip’s color, whereas the notes of the inactive clips are drawn in gray.
- The active clip’s loop bar appears in the clip color, while the inactive ones appear in gray. Each time it is clicked, the active clip’s loop bar turns black. Clicking elsewhere on the active clip’s timeline, away from the loop bar, restores its loop bar to the clip color while keeping that clip in focus.
- The active clip’s name is shown beneath the loop bars.
- Moving the mouse over an inactive clip’s loop bar exposes that clip’s color and notes, which helps you settle on a different clip in the selection to edit. Clicking a clip’s note or loop bar switches editing to that clip.
- Every clip and note editing action offered by the Clip View in the MIDI Note Editor applies solely to the active clip.
- The scale shown in the Clip View belongs to the clip that is currently selected. That scale governs the Fold to Scale option.
- Turning on Fold to Notes folds every key track outside all of the selected clips.

While Focus Mode is off:

- Because all notes are active, each one appears in its clip’s color.
- Clicking a clip’s loop bar turns it black, which then lets you randomize Velocity or Chance for that clip’s notes by first-clicking. The loop brace that is not selected shows the color of its clip.
- The root note and scale name for the clips currently selected appear in the Clip View only when they match across every clip. If they differ, an asterisk appears wherever the root notes or scale names are not the same.
- Every clip and note editing action offered by the Clip View in the MIDI Note Editor is available for all of the selected clips.
- You can cut or copy notes out of several clips and paste them into that same group of clips, provided the clip selection/foreground clip stays unchanged, or into another clip after that new clip has been selected.
- Note editing actions (for example copy, cut, paste, delete) work when you handle note selections that span clips and loop boundaries.
- Time can be selected in the MIDI Note Editor across loop and clip boundaries.

### 10.8.2 Multi-Clip Editing in the Session View

Within the Session View you can pick and display as many as eight MIDI clips at once, every one of which has to be looped. Inside the MIDI Note Editor the loop bars run vertically, ordered first by track and then by scene.

When the selected clips differ in length, the MIDI Note Editor displays however many loop iterations are needed for the clips to line back up. Any stretch of the timeline beyond a clip’s loop area is shown in a darkened shade of the clip color. Hovering over a clip, you see its loop start and end drawn as black vertical lines in the MIDI Note Editor. Should a clip’s start marker sit ahead of the loop start, the clip’s loop markers shift to reflect that.

### 10.8.3 Multi-Clip Editing in the Arrangement View

Within the Arrangement View you can pick and display MIDI clips drawn from as many as eight tracks across a span of time. Inside the MIDI Note Editor the loop bars are arranged vertically by track and horizontally by time.

You can draw notes continuously across clip boundaries, apart from when Focus Mode is on.

Rather than showing silence ahead of or following the chosen clips, the MIDI Note Editor fits its display span to run from the start of the first clip through to the end of the final clip in the selection. When the selection mixes looped and unlooped clips, the Loop button in the Clip View appears half colored.
