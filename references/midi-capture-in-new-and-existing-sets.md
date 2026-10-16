# MIDI Capture In New And Existing Sets

Open when you need guidance on MIDI Capture In New And Existing Sets in Ableton Live.

Context: [Capturing MIDI](recording-new-clips.md#1910-capturing-midi).

<a id="source-19101-starting-a-new-live-set"></a>
### 19.10.1 Starting a New Live Set

When the Live Set holds no other clips and the transport is stopped:

- Every monitored MIDI track gets a new clip holding the phrase you played. Bear in mind that Capture MIDI drops clips solely into whichever of the Session or Arrangement View currently has focus.
- Capture MIDI works out and sets the song tempo, fixes sensible loop boundaries, and snaps the played notes onto the grid. Note that its tempo detection lands the tempo within the 80-160 BPM range. Should you feel the material sits at a tempo beyond that span, you're free to reset the song tempo however you like. For Capture MIDI to read a phrase accurately, finishing your playing on the next bar's first beat (the “downbeat”) is advised.
- Live’s transport starts running straight away and plays the captured loop back. That gives you a chance to overdub if you'd like (overdubbing through Capture MIDI is detailed in the Adding Material to an Existing Live Set section below).
- Everything you played gets stored in the clip, with any notes preceding the detected phrase landing ahead of the clip start marker. From there you can move the start/end or loop markers to define another loop. Trimming away unwanted content beyond the set loop is as simple as right-clicking the clip and choosing the Crop Clip command.

Note: When the first captured MIDI clip holds just one note, the loop boundaries snap to that note's start and end, the tempo is computed from it, and you end up with a one, two, four, or eight bar loop. That's especially handy when triggering a rhythmic sample off a single MIDI note.

<a id="source-19102-adding-material-to-an-existing-live-set"></a>
### 19.10.2 Adding Material to an Existing Live Set

When Live’s transport is already running, the Live Set holds other clips, or the tempo is [automated](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#editing-the-tempo-automation):

- Capture MIDI leaves the song tempo alone, neither detecting nor changing it. It instead relies on the current tempo to pick out a coherent musical phrase from what you played and build a loop.
- With transport running, you can “play along” with the other clips. Capture MIDI also lets you “overdub” a clip that's playing by playing over it on that same track. A press of the Capture MIDI button stacks what you just played onto the clip's existing content, so you grow your pattern one layer at a time.
- Everything you played is stored in the clip, and any notes coming before the detected phrase sit ahead of the clip start marker. That lets you move the start/end or loop markers to define a different loop.
