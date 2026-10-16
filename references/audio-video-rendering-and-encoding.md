# Audio Video Rendering And Encoding

Open when you need guidance on Audio Video Rendering And Encoding in Ableton Live.

Context: [Exporting Audio and Video](managing-files-and-sets.md#513-exporting-audio-and-video).

<a id="source-5131-selection-options"></a>
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

<a id="source-5132-rendering-options"></a>
#### 5.1.3.2 Rendering Options

Audio Rendering Options.

A number of audio rendering options live in the Export dialog:

- _Include Return and Main Effects –_ Turning this on has Live render each chosen track one by one together with whatever return tracks that track feeds, plus the effects sitting on the Main track. It comes in handy for prepping material for a live show, or for handing stems off to a mixing engineer or remix artist.
- _Render as Loop_ — With this enabled, Live produces a sample suited to looping. Picture a Live Set that runs a delay effect: when Render as Loop is active, Live performs the render in two passes. The first pass writes no samples to disk but applies the chosen delay effect. Once the second pass begins committing audio to disk, it folds in the delay “tail“ carried over from the first pass.
- _Convert to Mono_ — Enabling this makes Live output a mono file rather than a stereo one.
- _Normalize_ — When this is on, the sample that emerges from rendering gets normalized — that is, the file is boosted until its loudest peak reaches the full available headroom.
- _Create Analysis File_ — Switch this on and Live writes an .asd file holding analysis details for the rendered sample. Tick it whenever you plan to bring the new sample back into Live.
- _Sample Rate_ — Here's how your sample-rate pick behaves: choosing a rate that matches or exceeds the one your project runs at (set in the Audio tab of Live’s Settings) lets Live export in a single pass at the rate you picked in the Export dialog. Pick a rate _lower_ than your project's current sample rate and Live exports first at the project rate, then downsamples in a second pass with a high-quality process. Expect this to take a brief moment.

<a id="source-5133-encoding-options"></a>
#### 5.1.3.3 Encoding Options

Audio Encoding Options.

- _Encode PCM_ — Switching this on yields a lossless audio file.
- _File Type_ — PCM export can be written as WAV, AIFF, and FLAC formats.
- _Bit Depth,\*\*Dither Options_ — Whenever your render uses a bit depth below 32-bit, pick one of the dither modes. Dithering layers a faint bit of noise over the rendered audio while cutting down the artifacts that come from lowering the bit depth. Triangular is the preset choice and the “safest“ pick if there's any chance you'll process the file further. Rectangular mode adds even less dither noise, though it trades that for extra quantization error. The trio of Pow-r modes ramp up the dithering by degrees while shoving the noise beyond the audible range. Bear in mind that dithering ought to touch a given audio file only one time. When more processing lies ahead for your rendered file, rendering to 32-bit is the better route so you can skip dithering for now. The Pow-r modes in particular have no business on anything bound for a later mastering stage — reserve them strictly for final output.
- _Encode MP3_ — Switching this on produces a CBR 320 kbps MP3 file. PCM and MP3 can be exported together at once. Leave both toggles off and the Export button goes inactive.

<a id="source-5134-video-rendering-options"></a>
#### 5.1.3.4 Video Rendering Options

Video Rendering Options.

On top of the audio-rendering controls, the Export dialog hands you extra options for rendering video:

- _Create Video_ — Turn this on and a video file lands in the same directory as your rendered audio. Keep in mind it's only selectable when video clips sit in the Arrangement View. What's more, you can't render video by itself — switching video rendering on always yields a video on top of the rendered audio.
- _Video Encoder_ — Through this chooser you pick which encoder handles the video render. The options on offer here hinge on the encoders already installed.
- _Video Encoder Settings_ — Hitting this button brings up the settings window belonging to the chosen encoder. The available settings shift according to which encoder you selected. Some encoders expose nothing for the user to adjust, and then the Edit button stays inactive.

After your choices are set and you press Export to set things in motion, the audio render runs first. The video render follows once the audio finishes. Be aware that, according to which encoder is in play, video rendering might run across several passes. A progress bar from Live keeps you posted on where the process stands.

So long as no custom window size or aspect ratio was set in the encoder settings, the finished video file plays back just the way it looked during real time playback in Live. That video file holds the rendered audio as well.

The [Working with Video](https://www.ableton.com/en/live-manual/12/working-with-video/#working-with-video) chapter goes deeper into handling video inside Live.

<a id="source-5135-real-time-rendering"></a>
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
