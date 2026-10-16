# Warp Settings Imports And Markers

Open when you need guidance on Warp Settings Imports And Markers in Ableton Live.

Context: [Warping](audio-clips-tempo-and-warping.md#92-warping).

<a id="source-921-warping-options-in-settings"></a>
### 9.2.1 Warping Options in Settings

Beyond flipping the Warp switch on a clip-by-clip basis, the Record, Warp & Launch Settings let you set how samples behave at load time. The moment a sample comes in, Live judges it to be short or long and then applies one of the options listed here.

Through the _Loop/Warp Short Samples_ option, you pick the default warp state given to short samples:

- Unwarped One Shot - Samples stay unwarped at load.
- Warped One Shot - Samples get warped using the default Warp Mode, but no looping is applied.
- Warped Loop - Samples are both warped and looped.
- Auto - Live picks whichever of the choices above fits the particular sample best. This is the default selection.

With the _Auto-Warp Long Samples_ option, you decide whether long samples warp automatically as they load. It comes switched on by default. After a sample is auto-warped, a [Warp Marker](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-markers) lands on the first beat of every bar. Turn the option off and long samples stay unwarped when dropped onto tracks.

The _Default Warp Mode_ option determines which [Warp Mode](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes) gets applied automatically as samples are warped. A Warp Mode sets the algorithm that time-stretches the audio, shaping how the clip ends up sounding. Out of the gate, Beats mode serves as the default Warp Mode.

<a id="source-922-importing-samples"></a>
### 9.2.2 Importing Samples

Samples can reach a Set either by dragging them in from folders on your machine, or — with an audio track selected — through the _Import Audio File…_ command under the Create menu, which brings in MP3, AAC, Ogg Vorbis, Ogg FLAC, or FLAC files. That command drops files at the insert marker in the Arrangement View, or into whichever clip slot is selected in the Session View.

The first time a file enters Live, it undergoes analysis and stays unplayable and uneditable until that analysis wraps up. After it finishes, the sample shows up in the Sample Editor and, most of the time, sits in sync with the Set's tempo.

<a id="source-923-warp-markers"></a>
### 9.2.3 Warp Markers

A Warp Marker pins a chosen spot in a sample — a transient, for instance — to a definite location on the timeline. Markers serve either to chart the audio's timing faithfully or to reshape its rhythm. A handful of starter Warp Markers appear automatically the first time a sample is imported, yet you remain free to add as many of your own as the job calls for.

To drop a Warp Marker, double-click anywhere across the top half of the Sample Editor and one appears at that spot. The shortcut Ctrl+I (Win) / Cmd+I (Mac) does the same at the insert marker. Once placed, markers respond to the arrow keys or can be dragged to whatever points in time you need.

Warp Markers Shown in the Sample Editor.

With a Warp Marker selected, holding Shift lets you drag the waveform around, giving you fine control over exactly where the audio beneath the marker begins.

Removing Warp Markers is a matter of double-clicking them, or selecting the matching time in the Sample Editor and pressing the Backspace (Win) or Delete (Mac) key.

When you want the Sample Editor to [scroll](https://www.ableton.com/en/live-manual/12/clip-view/#zooming-and-scrolling-in-the-clip-views-editor) along with playback as you edit clips, switch on the Follow switch in the Control Bar. Bear in mind that Follow halts the moment you make an edit inside the Sample Editor. Starting playback, or clicking in the Arrangement or clip scrub area, gets Follow going again.

The Follow Switch on the Control Bar.
