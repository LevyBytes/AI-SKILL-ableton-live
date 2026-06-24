# Recording New Clips

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 19. Recording New Clips

Here the focus is on capturing fresh clips that originate from audio and MIDI input. Be aware that this differs from the [capturing of Session clips into the Arrangement](https://www.ableton.com/en/live-manual/12/session-view/#recording-sessions-into-the-arrangement), which is a separate workflow.

To get clean audio takes, first confirm that the audio settings have been configured correctly. Bear in mind, too, that gear such as microphones, guitars and turntables runs below line level, so their signal must be amplified before any recording happens. That means you'll need either an audio interface containing a preamp or a standalone external preamp for such sources.

With MIDI tracks, you can “capture” what you played after the fact, so there's no requirement to arm the Record button ahead of time. The benefit is greater room to improvise or experiment on the spot. The [Capturing MIDI](https://www.ableton.com/en/live-manual/12/recording-new-clips/#capturing-midi) section covers this in depth.

### 19.1 Choosing an Input

Whatever source appears in a track's In/Out section is what that track will capture; that section becomes visible once the View menu’s In/Out option is checked. Within the Arrangement View, expand and enlarge the track so the In/Out section is fully visible.

The Track In/Out Section, shown for the Arrangement (Left) alongside the Session View (Right).

By default, audio tracks capture a mono signal taken from external input 1 or 2. MIDI tracks, by default, take in every MIDI message arriving through the currently active external [input devices](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#midi-port-inputs-and-outputs). You can also enable the computer keyboard to serve as a [pseudo-MIDI input device](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#playing-midi-with-the-computer-keyboard), which lets you lay down MIDI even when no MIDI controller hardware is at hand.

Each track lets you pick a different source instead of its default: any mono or stereo external input, one particular MIDI channel from one particular MIDI-in device, or a feed arriving from a separate track. Full detail on these choices lives in the [Routing and I/O](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) chapter.

### 19.2 Arming (Record-Enabling) Tracks

Track Arm Buttons in the Arrangement (Left) and Session (Right) Mixers.

Enable a track for capture by clicking its Arm button. Whether you press a track’s Arm button from the Session View or the Arrangement View makes no difference, because both views operate on one shared track set.

Armed tracks are monitored as standard behavior: their incoming signal travels through the device chain out to the output so you can hear the take as it happens. The name for this is [“auto-monitoring“](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#monitoring), and it can be adjusted to suit your workflow.

When a [natively supported control surface](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#natively-supported-control-surfaces) is in use, arming a MIDI track makes that surface lock onto whatever instrument sits in the track.

Pressing one track’s Arm button disarms every other track, unless you hold the Ctrl (Win) / Cmd (Mac) modifier. With several tracks selected, clicking the Arm button on one of them arms the rest at the same time. Because arming also selects the track, you gain quick access to its devices in the Device View.

### 19.3 Recording

Both the Session and the Arrangement Views support recording. When you need to capture several tracks at once, or you prefer watching the take unfold linearly as it happens, the Arrangement View tends to suit you better. Reach for the Session View instead whenever you want to split a take smoothly across many clips or record at the same time as you trigger other clips in Live.

### 19.3.1 Recording Into the Arrangement

Recording Into the Arrangement.

1. A click on the Control Bar’s Arrangement Record button begins the take. Exactly how it acts hinges on the “Start Playback with Record” button in the Record, Warp & Launch Settings. With that turned on, the take kicks off the instant you press the button. With it turned off, nothing records until either the Play button is engaged or Session clips fire. No matter how this preference is set, pressing Arrangement Record with Shift held flips to the reverse behavior.
2. The take generates fresh clips across every track whose Arm button is lit.
3. With MIDI Arrangement Overdub turned on, each new MIDI clip blends the existing track signal together with the freshly arriving input. Keep in mind that overdubbing is exclusive to MIDI tracks.
4. To block recording ahead of a punch-in point, switch on the Punch-In switch. It shields the track regions you'd rather leave untouched and gives you room for a pre-roll or “warm-up“ stretch. That punch-in point coincides with the Arrangement Loop’s start position.
5. In the same way, switch on the Punch-Out switch to stop recording past the punch-out point. The punch-out point lines up with the Arrangement Loop’s end position.
6. Recording into the [Arrangement Loop](https://www.ableton.com/en/live-manual/12/arrangement-view/#the-arrangement-loop) causes Live to keep every pass of audio it captures.

A loop take can be “unrolled“ afterward, either by triggering the Edit menu’s Undo command over and over or visually within the Clip View: once the loop take finishes, double-click the new clip. The Clip View’s Sample Editor then shows one extended sample holding everything recorded across the loop-recording run. Whatever the Clip View’s loop brace covers is the last pass; sliding the markers leftward lets you preview audio from earlier passes.

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

### 19.3.4 MIDI Step Recording

In the MIDI Editor you can lay down notes while the transport sits still: hold keys on your controller or computer MIDI keyboard and push the insert marker forward in line with the grid settings. That workflow, called step recording, lets you place notes at whatever speed you like, free of any metronome or guide track.

Step Recording in the MIDI Editor.

1. Arm the MIDI track holding the clip you intend to record into.
2. Switch on the Preview switch inside the clip’s MIDI Editor.
3. Click within the MIDI Editor to drop the insert marker wherever you'd like the take to start.

Tapping the right arrow key on the computer keyboard shifts the insert marker rightward in step with the grid settings. Whatever notes you're holding as you tap the right arrow key get written into the clip. Keep holding those notes and tap the right arrow key once more to lengthen them. To erase notes you've only just laid down, keep them held and tap the left arrow key.

You can also [MIDI map](https://www.ableton.com/en/live-manual/12/recording-new-clips/#using-remote-control-for-recording) the step recording navigators.

### 19.4 Recording in Sync

Whatever audio and MIDI you've captured stays locked together in Live, even once you settle on a new song tempo down the line. Indeed, Live lets you shift the tempo whenever you want, whether before, after or right in the middle of a take. As one trick, you might drop the tempo to nail a tough passage, then raise it back up once you're done.

Recording _in sync_ matters because it's what guarantees everything later _plays in sync_.

The Metronome Switch.

The simplest route to recording in sync is playing along with the built-in metronome, switched on by its Control Bar switch, which starts ticking the moment you hit the Play button or fire a clip.

The Preview Volume Knob.

Dial the metronome's loudness with the mixer’s Preview Volume knob. The pull-down menu beside the metronome switch holds additional metronome options.

Bear in mind that Live’s reading of a clip's rhythm can be reshaped whenever you wish through [Warp Markers](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-markers). These markers serve to correct timing slips and to shift the groove or feel of any audio or MIDI take. With Warp Markers you can repair issues that would otherwise demand intricate editing, or that simply couldn't be addressed otherwise.

### 19.4.1 Metronome Settings

Reach the Metronome Settings menu either through the pull-down switch beside the metronome or by opening the metronome's own context menu.

From that menu you can define the recording [count-in length](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-with-count-in). The metronome’s tick sound is adjustable here as well.

Under the _Rhythm_ settings you choose the beat division on which the metronome ticks. When left on the default “Auto” setting, the spacing of ticks tracks the time signature’s denominator. Any beat division that won't fit inside one bar of the active time signature shows up greyed out.

Should a time signature change leave the chosen beat division too large for a bar, the metronome’s tick falls back to the “Auto” setting. Yet if a later time signature change once again lets that beat division fit a bar, the tick returns to the division you selected.

With Enable Only While Recording checked and the metronome switched on, the metronome lights up whenever transport runs but only sounds during recording. When you record into the Arrangement with the Punch-In switch engaged, the metronome stays silent until the punch-in point arrives.

### 19.5 Recording Quantized MIDI Notes

When you're about to record MIDI, there's an option to quantize the notes automatically as they go down. The Edit menu's Record Quantization chooser is where you select the meter subdivisions your captured notes will snap to. During Arrangement recording, that quantization forms its own separate step in Live’s Undo history. So if, say, you recorded with Record Quantization on “Eighth Note Triplet Quantization“ and then reconsidered, the Edit menu’s Undo command would roll back the quantization alone and leave the rest of your take untouched.

Whether in Session or Arrangement recording, the Record Quantization setting can't be altered while a take is in progress.

During overdub recording with the Clip View Loop turned on, any change to the Record Quantization applies right away and can't be undone on its own through the Edit menu command.

You can also quantize captured MIDI notes after the fact via the Edit menu’s [Quantize command](https://www.ableton.com/en/live-manual/12/editing-midi/#quantizing-notes), covered in the chapter about editing MIDI.

### 19.6 Recording with Count-in

You configure a recording count-in through the pull-down menu beside the Metronome switch. Set to anything other than “None,“ it makes Live hold off on recording until the count-in finishes. While it runs, the Control Bar's Arrangement Position fields show the count-in in blue as bars-beats-sixteenths.

The Count-In is Displayed in the Control Bar.

The count-in counts up from negative bars-beats-sixteenths — starting at -2.1.1., say, when the Count-In setting is 2 bars — and reaches 1.1.1., where recording begins.

### 19.7 Setting up File Types

These Settings on the Record, Warp & Launch tab govern the sample files that recording produces:

- Pick the sample file type you'd like Live to write from the File Type chooser inside the Record, Warp & Launch Settings.
- Pick the bit depth for the sample file your recording will produce from the Bit Depth chooser inside the Record, Warp & Launch Settings.

Configuring sensible defaults for your recorded clips on the Record, Warp & Launch Settings tab saves you effort. A particularly wise move is signaling the broad type of sound you'll capture by selecting a suitable default _Warp Mode_. Then, if you opt for a different song tempo afterward, Live keeps up [good sound quality](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes) on its own, generally needing no extra tweaking.

### 19.8 Where are the Recorded Samples?

Captured samples live inside the current Set’s Project folder, specifically within Samples/Recorded. Before the Set has been saved, they sit wherever the Temporary Folder preference points, a setting located on the Settings’ File/Folder tab. So Live doesn't exhaust disk space while you record into a fresh Set, confirm that the Temporary Folder resides on a drive or partition holding enough free room.

### 19.9 Using Remote Control for Recording

Through [Key Map Mode and MIDI Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) you can drive Live’s recording features with no mouse involved.

The Control Bar’s Arrangement Record and transport controls are mappable, as are the track Arm buttons. To record into the Session slots, you're able to map the Session Record and New buttons, each slot on its own, plus the relative navigation controls, so recording can be triggered remotely; as an example:

The Scene Up/Down Buttons.

You assign one key to advance to the next scene…

A Track Launch Button.

… while a different key both starts and stops recording in that track.

The [step recording navigators](https://www.ableton.com/en/live-manual/12/recording-new-clips/#midi-step-recording) can be mapped too.

The Step Recording Arrows.

That lets you, for instance, drive the clip’s insert marker with MIDI foot pedals, leaving both hands free to play a keyboard.

### 19.10 Capturing MIDI

Across [armed](https://www.ableton.com/en/live-manual/12/recording-new-clips/#arming-record-enabling-tracks) or [input-monitored](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#monitoring) tracks, Live constantly monitors MIDI input, and Capture MIDI pulls back whatever you've just played on them. It comes in handy when you neglected to arm the Record button before playing, or when you'd rather improvise and experiment loosely without the pressure of an active take.

The Capture MIDI Button in the Control Bar.

Press the Capture MIDI button to grab the MIDI notes you've just played.

With [Push 1](https://www.ableton.com/en/live-manual/12/using-push-1/#using-push-1) or [Push 2](https://www.ableton.com/en/live-manual/12/using-push-2/#using-push-2), fire Capture MIDI by holding the Record button while pressing the New button. With [Push 3](https://www.ableton.com/push/manual/), there's a dedicated Capture button to use instead.

How Capture MIDI acts varies with the state of the Live Set. Those varying behaviors are examined just below.

### 19.10.1 Starting a New Live Set

When the Live Set holds no other clips and the transport is stopped:

- Every monitored MIDI track gets a new clip holding the phrase you played. Bear in mind that Capture MIDI drops clips solely into whichever of the Session or Arrangement View currently has focus.
- Capture MIDI works out and sets the song tempo, fixes sensible loop boundaries, and snaps the played notes onto the grid. Note that its tempo detection lands the tempo within the 80-160 BPM range. Should you feel the material sits at a tempo beyond that span, you're free to reset the song tempo however you like. For Capture MIDI to read a phrase accurately, finishing your playing on the next bar's first beat (the “downbeat”) is advised.
- Live’s transport starts running straight away and plays the captured loop back. That gives you a chance to overdub if you'd like (overdubbing through Capture MIDI is detailed in the Adding Material to an Existing Live Set section below).
- Everything you played gets stored in the clip, with any notes preceding the detected phrase landing ahead of the clip start marker. From there you can move the start/end or loop markers to define another loop. Trimming away unwanted content beyond the set loop is as simple as right-clicking the clip and choosing the Crop Clip command.

Note: When the first captured MIDI clip holds just one note, the loop boundaries snap to that note's start and end, the tempo is computed from it, and you end up with a one, two, four, or eight bar loop. That's especially handy when triggering a rhythmic sample off a single MIDI note.

### 19.10.2 Adding Material to an Existing Live Set

When Live’s transport is already running, the Live Set holds other clips, or the tempo is [automated](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#editing-the-tempo-automation):

- Capture MIDI leaves the song tempo alone, neither detecting nor changing it. It instead relies on the current tempo to pick out a coherent musical phrase from what you played and build a loop.
- With transport running, you can “play along” with the other clips. Capture MIDI also lets you “overdub” a clip that's playing by playing over it on that same track. A press of the Capture MIDI button stacks what you just played onto the clip's existing content, so you grow your pattern one layer at a time.
- Everything you played is stored in the clip, and any notes coming before the detected phrase sit ahead of the clip start marker. That lets you move the start/end or loop markers to define a different loop.
