# MIDI Multiclip Focus And View Behavior

Open when you need guidance on MIDI Multiclip Focus And View Behavior in Ableton Live.

Context: [Multi-Clip Editing](midi-scales-and-clips-routes.md#108-multi-clip-editing).

<a id="source-1081-focus-mode"></a>
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

<a id="source-1082-multi-clip-editing-in-the-session-view"></a>
### 10.8.2 Multi-Clip Editing in the Session View

Within the Session View you can pick and display as many as eight MIDI clips at once, every one of which has to be looped. Inside the MIDI Note Editor the loop bars run vertically, ordered first by track and then by scene.

When the selected clips differ in length, the MIDI Note Editor displays however many loop iterations are needed for the clips to line back up. Any stretch of the timeline beyond a clip’s loop area is shown in a darkened shade of the clip color. Hovering over a clip, you see its loop start and end drawn as black vertical lines in the MIDI Note Editor. Should a clip’s start marker sit ahead of the loop start, the clip’s loop markers shift to reflect that.

<a id="source-1083-multi-clip-editing-in-the-arrangement-view"></a>
### 10.8.3 Multi-Clip Editing in the Arrangement View

Within the Arrangement View you can pick and display MIDI clips drawn from as many as eight tracks across a span of time. Inside the MIDI Note Editor the loop bars are arranged vertically by track and horizontally by time.

You can draw notes continuously across clip boundaries, apart from when Focus Mode is on.

Rather than showing silence ahead of or following the chosen clips, the MIDI Note Editor fits its display span to run from the start of the first clip through to the end of the final clip in the selection. When the selection mixes looped and unlooped clips, the Loop button in the Clip View appears half colored.
