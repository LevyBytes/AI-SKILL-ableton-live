# Session View

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 7. Session View

Within Live’s [Arrangement View](https://www.ableton.com/en/live-manual/12/arrangement-view/#arrangement-view) — and in conventional sequencers generally — events are pinned to a set song timeline. That model proves restrictive for several kinds of work:

- During a live set or a DJ performance, you rarely know ahead of time which pieces will play, how long each runs, or the order of the sections inside them.
- Theatrical sound design must respond moment-to-moment to the action unfolding onstage.
- While scoring a track or a film, kicking off from an improvised pass — then honing it toward the finished piece — often proves quicker and sparks more ideas.

Handling precisely these scenarios is the purpose of Live’s distinctive _Session View_.

### 7.1 Session View Clips

The Controls for a Session View Clip.

1. A triangular button sits at the left edge of every clip in the Session View. Whenever you like, click that button with the mouse to “launch“ playback of the clip, or single out a clip beforehand by clicking its name and then triggering it with the computer’s Enter key. From there the arrow keys let you hop to adjacent clips. See the manual section covering [clip launch settings](https://www.ableton.com/en/live-manual/12/launching-clips/#the-launch-controls) if you want to tailor that behavior.
2. To halt a clip that’s playing, click a square Clip Stop button — either within one of the track’s slots or down in the _Track Status field_ beneath the Session grid.

When one or more Session View clips are selected, hitting the 0 key switches those clips off.

By means of the computer keyboard or a MIDI controller, clips support [remote control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control). It is even possible to assign them across MIDI note ranges, letting them sound chromatically.

There’s no restriction on when or in what sequence clips fire. Their arrangement on the grid imposes no playback order; the Session grid grants random access to whatever clips sit within it.

Be aware that halting a Session View clip still leaves the Control Bar’s Play button lit, with the Arrangement Position fields continuing to advance. By holding an unbroken stream of musical time, those fields let you track exactly where you are in song time throughout a live set or while [recording into the Arrangement](https://www.ableton.com/en/live-manual/12/session-view/#recording-sessions-into-the-arrangement), no matter what the individual Session clips happen to be doing.

A double-click of the Control Bar’s Stop button at any point resets the Arrangement Position fields to 1.1.1 and halts playback across the whole Live Set.

The Arrangement Position Fields and the Stop Button.

To rename a clip, use the Rename command found in the Edit menu or in the clip’s context menu; issuing the Rename command also lets you rename a batch of selected clips together. Likewise, the Edit Info Text command in the Edit menu or the clip’s context menu lets you attach your own descriptive text to a clip. Within that context menu there’s also a color palette for picking a custom clip color.

Drag-and-drop reorders clips. You can grab several clips at once — adjacent ones via Shift-clicking, scattered ones via Ctrl-clicking.

Slots inside [Group Tracks](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks) display a shaded region signaling that one or more of the enclosed tracks holds a clip in that scene. That shading takes on the color of the group’s left-most clip. Such group slots carry launch buttons as well, firing every one of the matching clips. Where a group slot has no clips behind it, a stop button appears instead. Clicking any group slot selects each clip it stands for.

Group Slots and Group Launch Buttons.

### 7.2 Tracks and Scenes

A single clip is the most any vertical column — that is, any track — will play at one moment. So it’s logical to gather clips meant as alternatives to one another into the same column: the sections of a song, different takes on a drum loop, and so on.

Resized Session View Tracks.

So that you can reach more clips simultaneously, Session View tracks are resizable: click and drag along the edges of their title bars. Narrowing a track this way leaves only its Clip Launch buttons and the most important track controls on view. Holding Alt (Win) / Option (Mac) as you drag a single track resizes every Session View track together.

A Scene in the Session View.

With a Session View track header selected, pressing the 0 key turns that track off.

Those horizontal rows go by the name _scenes_. Sitting in the far-right column — the one standing for the [Main track](https://www.ableton.com/en/live-manual/12/mixing/#return-tracks-and-the-main-track) — are the _Scene Launch buttons_. Clicking the matching Scene Launch button fires every clip in that row at once, which comes in handy when staging the live performance of a multi-part song. To call off a scene you’ve already triggered, click the Cancel Scene Launch entry within the Main track’s context menu.

Once a scene launches, the scene directly beneath it is queued up as the next to fire automatically — unless you’ve set the Select Next Scene on Launch option in the Launch Settings to “Off.“ That behavior lets you run scenes downward through the list without selecting each one first. Both computer keys and a MIDI controller can fire scenes and [scroll between them](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#relative-session-view-navigation).

To rename a scene, reach for the Rename command, which lives in the Edit menu and also in the scene’s context menu. To rename a run of scenes in quick succession, fire the Rename command and tap the computer’s Tab key to step from one to the next. Giving a scene your own descriptive text works much the same way through the Edit Info Text command, located in the Edit menu as well as the scene’s context menu. That context menu also holds a color palette for assigning a custom scene color.

Drag-and-drop reorders scenes. Adjacent ones are gathered by Shift-clicking and scattered ones by Ctrl-clicking. Dropping a dragged set of non-adjacent scenes collapses them together; to relocate non-adjacent scenes while keeping them apart, reach for Ctrl + the up or down arrow keys rather than the mouse.

A number belonging to each scene shows up in a column along the right edge. Position dictates these numbers: relocate a scene and its number updates to reflect where it now sits.

### 7.2.1 Editing Scene Tempo and Time Signature Values

Drag the left edge of the Main track’s title header outward and the Scene Tempo and Scene Time Signature controls come into view, letting you attach a tempo, a time signature, or both to a chosen scene. By default these controls stay tucked away. As soon as the scene fires, the project shifts itself to match those settings. To alter a scene’s tempo or time signature values:

- Drag upward or downward inside whichever field you want.
- Click, key in a number, and press Enter.

These tempo and time signature values for scenes can likewise be edited from the [Scene View](https://www.ableton.com/en/live-manual/12/session-view/#scene-view).

You’re free to pick any tempo so long as it stays inside the span permitted by Live’s Tempo control (20-999 BPM). Likewise any time signature works, as long as its numerator falls between 1 and 99 and its denominator carries a beat value of 1, 2, 4, 8 or 16.

Once active, the Scene Tempo and Scene Time Signature controls can be switched off and cleared through the Return to Default context menu entry or with the Delete key; double-clicking either control disables it as well.

The left and right arrow keys let you jump in a hurry from a selected clip slot or scene over to the Scene Tempo and Scene Time Signature controls. While keying in a scene name, or a tempo or time signature value within the Main track, the Tab or ShiftTab keyboard shortcut steps to the following or preceding control so you can edit them swiftly. Reaching a scene’s last or first control sends the navigation onward to the next or previous scene.

Note: With a Scene Tempo/Time Signature control selected in the Main track, a single press of Enter selects the corresponding scene; press Enter a second time to launch that selected scene.

These Scenes Will Change the Tempo and Time Signature.

A scene carrying a tempo and/or time signature change shows a colored Scene Launch button.

Note: Where a Set built in a Live release earlier than Live 11 stored tempo and/or time signature values inside its scene names, those values transfer across to the Scene Tempo and/or Time Signature controls. Opening such a Set in a more recent Live version widens the Main track so the Scene Tempo and Scene Time Signature controls show.

### 7.2.2 Scene View

Adjusting and setting the properties of a scene is what the Scene View is for.

The Scene View.

The Scene View opens when you select one or several scenes, click a Scene Tempo or Scene Time Signature control, or click the Main track title bar.

Up in the Scene View’s top portion sit the Tempo and Signature sliders for editing the tempo and time signature values of the chosen scene(s). The [Editing Scene Tempo and Time Signature Values](https://www.ableton.com/en/live-manual/12/session-view/#editing-scene-tempo-and-time-signature-values) part of this chapter goes deeper into these controls.

Tempo and Time Signature Controls in the Scene View.

Down in the Scene View’s bottom portion, the controls there let you edit [Follow Actions](https://www.ableton.com/en/live-manual/12/launching-clips/#follow-actions) for the chosen scene(s).

Follow Action Controls in the Scene View.

With just one scene selected, the Scene View’s title bar shows that scene’s name and number — plus its color, where one is assigned. Where several scenes are selected, the title bar reports the count of selected scenes in place of that.

The context menu on the Scene View’s title bar offers two choices: renaming a scene and picking a custom scene color from the palette. These hold true with multiple scenes selected as well.

### 7.3 The Track Status Fields

A glance at the Track Status field — positioned right above the mixer controls of the active track — tells you that track’s status:

A Track Playing a Looping Session Clip.

Within a clip track, the pie-chart icon stands for a [looping Session clip](https://www.ableton.com/en/live-manual/12/clip-view/#looping-clips). To the circle’s right sits the loop length in beats, while the figure on its left counts how many passes the loop has made since it launched. For a Group Track, a number-free pie-chart shows up in the Track Status field whenever one or more clips in an enclosed track are playing.

… A One-shot Session Clip…

A one-shot Session clip — one that does not loop — is shown by the progress-bar icon, whose value reports the play time still remaining in minutes:seconds.

… Monitoring the Input…

An audio track configured to [monitor its input](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#monitoring) shows a microphone icon, while a MIDI track in the same situation shows a keyboard icon.

… Playing the Arrangement.

When a track is sounding clips out of the Arrangement, a small display depicting the Arrangement clips in play comes up.

### 7.4 Setting Up the Session View Grid

A clip lands in the Session View either by import from the browser or via [recording](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips).

Dropping Multiple Clips Into the Session View.

When you drag several clips into your Set at once, Live’s default is to stack them into a single track — running vertically in the Session View or horizontally in the Arrangement View. Holding Ctrl (Win) / Cmd (Mac) before you release them spreads the clips across multiple tracks instead. That trick applies to plain audio or MIDI files, though not to [Live Clips](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-clips), since those may carry their own embedded devices.

Drag-and-drop relocates clips around the Session grid. To shift a group of clips together, first select them with the Shift or Ctrl (Win) / Cmd (Mac) modifier before you drag. Alternatively, click inside an empty slot and “rubber-band“ a selection out from there.

### 7.4.1 Select on Launch

Out of the box, clicking a Session View clip’s Launch button selects the clip too, because you’ll usually want the Clip View pointed at the freshly launched clip. Even so, certain power-users would rather the present focus — say, a return track’s devices — not vanish merely because a clip fired, particularly when they launch a clip specifically to hear it against the return track device settings. Switch off the Select on Launch option in the Launch Settings if you’d sooner have the view stay put as you launch clips or scenes.

### 7.4.2 Removing Clip Stop Buttons

Slots Without Clip Stop Buttons.

The Edit menu’s Add/Remove Stop Button command lets you place Clip Stop buttons on the grid or take them away. That’s handy for setting up scene launch behavior ahead of time: say you’d rather scene 3 leave track 4 untouched — just clear the scene 3/track 4 Stop button.

### 7.4.3 Editing Scenes

Beyond the usual Edit menu commands — cut, copy, paste and duplicate — the Create menu holds two handy commands aimed squarely at scenes:

- _Insert Scene_ drops an empty scene right under the present selection.
- _Capture and Insert Scene_ drops a new scene under the present selection, fills it with copies of whatever clips are running at that moment, and fires the new scene at once with no break in the sound. It’s a real boon while developing material in the Session View: snapshot a compelling moment as a fresh scene, then carry on tweaking clip properties and testing clip combinations.

### 7.5 Recording Sessions into the Arrangement

What you perform in the Session View can be captured into the Arrangement, opening up an improvised route to building songs and scores.

The Control Bar’s Arrangement Record Button.

While the Arrangement Record button is engaged, Live records every move you make into the Arrangement:

- Whichever clips you launch;
- Adjustments to those [clips’ properties](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view);
- Adjustments to the mixer and to the devices’ controls — what’s called [_automation_](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#recording-automation-in-arrangement-view);
- Tempo and time signature shifts, when those are baked into the names of the scenes you launch.

Press the Arrangement Record button once more, or halt playback, to wrap up recording.

The Arrangement Selector.

Open the Arrangement View to see what your recording produced. You’ll find that Live has duplicated the clips you fired off while recording into the Arrangement, on the right tracks and at the right song positions. Bear in mind no new audio data came from the recording — only clips.

A track’s Session clips and Arrangement clips can’t both sound at once; they’re mutually exclusive. Launching a Session clip makes Live drop that track’s Arrangement playback in favor of the Session clip, while clicking a Clip Stop button halts the Arrangement playback, leaving silence.

Playback of the Arrangement stays paused until you deliberately tell Live to pick it back up by clicking the Back to Arrangement button — it shows in the Arrangement View and glows as a reminder that what’s sounding isn’t the same as the Arrangement.

The Back to Arrangement Button as shown within the Session View.The Back to Arrangement Button as it appears in the Arrangement View.

Click the Stop All Clips button in the Main track Status field to switch off every Arrangement clip in one go. Because the Arrangement’s clips and the Session View’s clips live independently of each other, you can keep improvising into the Arrangement again and again until it lands right.

The Stop All Clips Button.

On top of that, clips travel not just around the Session grid but also between the Session View and the Arrangement in both directions: through Copy and Paste, by dragging them onto the or selectors, or simply by dragging them across the two windows once you’ve switched on the Second Window option with CtrlShiftW (Win) / CmdShiftW (Mac) or through the View menu.

Pasting material out of the Arrangement and into the Session View prompts Live to hold onto the clips’ temporal layout by stacking them in a corresponding top-to-bottom order. Working downward through the scenes then lets you rebuild the original arrangement — a handy way to send a finished piece of music back into the improvisational phase.

The Arrangement View’s _Consolidate Time to New Scene_ command offers yet another route for shifting material from the Arrangement to the Session; reach it from the Create menu or the context menu of an Arrangement selection. It gathers everything inside the chosen time range into a single new clip on each track, dropping those new clips into a fresh Session View scene beneath the scene that was selected. As with the Arrangement’s [Consolidate command](https://www.ableton.com/en/live-manual/12/arrangement-view/#consolidating-clips), this generates a new sample for each audio track in the selection that held at least one clip.
