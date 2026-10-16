# Audio Clip Warp Reverse And Playback

Open when you need guidance on Audio Clip Warp Reverse And Playback in Ableton Live.

Context: [Audio Utilities Panel](clip-view.md#84-audio-utilities-panel).

<a id="source-841-warp-controls"></a>
### 8.4.1 Warp Controls

Live provides several controls for fine-tuning the time-warping engine toward [optimal stretching quality](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes).

The Warp Controls.

With the Warp toggle off, Live sounds the sample at its native tempo, paying no mind to the present Live Set tempo. That suits samples lacking any built-in rhythmic structure: percussion hits, atmospheres, sound effects, spoken word and similar material. Flip the Warp toggle on to keep rhythmically structured samples (sample loops, music recordings, full music pieces, and so on) locked to the present song tempo. The speed of a warped sample tracks the tempo as you adjust the Control Bar’s Tempo control.

The Control Bar’s Tempo Field.

To warp accurately, Live has to understand the sample’s metrical structure. With loops that are prepared well, tempo and duration come out automatically; usually that’s precise enough for the sample to be ready for use in Live right away. Other samples may need a few hints from you.

<a id="source-842-reversing-samples"></a>
### 8.4.2 Reversing Samples

Pressing the Reverse button produces a fresh sample by flipping the sample that the current clip points to.

The Reverse Button.

Take this route and Live reapplies the former clip’s settings (following the rules laid out below) and swaps the original sample for a new, reversed one inside the Clip View. After you save the Live Set, that new sample lives in the Set’s Project folder, under Samples/Processed/Reverse. Before the Set is saved, new samples sit at whatever spot is named as the Temporary Folder in Live’s Settings.

A handful of rules govern the reversing process. First, any Warp Markers stay pinned to their spots _in the sample_. So a Warp Marker on the downbeat of a clip’s second bar lands on the downbeat of the second-to-last bar once reversed. Clip loop/region settings flip in much the same way. Second, clip envelopes hold their place _in time_. Hence a mixer volume envelope that pulls down the volume across a clip’s first half keeps doing precisely that following reversal.

Reversing runs fairly quickly (roughly as quick as copying), though very long samples may take a moment. Should that happen, a progress bar appears in Live’s Status Bar, and further actions in the program lock up briefly (although clips already playing keep going). The instant Live starts drawing a new waveform into the Sample Editor, you can play the reversed clip and carry out other actions in the program. After a sample has been reversed, Live retains data on both the original and reversed versions right up until the program is shut. Consequently, flipping the sample back to the original and then reversing it once more happens instantly.

Reversing several clips at once isn’t possible in the Session View. Within the Arrangement View, though, you can reverse a chunk of material even if it spans multiple clips. To pull this off, mark the time range you wish to reverse and pick the Reverse Clip(s) command from the clip’s context menu, or tap the R shortcut key.

Reversing clips during a live performance isn’t advised, since a faint audio glitch may now and then crop up while Live reapplies the warp and loop settings.

<a id="source-843-destructive-sample-editing"></a>
### 8.4.3 Destructive Sample Editing

Pressing the Edit button launches the sample in an outside sample editing application, the one you designate under the File & Folder Settings.

The Launch Sample Editor Button.

Working a sample in an external program means you must halt Live’s playback. Upon returning to Live, the edited rendition of the sample plays back. The present set of Warp Markers survives only when the sample length stays identical to what it was before editing.

Keep in mind that edits to one sample can ripple through other clips that draw on the same sample.

<a id="source-844-clip-start-and-end-fades"></a>
### 8.4.4 Clip Start and End Fades

Switched on, the Clip Fade toggle lays a brief fade across the clip start and end to head off clicks at the clip edges. How long that fade lasts depends on the signal and spans 0-4 milliseconds.

The Clip Fade Toggle.

Keep in mind the toggle exists solely for clips in Session View. Over in Arrangement View, [clip fades](https://www.ableton.com/en/live-manual/12/arrangement-view/#audio-clip-fades-and-crossfades) get tuned through envelopes.

For every new clip, the Clip Fade toggle sits on by default whenever the Create Fades on Clip Edges option is switched on under the Record, Warp & Launch Settings.

Automatically Create Short Fades At Clip Edges.

<a id="source-845-clip-ram-mode"></a>
### 8.4.5 Clip RAM Mode

Switching on the RAM Mode toggle has Live pull the audio that the clip points to into the computer’s memory instead of streaming it off disk as it plays.

The RAM Mode Toggle.

RAM Mode can address these situations:

- Your computer’s hard disk runs too slowly to feed audio across as many tracks as you’d like in real time. For deeper detail on disk-related trouble, head to [Managing the Disk Load](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#managing-the-disk-load).
- You run into audio dropouts while playing clips in [Legato Mode](https://www.ableton.com/en/live-manual/12/launching-clips/#legato-mode).

Your computer leans on the hard disk to swap out RAM contents left idle for a stretch. The greater the count of clips you keep in RAM Mode, the likelier they are to be swapped out. Live copes with disk overloads more gracefully than with swapped-out audio that shows up late: a disk overload brings unwanted mutes, while a RAM overload brings both mutes and rhythmic “hiccups.“

<a id="source-846-high-quality-interpolation"></a>
### 8.4.6 High Quality Interpolation

With the High Quality toggle switched on, Live applies a sophisticated sample-rate conversion algorithm that yields finer sound quality while drawing more CPU load.

The High Quality Toggle.

<a id="source-clip-view-part-2"></a>

Running a sample through the Hi-Q algorithm yields lower distortion — most noticeably in the upper frequency range — whenever you transpose it or reconcile an imported file’s sampling rate with the rate your system uses. While this mode is active, you can shift a sample by about 19 semitones up or down before audible aliasing tends to creep in.
