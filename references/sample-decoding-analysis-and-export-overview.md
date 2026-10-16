# Sample Decoding Analysis And Export Overview

Open when you need guidance on Sample Decoding Analysis And Export Overview in Ableton Live.

Context: [Sample Files](managing-files-and-sets.md#51-sample-files).

<a id="source-511-the-decoding-cache"></a>
### 5.1.1 The Decoding Cache

So that processing power isn't wasted, the decoded versions of compressed samples are held by Live in the _cache_. You rarely have to tend to it yourself, since Live clears out the older entries on its own to free space for fresh ones. Still, the File & Folder Settings’ Decoding Cache section lets you cap how big it gets. It stays within the Maximum Cache Size setting and always preserves the Minimum Free Space on the hard disk. Hitting the adjacent Cleanup button removes every file that the current Live Set isn't relying on.

Settings for the Decoding Cache.

<a id="source-512-analysis-files-asd"></a>
### 5.1.2 Analysis Files (.asd)

The first time a sample enters the program, Live generates a small companion called an _analysis file_. Inside it sits information Live collected to sharpen stretching quality, render the waveform faster, and work out the tempo of [long samples](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#auto-warping-long-samples) on its own.

Bringing a lengthy sample into a project may prompt Live to report that playback has to wait until analysis finishes. That message stays away when the clip has already gone through analysis (meaning Live locates an analysis file for it), or when the Record, Warp & Launch Settings’ Auto-Warp Long Samples preference has been switched off.

Beyond that, the _default clip settings_ for a sample can be kept in an analysis file:

A press of the Clip View’s [Save button](https://www.ableton.com/en/live-manual/12/clip-view/#saving-default-audio-clip-settings-with-the-sample) commits the present clip’s settings into the sample’s analysis file. When you later drag that sample back into Live, every one of its clip settings comes along untouched. It's an especially handy way to keep Warp Marker settings tied to the sample. Tucking default clip settings into the analysis file should not be confused with saving the clip as a Live Clip.

Analysis files conveniently hold the default values for a given sample, yet remember that every clip in a Live Set may carry its own distinct settings — even when several clips point at the very same sample on disk. That said, dragging a _new_ copy of the sample into a Live Set makes Live apply whatever the analysis file holds to that freshly made clip.

Each analysis file carries the name of the sample it belongs to, plus a tacked-on “.asd“ extension, and Live drops it into the very folder where the sample resides.

Samples accompanied by an .asd file show up this way in the browser.

Samples lacking an .asd file appear like this instead.

The analysis files on their own stay hidden from Live’s browser.

Keep in mind that switching off the Create Analysis Files option in the File & Folder Settings stops these .asd files from being generated. Should an .asd file go missing, Live can rebuild everything apart from the default clip settings, though doing so takes a while with longer samples.

<a id="source-513-exporting-audio-and-video"></a>
### 5.1.3 Exporting Audio and Video

Through the File menu’s _Export Audio/Video_ command you can render Live’s audio output into fresh samples. Those files might go onto an audio CD for playback, or onto a data CD that backs up your project or feeds other digital audio software. When your Set carries video, the same Export Audio/Video command writes a new video file alongside the rendered audio in that same directory.
