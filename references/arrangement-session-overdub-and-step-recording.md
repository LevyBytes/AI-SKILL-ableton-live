# Arrangement Session Overdub And Step Recording

Open when you need guidance on Arrangement Session Overdub And Step Recording in Ableton Live.

Context: [Recording](recording-new-clips.md#193-recording).

<a id="source-1931-recording-into-the-arrangement"></a>
### 19.3.1 Recording Into the Arrangement

Recording Into the Arrangement.

1. A click on the Control Bar’s Arrangement Record button begins the take. Exactly how it acts hinges on the “Start Playback with Record” button in the Record, Warp & Launch Settings. With that turned on, the take kicks off the instant you press the button. With it turned off, nothing records until either the Play button is engaged or Session clips fire. No matter how this preference is set, pressing Arrangement Record with Shift held flips to the reverse behavior.
2. The take generates fresh clips across every track whose Arm button is lit.
3. With MIDI Arrangement Overdub turned on, each new MIDI clip blends the existing track signal together with the freshly arriving input. Keep in mind that overdubbing is exclusive to MIDI tracks.
4. To block recording ahead of a punch-in point, switch on the Punch-In switch. It shields the track regions you'd rather leave untouched and gives you room for a pre-roll or “warm-up“ stretch. That punch-in point coincides with the Arrangement Loop’s start position.
5. In the same way, switch on the Punch-Out switch to stop recording past the punch-out point. The punch-out point lines up with the Arrangement Loop’s end position.
6. Recording into the [Arrangement Loop](https://www.ableton.com/en/live-manual/12/arrangement-view/#the-arrangement-loop) causes Live to keep every pass of audio it captures.

A loop take can be “unrolled“ afterward, either by triggering the Edit menu’s Undo command over and over or visually within the Clip View: once the loop take finishes, double-click the new clip. The Clip View’s Sample Editor then shows one extended sample holding everything recorded across the loop-recording run. Whatever the Clip View’s loop brace covers is the last pass; sliding the markers leftward lets you preview audio from earlier passes.

<a id="source-1932-recording-into-session-slots"></a>
### 19.3.2 Recording Into Session Slots

Fresh clips can be captured spontaneously into whichever Session slots you choose.

Recording Into the Session View.

1. So that clips come out cleanly cut, set the Global Quantization chooser to anything besides “None“.
2. Turn on the Arm button for whichever tracks you intend to capture. Clip Record buttons then show up in the empty slots of those armed tracks.
3. Press the Session Record button to capture the chosen scene across all armed tracks. Each clip slot gets a new clip marked by a red Clip Launch button signaling an active take. Pressing the Session Record button a second time switches straight from recording into loop playback.
4. As another route, clicking any individual Clip Record button records into that one slot. Hitting the clip’s Launch button then moves you directly from recording into loop playback.
5. Halt a clip completely by pressing either its Clip Stop button or the Control Bar's Stop button.

You can also stop playback and get ready for another “take” using the New button. That button silences clips across all armed tracks and picks a scene for fresh clips, spawning a new scene when one is needed. Bear in mind the New button only shows up under Key Map Mode and MIDI Map Mode. The [Computer Keyboard Remote Control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control) section walks through setting up keyboard assignments step by step. For more on MIDI assignments, consult the [MIDI and Key Remote Control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-remote-control) chapter.

The Control Bar shows the New Button while Key Map Mode is active.

By default, be aware that triggering a Session View scene won't begin recording in that scene's empty record-enabled slots. To override this, switch on the Start Recording on Scene Launch option in the Record, Warp & Launch Settings, which instructs Live to let empty scene slots record in those situations.

<a id="source-1933-overdub-recording-midi-patterns"></a>
### 19.3.3 Overdub Recording MIDI Patterns

Capturing drum-style patterns and similar parts is straightforward in Live. With Live’s Impulse instrument plus the method below, you can layer up drum patterns one step at a time while hearing the outcome. Alternatively, an instrument like Simpler, which supports chromatic play, lets you assemble melodies or harmonies a single note at a time.

1. Set the Global Quantization chooser to one bar.
2. So your incoming notes snap automatically, pick a fitting value under [Record Quantization](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-quantized-midi-notes).
3. Double-click one of the Session View slots on the MIDI track you want (whichever holds the Impulse or another instrument). An empty new clip lands in that slot. Its loop length starts out at one bar, though double-clicking the clip and editing its [loop properties](https://www.ableton.com/en/live-manual/12/clip-view/#clip-and-loop-region-settings) lets you alter that.
4. Arm the track.
5. Press the Session Record button.
6. Whatever notes you play go into the looping clip, and the Clip View lets you watch the take as it happens.
7. Because the clip overdubs each time it loops, you stack your pattern one layer after another. Should you want a break to rehearse, though, press the Session Record button again to switch overdubbing off. The clip keeps sounding, yet your playing stays unrecorded. Press the Session Record button yet again when you're set to resume. Each further press of the Session Record button flips back and forth between playback and overdub.

Keep in mind that holding Alt (Win) / Option (Mac) as you double-click the empty slot to make a new clip will both arm the track and trigger the clip automatically.

While overdub recording is underway, the Undo command is available at any moment to scrap the most recent take, and you can likewise draw, shift or erase notes within the Clip View’s MIDI Note Editor.

<a id="source-1934-midi-step-recording"></a>
### 19.3.4 MIDI Step Recording

In the MIDI Editor you can lay down notes while the transport sits still: hold keys on your controller or computer MIDI keyboard and push the insert marker forward in line with the grid settings. That workflow, called step recording, lets you place notes at whatever speed you like, free of any metronome or guide track.

Step Recording in the MIDI Editor.

1. Arm the MIDI track holding the clip you intend to record into.
2. Switch on the Preview switch inside the clip’s MIDI Editor.
3. Click within the MIDI Editor to drop the insert marker wherever you'd like the take to start.

Tapping the right arrow key on the computer keyboard shifts the insert marker rightward in step with the grid settings. Whatever notes you're holding as you tap the right arrow key get written into the clip. Keep holding those notes and tap the right arrow key once more to lengthen them. To erase notes you've only just laid down, keep them held and tap the left arrow key.

You can also [MIDI map](https://www.ableton.com/en/live-manual/12/recording-new-clips/#using-remote-control-for-recording) the step recording navigators.
