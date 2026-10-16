# Stem Separation

Open when you need guidance on Stem Separation in Ableton Live.

### 22. Stem Separation

The stem separation feature built into Live lets you pull the core components out of any recorded audio — be it a full track, a loop, or a sample — and split them into separate pieces. Once extracted, a stem behaves like every other audio clip, so you're free to warp it, slice it, reorder it, and run effects over it.

Breaking a layered recording apart into stems opens up many creative possibilities. For instance, you might pull out the vocals to build a remix or mashup, take melodies and rhythms apart, grab single instruments to sample, combine stems for a DJ set, and so on.

### 22.1 How Stem Separation Works in Live

The technique — known as well by the name _music source separation_ — examines both the spectral and temporal traits of an audio signal, then pulls out the components it identifies into pieces called _stems_.

Within Live, a deep learning model purpose-built for source separation drives this, and it has been tuned so it runs locally. As a result, you can produce stems right inside Live with no internet connection required and nothing extra to download or install.

Whether the file is mono or stereo, it can be broken into four stems: _Vocals_, _Drums_, _Bass_, and _Others_. Everything in the audio that isn't recognized as vocals, drums, or bass ends up in the Others stem.

We use songs as the running example across this chapter, yet remember that stem separation works just as well on any recorded audio you have.

### 22.2 Separating Audio Files and Clips

To separate an audio file from the browser, or to separate an audio clip out of the Session or Arrangement View, reach for the _Separate Stems to New Audio Tracks_ command, which lives in both the context menu and the Create menu.

Separating an Audio File Out of the Browser.Pulling an Audio Clip From the Session or Arrangement View.

After you pick the command, a dialog opens that presents several choices for how the separation will run.

The Separate Stems Dialog.

The Vocals, Drums, Bass, and Others toggles let you decide which parts of the song get pulled out during separation.

If you're only after a handful of elements, the _Merge to Single Track_ checkbox lets you fold the produced stems together. Switching it on collapses the chosen parts into one stem once separation finishes. Keep in mind merging applies only to two or three elements; the box stays disabled whenever a single element or all four are selected.

Use the Merge to Single Track Option to Combine Stems.

The quality mode selector lets you decide whether the run favors [speed or quality](https://www.ableton.com/en/live-manual/12/stem-separation/#separation-speed-vs-quality). _High Speed_ mode suits fast sketches and quick edits, whereas _High Quality_ mode is the choice when you need finer results.

Press the _Separate_ button to kick off the operation. Bear in mind that any playback in progress halts the moment stem separation gets underway.

Every stem that comes out lands as a clip on a track of its own, all gathered inside a fresh [Group Track](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks). Those stem clips and tracks take on the matching colors of the toggles in the stem separation dialog, and the Group Track inherits the track color of the source clip.

Separated Stems in the Arrangement View.

Pulling out just a single part of the song — the vocals, say — yields a lone track holding the stem clip rather than a Group Track.

With the Merge to Single Track option in play, the produced stem goes onto a new track, and both that track and the stem clip adopt the color of the source track.

A Merged Stem in the Arrangement View.

A few clip settings come into play when you separate a clip out of the Arrangement or Session View, shaping which slice of the audio gets handled. Should you move a clip's [start and end markers](https://www.ableton.com/en/live-manual/12/clip-view/#clip-and-loop-region-settings) in the Clip View ahead of separation, the stems will cover only the audible span those markers mark out. In the same way, when you [loop a warped clip](https://www.ableton.com/en/live-manual/12/clip-view/#looping-clips), processing spans from the start marker up through whatever loop region is active.

How the Active Clip Region and Loop Govern the Audio Portion That Gets Separated.

Separation can also target a time selection inside an Arrangement clip. To set that up, drag out a time selection across a clip in the Arrangement View; afterward, right-click the clip and choose _Separate Stems for Time Selection_. The very same Separate Stems dialog covered earlier appears. As soon as you hit _Separate_, the clip gets cut at the boundaries of your selection and stems are produced only for that slice of audio.

Separating the Audio That Falls Within a Clip Time Selection in the Arrangement View.

Rather than being baked into the processed stem audio, any audio effects belonging to the source track move onto the Group Track. On top of that, track automation gets duplicated onto the new Group Track, whereas clip envelope automation and modulation are duplicated onto the separate stem clips.

After the stems exist, Live switches off the source clip so the output isn't doubled. To turn it back on, select the clip and tap the 0 key.

When you invoke the Separate Stems to New Audio Tracks command on a song or sample in the browser, where the stems land — Session or Arrangement View — follows whichever view currently has focus. Should the Set be empty, the project tempo shifts to align with the source audio's tempo, provided [warping for samples](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping-options-in-settings) is turned on in Live's Record, Warp & Launch Settings.

Live keeps the audio files for separated stems inside the Current Project folder, at Samples → Processed → Stems. Whenever the Merge to Single Track option was applied, a file is generated for every individual stem plus one more for the merged stem. The file type chosen in the Record, Warp & Launch Settings governs the format of the separated stems. Each one carries a 44.1 kHz sample rate along with a bit depth that matches the original material.

### 22.2.1 Separation Speed vs. Quality

The Separate Stems dialog offers a pair of quality modes to pick from: _High Speed_ and _High Quality_. Your pick decides whether the run leans toward being quick or being accurate.

Pick High Speed and the run finishes sooner, although on aging setups it can still run a few minutes. Here, every stem comes out together in one pass.

Pick High Quality and accuracy rises — reflected in a stronger Signal-to-Distortion Ratio (SDR) score — but the trade-off is a longer run. In this mode the Vocals, Drums, and Bass elements each get their own separation pass. Afterward, the Others stem is assembled from whatever audio is left once those three passes finish.

No matter which mode you pick, trimming the sample ahead of separation cuts down the processing time. When you need stems from one part of a song only — the chorus, for instance — you can [shorten the clip](https://www.ableton.com/en/live-manual/12/clip-view/#cropping-clips) to that span with the _Crop Clip Sample to Time Selection_ command found in the Sample Editor. Cropping a clip from a time selection in the Arrangement is also an option, done through the _Crop Clip_ command in a track's context menu. Both Crop commands share the same shortcut, Ctrl+Shift+J (Win) / Cmd+Shift+J (Mac).

In High Quality mode, picking out only the stems you actually need trims the processing time too. When the goal is to isolate, say, the drums and vocals from a song, producing every stem is unnecessary. That said, including the Others element doesn't save you any separation time. Then every part still has to run so that the leftover audio separates correctly. Take separating Vocals and Others as a case: the Drums and Bass stems get produced as well. The Set receives only the Vocals and Others stems, while the Drums and Bass ones land in the Stems folder inside the Current Project.

Broadly, how long separation takes hinges heavily on your system setup. On older Windows machines and Intel Macs the operation can drag, since only the CPU does the work — unlike Macs running Apple silicon, where the GPU is used.

Given how the separation works, now and then you'll spot bits of audio landing in stems you wouldn't have predicted. Hi-hat high frequencies might surface in the Others stem, or chorus-laden synth tones might come through in the Vocals stem. Several factors can produce this bleed between stems, among them the quality mode in use and the tonal makeup of the source. Based on what you intend to do with the stems, it's worth separating a song once in High Speed mode and then a second time in High Quality mode to find which output sits best with that source material.
