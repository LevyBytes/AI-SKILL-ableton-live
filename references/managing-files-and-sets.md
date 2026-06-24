# Managing Files And Sets (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 5. Managing Files and Sets

Producing music in Live draws on several kinds of files: some hold [MIDI](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#midi-files) or [audio](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#sample-files), while others are particular to the application itself, like [Live Clips](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-clips) and [Live Sets](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-sets). The pages ahead cover how to handle every one of these file types when you work inside Live.

### 5.1 Sample Files

Any file holding audio data counts as a _sample_. Playback in Live covers uncompressed types (WAV, AIF and Sound Designer II for Mac) along with compressed ones (MP3, AAC, Ogg Vorbis, Ogg FLAC and FLAC).

Because samples stream straight off the disk during playback, even a hefty collection of sizeable samples won't bump up against your RAM ceiling. Be aware, though, that throughput trouble can surface when a drive sits almost full or (under Windows) is badly fragmented. The spin rate of a hard drive likewise plays a part in how well the disk performs. The section about [managing the disk load](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#managing-the-disk-load) has further detail.

Uncompressed mono and stereo samples can be mixed together in Live regardless of their duration, sample rate or bit depth, and no conversion step is needed beforehand. When a compressed sample is involved, Live first decodes it and saves a temporary, uncompressed copy. The decode is generally fast enough that playback starts almost immediately, so there's no need to sit through the whole process.

Note: Should you bring a lengthy sample into a project, Live may warn that playback isn't possible until analysis has run. The [analysis](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#analysis-files-asd) section explains why.

### 5.1.1 The Decoding Cache

So that processing power isn't wasted, the decoded versions of compressed samples are held by Live in the _cache_. You rarely have to tend to it yourself, since Live clears out the older entries on its own to free space for fresh ones. Still, the File & Folder Settings’ Decoding Cache section lets you cap how big it gets. It stays within the Maximum Cache Size setting and always preserves the Minimum Free Space on the hard disk. Hitting the adjacent Cleanup button removes every file that the current Live Set isn't relying on.

Settings for the Decoding Cache.

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

### 5.1.3 Exporting Audio and Video

Through the File menu’s _Export Audio/Video_ command you can render Live’s audio output into fresh samples. Those files might go onto an audio CD for playback, or onto a data CD that backs up your project or feeds other digital audio software. When your Set carries video, the same Export Audio/Video command writes a new video file alongside the rendered audio in that same directory.

#### 5.1.3.1 Selection Options

The Render Dialog’s Selection Options.

Within the Export dialog, the Rendered Track chooser presents a handful of choices regarding which audio signal gets rendered:

The Rendered Track Chooser.

- _Main_ — Live’s Main output taken post-fader. As long as you're listening to the Main output, the rendered file is guaranteed to match precisely what reaches your ears.
- _All Individual Tracks_ — Each track's post-fader output, return tracks and instrument-bearing MIDI tracks included. A distinct sample comes out of Live for every track, and since they all share one length, lining them up in other multitrack software is straightforward.
- _Selected Tracks Only_ — Behaves just like the All Individual Tracks choice, except it limits rendering to the tracks you had selected before the Export dialog opened.
- _(single tracks)_ — The post-fader output coming from whichever track is selected.

Where the exported material starts and how long it runs is governed by the remaining Selection fields:

- _Render Start_ — Fixes the spot where rendering kicks off.
- _Render Length_ — Sets how long the rendered sample runs.

Tip: To fill in both the Render Start and Length values quickly, highlight a time span in the Arrangement View before you reach for the Export Audio/Video command. Bear in mind, though, that a rendered audio file holds nothing beyond what you actually heard going in. If, say, you were running a mix of Session View clips together with Arrangement material, that combination is exactly what lands in the rendered file — no matter which view happens to be open at render time.

#### 5.1.3.2 Rendering Options

Audio Rendering Options.

A number of audio rendering options live in the Export dialog:

- _Include Return and Main Effects –_ Turning this on has Live render each chosen track one by one together with whatever return tracks that track feeds, plus the effects sitting on the Main track. It comes in handy for prepping material for a live show, or for handing stems off to a mixing engineer or remix artist.
- _Render as Loop_ — With this enabled, Live produces a sample suited to looping. Picture a Live Set that runs a delay effect: when Render as Loop is active, Live performs the render in two passes. The first pass writes no samples to disk but applies the chosen delay effect. Once the second pass begins committing audio to disk, it folds in the delay “tail“ carried over from the first pass.
- _Convert to Mono_ — Enabling this makes Live output a mono file rather than a stereo one.
- _Normalize_ — When this is on, the sample that emerges from rendering gets normalized — that is, the file is boosted until its loudest peak reaches the full available headroom.
- _Create Analysis File_ — Switch this on and Live writes an .asd file holding analysis details for the rendered sample. Tick it whenever you plan to bring the new sample back into Live.
- _Sample Rate_ — Here's how your sample-rate pick behaves: choosing a rate that matches or exceeds the one your project runs at (set in the Audio tab of Live’s Settings) lets Live export in a single pass at the rate you picked in the Export dialog. Pick a rate _lower_ than your project's current sample rate and Live exports first at the project rate, then downsamples in a second pass with a high-quality process. Expect this to take a brief moment.

#### 5.1.3.3 Encoding Options

Audio Encoding Options.

- _Encode PCM_ — Switching this on yields a lossless audio file.
- _File Type_ — PCM export can be written as WAV, AIFF, and FLAC formats.
- _Bit Depth,\*\*Dither Options_ — Whenever your render uses a bit depth below 32-bit, pick one of the dither modes. Dithering layers a faint bit of noise over the rendered audio while cutting down the artifacts that come from lowering the bit depth. Triangular is the preset choice and the “safest“ pick if there's any chance you'll process the file further. Rectangular mode adds even less dither noise, though it trades that for extra quantization error. The trio of Pow-r modes ramp up the dithering by degrees while shoving the noise beyond the audible range. Bear in mind that dithering ought to touch a given audio file only one time. When more processing lies ahead for your rendered file, rendering to 32-bit is the better route so you can skip dithering for now. The Pow-r modes in particular have no business on anything bound for a later mastering stage — reserve them strictly for final output.
- _Encode MP3_ — Switching this on produces a CBR 320 kbps MP3 file. PCM and MP3 can be exported together at once. Leave both toggles off and the Export button goes inactive.

#### 5.1.3.4 Video Rendering Options

Video Rendering Options.

On top of the audio-rendering controls, the Export dialog hands you extra options for rendering video:

- _Create Video_ — Turn this on and a video file lands in the same directory as your rendered audio. Keep in mind it's only selectable when video clips sit in the Arrangement View. What's more, you can't render video by itself — switching video rendering on always yields a video on top of the rendered audio.
- _Video Encoder_ — Through this chooser you pick which encoder handles the video render. The options on offer here hinge on the encoders already installed.
- _Video Encoder Settings_ — Hitting this button brings up the settings window belonging to the chosen encoder. The available settings shift according to which encoder you selected. Some encoders expose nothing for the user to adjust, and then the Edit button stays inactive.

After your choices are set and you press Export to set things in motion, the audio render runs first. The video render follows once the audio finishes. Be aware that, according to which encoder is in play, video rendering might run across several passes. A progress bar from Live keeps you posted on where the process stands.

So long as no custom window size or aspect ratio was set in the encoder settings, the finished video file plays back just the way it looked during real time playback in Live. That video file holds the rendered audio as well.

The [Working with Video](https://www.ableton.com/en/live-manual/12/working-with-video/#working-with-video) chapter goes deeper into handling video inside Live.

#### 5.1.3.5 Real-Time Rendering

As a rule, rendering takes place offline. Things shift, though, when your Set holds an [External Audio Effect](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#external-audio-effect) or [External Instrument](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#external-instrument) that sends signal out to a hardware effects unit or synthesizer. Under those conditions, the Main output gets rendered in real time. While rendering single tracks, any track whose signal path never touches an external device is rendered offline, after which the tracks that do reach such devices render in real time. Live follows each track’s signal flow on its own and works out whether real-time rendering is called for. A set of options then greets you as the render starts:

Waiting for External Devices to Become Silent.

- _Skip_ — Out of the box, Live holds off ten seconds before a real-time render gets going. That pause gives any lingering sound from external devices room to die away, but when you want longer (say you're letting a drawn-out reverb tail finish), type a fresh number into the number box to extend it. Conversely, if you know your external devices are dead quiet, pressing “Skip,“ launches the render right away and moves things along.

Once rendering is underway, the dialog switches over to display a recording progress bar:

Real-Time Rendering in Progress.

- _Auto-Restart on drop-outs_ — A real-time render leans on a bit more CPU than its non-real-time counterpart, so now and then drop-outs (tiny gaps or glitches in the sound) may creep in. Live notices when a drop-out occurs, and with the Auto-Restart option turned on, rendering kicks off afresh from the top.
- _Restart_ — Kicks off the rendering process again by hand.
- _Cancel_ — Halts the rendering process and discards the file rendered so far.

Should there have been more than one try, the dialog box also shows the tally of rendering attempts. When dropouts and restarts won't stop, shutting down other open applications frees up processing power for the render. The chapter on [computer audio resources](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#computer-audio-resources-and-strategies) holds further pointers for boosting performance.

### 5.2 MIDI Files

Inside a _MIDI file_ are instructions that drive MIDI compatible synthesizers or instruments — Live’s Simpler among them — to produce a particular musical result. Both hardware and software MIDI sequencers can export them. Pulling a MIDI file into Live differs from how samples behave: its data folds straight into the Live Set, and the MIDI clips that result keep no tie back to the original file. A distinctive icon marks MIDI files in the browser.

A MIDI File in the Browser.

Importing MIDI files happens either through the browser or via the Create menu’s Import MIDI File… command. Run the Import MIDI File… command from the Arrangement View and the file drops in at the Insert Marker position. Issue it from the Session View instead and the file goes into whichever clip slot is currently selected.

### 5.2.1 Exporting MIDI Files

MIDI clips in Live may be written out as Standard MIDI files. The route to exporting one is the File menu’s Export MIDI Clip command, which brings up a file-save dialog where you pick where the new MIDI file should land.

Exporting to a MIDI file is not the same thing as saving the clip as a Live Clip.

### 5.3 Live Clips

Single audio or MIDI clips may be saved to disk as Live Clips, making them simple to call up and reuse across any project. Since an audio clip merely points to samples on disk instead of carrying the audio data itself, it stays tiny, so growing and tending your own library is no trouble.

Saving a clip out of the open Live Set is as easy as dragging it onto the Places section of the browser and dropping it in the Current Project or any user folder. With audio clips, Live takes care of copying the clip’s sample into that new spot according to what's picked in the [Collect Files on Export](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#collect-files-on-export) chooser. From there you may enter your own name for the clip or accept Live’s proposed one by pressing Enter.

A Live Clip in the Browser.

Live Clips make an excellent vault for ideas you mean to revisit or build on later, because they preserve not just the source clip with every one of its clip and envelope settings, but the source track’s devices too. To rebuild a Live Clip’s device chain, drop it either onto a track that holds no clips or devices, or into the empty area of the Session or Arrangement View where no tracks sit. Bear in mind that a Live Clip dragged onto a track that already carries devices or clips arrives with its clip settings but leaves its devices behind. As an example, you might drop a bassline Live Clip onto an existing track already running a bass instrument instead of spinning up a new track.

Any clips that live inside Live Sets already saved to disk count as Live Clips as well. The section about [merging Sets](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#merging-sets) covers more on the subject.

Keep in mind that tucking default clip settings into a sample’s analysis file is a separate matter from saving a Live Clip. The default clip held in the .asd file tags the sample with reasonable default values (warp, gain and pitch settings) so it behaves predictably the moment it joins a Set. Live Clips, by contrast, sit on disk as standalone musical ideas. You might, for instance, spin off several variants of one audio clip using assorted warp, pitch, envelope and effect settings, then save each as its own Live Clip. The browser then lets you sort and preview those clips one by one, despite every one of them pointing at the same source sample.

### 5.4 Live Sets

Whatever you build and edit in Live is a document known as a _Live Set_. Picture it as one “song.“ A Set has to be saved within a project so that Live can track and oversee every piece making up the Live Set: Live Clips, device presets, whatever samples are in play, and so on.

### 5.4.1 Creating, Opening and Saving Sets

Fresh Live Sets come from the File menu’s New Live Set command, while the Open Live Set or Open Recent Set command brings up existing ones. From the browser, a double-click on a Live Set, or pressing Enter on it, opens it as well.

The File menu’s Save Live Set command stores the current Live Set precisely as it stands, clips and settings and all.

To save the current Live Set under another name and/or in another directory location, reach for the Save Live Set As command; the Save a Copy command instead spawns a duplicate of the current Live Set bearing a new name and/or new directory location.

### 5.4.2 Accessing a Set’s Undo History

Every action carried out since a Set was opened shows up in the Undo History, which can roll them back or restore them up to any chosen point. Reversing or recovering a whole batch of actions in one move is therefore simple, with no need to undo or redo each step on its own.

Bring up the Undo History by picking the _Undo History_ entry from the View menu, or with the shortcut CtrlAltZ (Win) / CmdOptionZ (Mac).

The Undo History for a Set.

After it opens, the actions appear in the sequence they happened, newest sitting at the top and oldest at the bottom. To roll the Set back to a given action in its history, pick that action by clicking it or by stepping to it with the up and down arrow keys and hitting Enter. Whatever actions sit above the one you chose turn grey, signalling that they've been undone, while the actions beneath it stay live since their changes are still in force. Choosing a greyed-out action reinstates it together with any other undone actions sitting below it.

Be aware that closing a Set discards its Undo History rather than storing it, and the list resets whenever the Set is opened again. Live regards creating or opening a Set as the opening entry in the Undo History, which is why that step can't be undone.

### 5.4.3 Merging Sets

Merging Sets is painless in Live, which proves useful for pulling together work from separate versions or pieces. To bring every track (the return tracks aside) of one Live Set into another, drag the Set out of the browser into the current Set and drop it on any track title bar or onto the drop area beside or beneath the tracks. The tracks from the dropped Set are rebuilt in full — their Session and Arrangement View clips, their devices, and their automation all carry over.

The Session View zone where Live Sets are dropped to import them.The Arrangement View zone for dropping Live Sets to import them.

When you'd rather grab single tracks out of a Set, the Live Set can be unfolded inside the browser exactly as though it were a folder.

Unfolding a Set to Reveal its Contents.

At this point you can drag those individual tracks and drop them following the method laid out at the start of this section. Whatever [grooves](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves) were saved alongside your Set also turn up as a folder inside the unfolded Set.

Should you be after only the device chain — say a device plus its audio or MIDI effects — from another Set, drag the Devices icon out of that Set in the browser.

The Devices Icon in an Expanded Live Set.

Dragging [Group Tracks](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks) and nested Group Tracks straight from Live’s browser works too. Group Tracks open up in the browser, which lets you pull a single track out from inside.

Beyond unfolding Sets themselves, you can open up the tracks within them to reach the individual Session View clips that were placed on the track:

Revealing the Session View Clips Contained in a Set.

Session View clips from the Set can be browsed, previewed and imported just as if each had been kept as its own Live Clip. The upshot is that any Live Set may act as a sound pool for any other, inviting creative reuse and crossover.

### 5.4.4 Exporting Session Clips as New Sets

A group of Session View clips can become a brand-new Live Set when you drag them onto the browser. Begin by selecting several Session View clips at once — click and drag, or hold the Shift or Ctrl (Win) / Option (Mac) modifiers. With your selection made, drop those clips onto the Current Project or some user folder; there you'll either accept the name Live proposes or supply your own.

### 5.4.5 Template Sets

Reach for the File menu’s Save Live Set As Default Set… command to store the current Live Set as your default template. From then on Live treats those settings as the starting, default state every new Live Set inherits. This lets you set up in advance:

- The way your multichannel input/output is arranged.
- Ready-made devices such as EQs and Compressors sitting in each track.
- [Computer key mappings](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control).
- [MIDI mappings](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-remote-control).

Keep in mind that any template Set shown in Live’s browser may be promoted to the default Live Set through the Set Default Live Set entry, found in the Set’s context menu or the File menu.

Beyond that single default template, you're free to build extra template Sets aimed at different kinds of projects, each carrying its own distinct layout of tracks, devices, and the like. The way to do this is to save the current Live Set with the File menu’s Save Live Set As Template… command. Whatever you save this way shows up in the browser’s Templates category and in the User Library's Templates folder. That Templates folder under the User Library springs into existence on its own the first time a template Set is saved. These Sets behave as templates from then on: they open with the configuration you stored but carry the name Untitled.als, primed to serve as a new Set.
