# Resampling And Internal Routing Overview

Open when you need guidance on Resampling And Internal Routing Overview in Ableton Live.

Context: [Routing and I/O](routing-and-i-o.md#17-routing-and-io).

<a id="source-174-resampling"></a>
### 17.4 Resampling

You can feed Live’s Main output into a single audio track and record it — in other words, resample it. Resampling makes for an enjoyable and handy technique, since it turns whatever is happening right now in a Live Set into samples you can fold back in straight away. It serves for capturing tracks loaded with CPU-hungry devices so those devices can be removed afterward, or for a fast preview ahead of [rendering to disk](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video).

Selecting the “Resampling“ option in any audio track’s Input Type chooser steers the Main output onto that track. From there you settle on precisely what to resample, muting, soloing, or otherwise tweaking the tracks that feed the Main output. It is wise to watch the Main Volume meter so your level stays as hot as it can without clipping (shown by red in the meter). After that, arm the track and record into one of its [empty clip slots](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-into-session-slots). Bear in mind that the recording track’s own output stays muted throughout resampling and is left out of the recording.

Whatever samples resampling produces land inside the current Set’s [Project folder](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-projects), within Samples/Recorded. As long as the Set stays unsaved, they sit instead at the spot named by the [Temporary Folder](https://www.ableton.com/en/live-manual/12/recording-new-clips/#where-are-the-recorded-samples).

<a id="source-175-internal-routings"></a>
### 17.5 Internal Routings

Both Live’s mixer and its external routing devices make inter-track routings possible. While such routings can be a bit bewildering, they unlock a wealth of useful creative and technical possibilities. Through the mixer, inter-track routing happens in two ways:

1. Track A is configured to push its output signal over to Track B. That works because any track able to accept an output signal of the right type from Track A turns up in its Output Type chooser.
2. Track B is configured to pull its input signal from Track A. That works because any track furnishing a signal of the right type shows up in Track B’s Input Type chooser.
   Two Ways to Route Track A into Track B.

Either route ends with Track A’s output flowing into Track B. Approach 1 keeps Track B’s in/out settings untouched and, whenever we like, lets us bring in further tracks that send their output into Track B. It is the go-to technique for “many-to-one“ routings — submixes, say, or a handful of MIDI tracks driving the same instrument. Here, soloing Track B still lets you hear the output of every track feeding it. You can equally solo Track A and hear its output signal. When you do, all the other tracks fall silent, even the ones that may also feed Track B. Strictly speaking, what reaches your ears is Track B’s output stripped of everything but Track A’s signal.

Approach 2, by contrast, leaves Track A untouched apart from Track B tapping its output. Adding more tracks akin to Track B, each tapping Track A’s output, is just as easy. Layering instruments is a fine illustration of this kind of “one-to-many“ routing arrangement.
