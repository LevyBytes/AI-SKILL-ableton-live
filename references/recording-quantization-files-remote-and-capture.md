# Recording Quantization Files Remote And Capture

Open when you need guidance on Recording Quantization Files Remote And Capture in Ableton Live.

Context: [Recording New Clips](recording-new-clips.md#19-recording-new-clips).

<a id="source-195-recording-quantized-midi-notes"></a>
### 19.5 Recording Quantized MIDI Notes

When you're about to record MIDI, there's an option to quantize the notes automatically as they go down. The Edit menu's Record Quantization chooser is where you select the meter subdivisions your captured notes will snap to. During Arrangement recording, that quantization forms its own separate step in Live’s Undo history. So if, say, you recorded with Record Quantization on “Eighth Note Triplet Quantization“ and then reconsidered, the Edit menu’s Undo command would roll back the quantization alone and leave the rest of your take untouched.

Whether in Session or Arrangement recording, the Record Quantization setting can't be altered while a take is in progress.

During overdub recording with the Clip View Loop turned on, any change to the Record Quantization applies right away and can't be undone on its own through the Edit menu command.

You can also quantize captured MIDI notes after the fact via the Edit menu’s [Quantize command](https://www.ableton.com/en/live-manual/12/editing-midi/#quantizing-notes), covered in the chapter about editing MIDI.

<a id="source-196-recording-with-count-in"></a>
### 19.6 Recording with Count-in

You configure a recording count-in through the pull-down menu beside the Metronome switch. Set to anything other than “None,“ it makes Live hold off on recording until the count-in finishes. While it runs, the Control Bar's Arrangement Position fields show the count-in in blue as bars-beats-sixteenths.

The Count-In is Displayed in the Control Bar.

The count-in counts up from negative bars-beats-sixteenths — starting at -2.1.1., say, when the Count-In setting is 2 bars — and reaches 1.1.1., where recording begins.

<a id="source-197-setting-up-file-types"></a>
### 19.7 Setting up File Types

These Settings on the Record, Warp & Launch tab govern the sample files that recording produces:

- Pick the sample file type you'd like Live to write from the File Type chooser inside the Record, Warp & Launch Settings.
- Pick the bit depth for the sample file your recording will produce from the Bit Depth chooser inside the Record, Warp & Launch Settings.

Configuring sensible defaults for your recorded clips on the Record, Warp & Launch Settings tab saves you effort. A particularly wise move is signaling the broad type of sound you'll capture by selecting a suitable default _Warp Mode_. Then, if you opt for a different song tempo afterward, Live keeps up [good sound quality](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes) on its own, generally needing no extra tweaking.

<a id="source-198-where-are-the-recorded-samples"></a>
### 19.8 Where are the Recorded Samples?

Captured samples live inside the current Set’s Project folder, specifically within Samples/Recorded. Before the Set has been saved, they sit wherever the Temporary Folder preference points, a setting located on the Settings’ File/Folder tab. So Live doesn't exhaust disk space while you record into a fresh Set, confirm that the Temporary Folder resides on a drive or partition holding enough free room.

<a id="source-199-using-remote-control-for-recording"></a>
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

<a id="source-1910-capturing-midi"></a>
### 19.10 Capturing MIDI

Across [armed](https://www.ableton.com/en/live-manual/12/recording-new-clips/#arming-record-enabling-tracks) or [input-monitored](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#monitoring) tracks, Live constantly monitors MIDI input, and Capture MIDI pulls back whatever you've just played on them. It comes in handy when you neglected to arm the Record button before playing, or when you'd rather improvise and experiment loosely without the pressure of an active take.

The Capture MIDI Button in the Control Bar.

Press the Capture MIDI button to grab the MIDI notes you've just played.

With [Push 1](https://www.ableton.com/en/live-manual/12/using-push-1/#using-push-1) or [Push 2](https://www.ableton.com/en/live-manual/12/using-push-2/#using-push-2), fire Capture MIDI by holding the Record button while pressing the New button. With [Push 3](https://www.ableton.com/push/manual/), there's a dedicated Capture button to use instead.

How Capture MIDI acts varies with the state of the Live Set. Those varying behaviors are examined just below.
