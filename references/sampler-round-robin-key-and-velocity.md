# Sampler Round Robin Key And Velocity

Open when you need guidance on Sampler Round Robin Key And Velocity in Ableton Live.

Context: [The Zone Tab](sampler-zones-and-playback-routes.md#30105-the-zone-tab).

<a id="source-301051-round-robin-sample-playback"></a>
#### 30.10.5.1 Round Robin Sample Playback

Using Different Samples for Round Robin Playback.

With Round Robin, a fresh sample sounds on each successive note you play. The result is that, over time, you step through a group of samples following a set sequence.

One use, for instance, is to step Round Robin through samples of the same note or sound captured with varied articulations, lending gentle variety to otherwise repetitive drum or note figures. Alternatively, feeding it samples that sound wildly different produces surprising rhythmic or tonal twists across a pattern.

Turning Round Robin on is done by flipping the RR toggle within the Zone Editor.

Enable the RR Toggle to Activate Round Robin Playback.

After it's active, whichever samples in the [sample layer list](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#the-sample-layer-list) occupy the same [key zone](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#key-zones) become eligible to fire whenever a note lands in that range.

The Round Robin Mode chooser lets you pick how those samples get triggered:

_Forward_: Steps through samples in sequence, beginning at the top of the sample layer list and moving downward. After the final sample sounds, the sequence loops back around to the uppermost sample.

_Backward_: Steps through samples in sequence, beginning at the bottom of the sample layer list and working upward. After the topmost sample plays, the sequence starts over.

_Other_: Draws samples in random order, but guarantees the same sample is never fired two times back-to-back.

_Random_: Draws samples in random order, and here the same sample may indeed repeat several times in succession.

The Round Robin Mode Chooser.

Through the Reset Interval chooser you can dictate a fixed point at which the sequence starts over. That helps fire samples in a steady, predictable way. As an example, with the Round Robin Mode set to Forward and a reset interval of 1 bar, the uppermost sample sounds on each bar's opening note. With Backward, the sequence resets to the bottommost sample. With Other or Random, it resets to whichever sample played first.

The Reset Interval Chooser.

<a id="source-301052-the-sample-layer-list"></a>
#### 30.10.5.2 The Sample Layer List

The Sample Layer List.

Every sample held within the multisample you currently have loaded shows up here, each occupying its own layer. With extremely large multisamples, the list could stretch to hundreds of layers! Happily, you can give layers meaningful names (based on their root key, say). Hover over a layer here, or over a zone in the zone editors, and the Status Bar (bottom of screen) presents details about that sample. Pick any layer and its sample loads into the Sample tab so you can inspect it.

A right-click anywhere in the sample layer list brings up a context menu with choices for ordering and presenting the layers, spreading them across the keyboard, and assorted other sample-management and “housekeeping“ tasks.

_Delete_: Removes whichever sample(s) you currently have selected.

_Duplicate_: Makes a copy of whichever sample(s) you currently have selected.

_Rename_: Gives the chosen sample a new name.

_Distribute Ranges Equally_: Spreads samples uniformly across the editor’s full MIDI note range (C-2 to G8).

_Distribute Ranges Around Root Key_: When layers carry differing root keys, this choice spaces their ranges as evenly as it can around each root key while avoiding any overlap. When layers share one root key, their ranges come out evenly spaced.

_Small/Medium/Large_: Changes how far the Zone Editor is zoomed.

_Show in Browser_: Jumps to the chosen sample within the browser and highlights it.

_Manage Sample_: Brings up the File Manager with the chosen sample selected.

_Normalize Volume_: Tunes Sampler’s Volume control so that the loudest peak in each selected sample fills the full available headroom.

_Normalize Pan_: Tunes Sampler’s Pan control so each selected sample carries matching volume on both sides of the stereo field. Keep in mind this won't always recenter panned stereo samples; instead, Live works out a pan setting that yields a balanced stereo spread.

_Select All With Same Range_: Highlights every layer sharing the zone range of the layer you've currently selected. What you get back varies with whichever Zone Editor (Key, Velocity or Sample Select) happens to be active.

_Sort Alphabetically (Ascending and Descending)_: Orders samples by name in alphabetical sequence.

_Sort by Key (Ascending and Descending)_: Orders key zones either ascending or descending.

_Sort by Velocity (Ascending and Descending)_: Orders velocity zones either ascending or descending.

_Sort by Selector (Ascending and Descending)_: Orders sample select zones either ascending or descending.

<a id="source-301053-key-zones"></a>
#### 30.10.5.3 Key Zones

The Key Zone Editor.

A sample's key zone sets the span of MIDI notes across which that sample sounds. A sample fires only when an arriving MIDI note falls inside its key zone. Each sample owns a key zone of its own, and that zone may cover anything from one solitary key right up to all 127.

The usual multisampled instrument is built from numerous separate samples spread among numerous key zones. A sample is recorded at one specific key within an instrument’s voice range (that key being its _root key_), yet it can still ring true when shifted a handful of semitones either way. That playable span typically becomes the sample’s key zone, while pitches outside it are covered by further samples wherever required.

Newly imported samples start out with key zones spanning the entire MIDI note range. Much like clips in the Arrangement View, you can reposition and resize zones — drag a left or right edge to resize, then slide the zone where you want it.

Either end of a zone can also be faded across several semitones by dragging its upper-left or upper-right corner. That lets neighboring samples crossfade cleanly into one another as you move along the keyboard. Above the sample layer list, the Lin and Pow boxes show whether a zone fades in linear or exponential fashion.

<a id="source-301054-velocity-zones"></a>
#### 30.10.5.4 Velocity Zones

The Velocity Zone Editor.

A velocity zone fixes which span of MIDI Note On velocities (1-127) a given sample reacts to. Since how hard you play dramatically alters the tone of most instruments, the finest multisamples record not just the individual notes but also each note captured at several velocities.

Switch on the Velocity Zone Editor and it shows up beside the sample layer list. Velocity runs along a scale of 1-127, and that range of numbers is printed across the editor's top edge. Apart from that, the Velocity Zone Editor behaves exactly like the Key Zone Editor.
