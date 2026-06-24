# Audio Clips Tempo And Warping (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 9. Audio Clips, Tempo, and Warping

Within Live, recorded sound offers plenty of room for creative reshaping and stretching. The act of reshaping a clip's timing and groove goes by the name _warping_. Through warping, you handle audio as if it had elastic properties, which makes fluid time-stretching and locking to a tempo possible.

You can apply any of several [Warp Modes](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes) to a clip, which shifts its timing while leaving pitch untouched, or the reverse. The same feature can imitate how analog tape behaves by shifting pitch and timing together. On top of that, warping makes it simple to blend clips recorded at different BPMs.

### 9.1 Tempo

### 9.1.1 Setting the Tempo

The Tempo Field in the Control Bar.

Through the tempo field on the Control Bar, you control how fast your Live Set plays back. It is even possible to [automate the tempo](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#editing-the-tempo-automation) so that gradual or abrupt tempo shifts unfold across the song timeline.

Two readouts appear in the tempo field: the coarse value measured in BPM and the fine value given in hundredths of a BPM. Each can be [key or MIDI mapped](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) on its own, which comes in handy when you need exact tempo adjustments while playing live.

Beyond that, the tempo can be synced between Live and outside gear in a number of ways: external hardware can track Live’s tempo, or the opposite, by way of MIDI Clock or Link, and Live’s tempo can also lock onto an incoming audio source through Tempo Follower. The [Synchronizing with Link, Tempo Follower, and MIDI](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-with-link-tempo-follower-and-midi) chapter covers this in greater depth.

### 9.1.2 Tapping the Tempo

The Tap Button.

Besides entering a tempo as a numeric value, the Tap Tempo button gives you another route: dial in the tempo through mouse clicks or taps on a computer key.

Clicking the Tap Tempo button once on each beat makes the Live Set's tempo trail the rhythm of your clicks.

If you would rather drive the tempo from a computer key than from clicks, assign a key to the Tap Tempo button by way of [Key Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control):

1. In the Control Bar, click the Key switch so that Key Map Mode turns on.
2. Select the Tap Tempo button.
3. On your keyboard, hit whichever key you intend to tap with.
4. Click the Key switch a second time to exit Key Map Mode.

From then on, that mapped key serves to tap out the tempo.

The Switch for Key Map Mode.

As another option, the Tap Tempo button can be bound to a MIDI note or controller — a footswitch pedal, say — through [MIDI Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#the-mapping-browser).

Tap tempo changes take effect in Live right away, yet each additional tap sharpens how precisely the tempo gets detected.

With the _Start Playback with Tap Tempo_ option turned on in the Record, Warp & Launch Settings, tapping can double as a way to [trigger playback](https://www.ableton.com/en/live-manual/12/arrangement-view/#transport-and-playback). Under a 4/4 time signature, four taps are needed before the song begins playing at the tapped tempo.

Should you start the transport by tapping, the play position of any apps linked through [Link](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#setting-up-link) syncs on its own. That keeps those apps locked to the tempo and properly placed inside the current musical phrase.

### 9.1.3 Nudging the Tempo

The Phase Nudge Up/Down Buttons.

Even though Live can be [easily synchronized](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-with-link-tempo-follower-and-midi) through Link or to outboard MIDI gear, there are times when you must line a Set up with outside sources that don't hold a steady tempo, like live players or turntables. Provided your Set's tempo is in the ballpark of the outside source, the Phase Nudge Up/Down buttons let you momentarily push Live's playback faster or slower to track those tempo shifts. Just like the Tap Tempo button, the Phase Nudge buttons accept [key or MIDI mapped](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) assignments for tactile control.

### 9.1.4 Clip Tempo Followers and Leaders

Out of the box, warped clips trail the Set's tempo; even so, any clip in the Arrangement View can be promoted to a tempo leader through the Lead/Follow toggle found in the Clip View's [Audio Utilities panel](https://www.ableton.com/en/live-manual/12/clip-view/#audio-utilities-panel).

By Default, Warped Clips Trail the Set's Tempo.

Once a clip is switched to Lead, the Set runs at whatever tempo the clip's [Warp Markers](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-markers) dictate. That allows the Set to lock onto the tempo of leader clips, so those clips sound as though no warping were applied. On top of that, the Control Bar's tempo field goes inactive.

Flip the Lead/Follow Toggle to Lead so the Clip Plays at Its Original Tempo.

You may flag as many clips as you like to be tempo leaders, though only a single clip governs the tempo at any given moment. If leaders sit on several different tracks, priority goes to the tempo of the playing clip located on the lowest track.

Live builds tempo automation on its own to follow the differences between each clip's tempo and the Set's tempo. You can see this automation in the Main track, but it stays read-only. Should leader clips be shuffled around in the Arrangement, the matching automation travels with them. If you want to preserve and modify those automation changes, reach for the _Unfollow Tempo Automation_ option located in the tempo field's context menu. Doing so demotes every leader clip to a follower and makes the Main track's automation editable.

Choose Unfollow Tempo Automation to Make It Editable.

Automation produced by clip tempo leaders takes priority over the tempo of any audio input syncing through [Tempo Follower](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-via-tempo-follower).

Keep in mind that while Live's [EXT switch](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-external-midi-devices-to-live) is active, the Lead/Follow toggle becomes unavailable.

### 9.2 Warping

A key strength of Live is that it can lock any sample to a tempo you pick. Warping opens the door to fluid beat matching, rhythmic play, and sound design, plus keeping tracks aligned during both playback and live shows.

Each audio clip's warping settings live in the Clip View's [Audio Utilities panel](https://www.ableton.com/en/live-manual/12/clip-view/#audio-utilities-panel). Double-clicking an audio clip in either the Session or Arrangement View brings up the Clip View.

The Warping Controls on the Audio Tab.

Warping for an audio clip is switched on and off by the _Warp_ switch.

With the Warp switch off, a sample runs at its own native tempo and ignores whatever the Set's tempo happens to be. That suits non-rhythmic material — think percussion one shots, textures, sound effects, or spoken word.

Flip the Warp switch on when you want rhythmically organized material, like loops or full songs, to lock to the Set's tempo.

### 9.2.1 Warping Options in Settings

Beyond flipping the Warp switch on a clip-by-clip basis, the Record, Warp & Launch Settings let you set how samples behave at load time. The moment a sample comes in, Live judges it to be short or long and then applies one of the options listed here.

Through the _Loop/Warp Short Samples_ option, you pick the default warp state given to short samples:

- Unwarped One Shot - Samples stay unwarped at load.
- Warped One Shot - Samples get warped using the default Warp Mode, but no looping is applied.
- Warped Loop - Samples are both warped and looped.
- Auto - Live picks whichever of the choices above fits the particular sample best. This is the default selection.

With the _Auto-Warp Long Samples_ option, you decide whether long samples warp automatically as they load. It comes switched on by default. After a sample is auto-warped, a [Warp Marker](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-markers) lands on the first beat of every bar. Turn the option off and long samples stay unwarped when dropped onto tracks.

The _Default Warp Mode_ option determines which [Warp Mode](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes) gets applied automatically as samples are warped. A Warp Mode sets the algorithm that time-stretches the audio, shaping how the clip ends up sounding. Out of the gate, Beats mode serves as the default Warp Mode.

### 9.2.2 Importing Samples

Samples can reach a Set either by dragging them in from folders on your machine, or — with an audio track selected — through the _Import Audio File…_ command under the Create menu, which brings in MP3, AAC, Ogg Vorbis, Ogg FLAC, or FLAC files. That command drops files at the insert marker in the Arrangement View, or into whichever clip slot is selected in the Session View.

The first time a file enters Live, it undergoes analysis and stays unplayable and uneditable until that analysis wraps up. After it finishes, the sample shows up in the Sample Editor and, most of the time, sits in sync with the Set's tempo.

### 9.2.3 Warp Markers

A Warp Marker pins a chosen spot in a sample — a transient, for instance — to a definite location on the timeline. Markers serve either to chart the audio's timing faithfully or to reshape its rhythm. A handful of starter Warp Markers appear automatically the first time a sample is imported, yet you remain free to add as many of your own as the job calls for.

To drop a Warp Marker, double-click anywhere across the top half of the Sample Editor and one appears at that spot. The shortcut CtrlI (Win) / CmdI (Mac) does the same at the insert marker. Once placed, markers respond to the arrow keys or can be dragged to whatever points in time you need.

Warp Markers Shown in the Sample Editor.

With a Warp Marker selected, holding Shift lets you drag the waveform around, giving you fine control over exactly where the audio beneath the marker begins.

Removing Warp Markers is a matter of double-clicking them, or selecting the matching time in the Sample Editor and pressing the Backspace (Win) or Delete (Mac) key.

When you want the Sample Editor to [scroll](https://www.ableton.com/en/live-manual/12/clip-view/#zooming-and-scrolling-in-the-clip-views-editor) along with playback as you edit clips, switch on the Follow switch in the Control Bar. Bear in mind that Follow halts the moment you make an edit inside the Sample Editor. Starting playback, or clicking in the Arrangement or clip scrub area, gets Follow going again.

The Follow Switch on the Control Bar.

#### 9.2.3.1 Transients and Pseudo-Warp Markers

The first time a sample lands on a track, Live runs an automatic analysis of the audio and locates its _transients_. Transients are amplitude peaks marking the onset of notes or beats, and they tend to make excellent spots for Warp Markers.

In the Sample Editor, transients show up as small gray markers along the top edge.

Transient Markers Shown in the Sample Editor.

Creating or deleting transients by hand is done through the matching commands in the Create menu, or with the shortcuts CtrlShiftI (Win) / CmdShiftI (Mac) and CtrlShiftBackspace (Win) / CmdShiftDelete (Mac). Clearing every hand-made transient is handled by the _Reset Transients_ option in the Sample Editor's context menu.

To lay down Warp Markers across all transients within a time selection, reach for the Insert Warp Markers command in the Create menu or the shortcut CtrlI (Win) / CmdI (Mac). Where the chosen region holds no transients, Warp Markers land at the selection's start and end instead.

Hovering over transient markers reveals _Pseudo-Warp Markers_. These resemble ordinary Warp Markers except that they appear gray rather than yellow. A double-click or a drag converts a pseudo-marker into a genuine Warp Marker. When no Warp Markers exist beyond the one just made, the clip's tempo shifts as well. Holding the Ctrl (Win) / Cmd (Mac) modifier as you turn a pseudo-marker into a Warp Marker also drops Warp Markers on the neighboring transients. Holding Shift and dragging a pseudo-marker relocates the transient to a fresh spot within the Sample Editor.

#### 9.2.3.2 Saving Warp Markers with a Sample File

Although Warp Markers get stored with the Live Set on their own, you can additionally write them into the sample file itself, so they turn up in the Sample Editor every time that file is dragged onto a track. Accomplish this by clicking the [Save button](https://www.ableton.com/en/live-manual/12/clip-view/#saving-default-audio-clip-settings-with-the-sample) on the clip's title bar. Bear in mind that saving default clip settings works only for samples you own, not for anything drawn from Live's Core Library or Pack content.

After a sample carries saved Warp Markers, Auto-Warp does nothing to it. Even so, you can still kick off auto-warping by hand through any of the [Warp From…](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#auto-warping-long-samples) context menu options.

### 9.2.4 Warping Short Samples

The sections that follow walk through using warping to lock various kinds of short samples to a Set's tempo. Every scenario presumes you have switched on, within the Record, Warp & Launch Settings, the _Loop/Warp Short Samples_ option, so that freshly added samples get [automatically warped](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping-options-in-settings) on entry to a Set — the default arrangement.

#### 9.2.4.1 Even-Length Loops

On import, Live presumes a sample holds a cleanly trimmed musical loop running 1, 2, 4, 8, or 16 bars, and it sets the tempo to suit. Two Warp Markers are also generated: one anchored to the sample's beginning and one to its end.

A Four-Bar Loop Shown in the Sample Editor.

You will find the sample's guessed tempo displayed in the BPM field of the Audio Utilities panel. When the exact BPM is known to you, type it straight into the field. When you're uncertain of the precise tempo, hold Shift while dragging the slider to nudge the BPM in small steps. Holding Shift and dragging from the clip's edge in Arrangement View likewise stretches or squeezes the clip's tempo.

The BPM Field Within the Audio Utilities Panel.

Now and then the original tempo gets estimated wrong, and the BPM field reports a value that runs either double-speed or half-speed. Setting it right is a matter of the ×2 and ÷2 buttons, which double or halve the tempo in turn.

#### 9.2.4.2 Odd-Length Loops

A sample whose bar count is odd ends up out of sync, because Live starts off presuming an even bar count thanks to the standard 4/4 time signature setting.

To get playback in sync, the Warp Marker at the sample's end has to sit on the downbeat of an even bar — bar eight in a nine-bar loop, say. Correcting it is just a matter of dropping a marker onto the right bar.

Live can also misjudge some odd-bar loops as being longer or shorter than they really are; a nine-bar loop, for example, might be read as an eight-bar loop. Should that happen, the final bar may stay hidden at first. The remedy is to drag the Warp Marker at the sample's end rightward until the eighth bar comes into view.

#### 9.2.4.3 Uneven-Length Loops

Samples that were never trimmed for gapless looping, or that lack a clear beat pattern, will likewise drift out of sync.

The fix is to drag the insert marker onto the first downbeat of the sample, then choose the _Set 1.1.1 Here_ context menu option to drop a Warp Marker right there.

Use the Set 1.1.1 Here Command to Drop the First Warp Marker.

With that first Warp Marker in place, you can move on to the _Warp From Here_ context menu option. To clear away leftover silence at the loop's tail, set a Warp Marker just ahead of the sample's silent stretch.

#### 9.2.4.4 Multi-Clip Warping

Select several clips of identical length and then add or tweak Warp Markers on any one of them, and those edits roll out to every selected clip at once. This proves especially handy when a group of clips shares the same rhythm and you want their timing reworked together — for instance, when you've recorded a multitrack performance and need to fix timing problems across all the tracks.

### 9.2.5 Auto-Warping Long Samples

The section below shows how auto-warping serves to lock longer samples, or whole songs, to a Set's tempo. Each scenario presumes you have switched on, inside the Record, Warp & Launch Settings, the _Auto-Warp Long Samples_ option, so that newly added samples come in [automatically warped](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping-options-in-settings) when joined to a Set — the default behavior.

Auto-Warp Results Shown in the Sample Editor.

#### 9.2.5.1 Adjusting Auto-Warp Results

More often than not, the [Auto-Warp algorithm](https://help.ableton.com/hc/en-us/articles/9230108251164) nails the audio clip's tempo, so it falls neatly in step with the Set's tempo. Still, when the auto-warped outcome isn't what you had in mind, you can refine it by hand.

While reworking Warp Markers on longer samples, it helps to switch on the metronome in the Control Bar so you have a constant tempo reference.

The Metronome Switch.

There are times when Auto-Warp lands the tempo but misses the downbeat. Any of these approaches will set it straight:

- Hold Shift and drag from a Warp Marker to shift where the waveform sits beneath that marker.
- Drag the insert marker onto the downbeat, then invoke the context menu's _Set 1.1.1 Here_ command to relocate the start marker there.
- Zoom in, drop a Warp Marker on the downbeat, and then pull that marker to the start of the timeline's first bar.
  Dragging a Warp Marker to Set the Start Position.

For a sample already trimmed for gapless looping, refining the Auto-Warp outcome is easy via the _Warp Sample as…_ command found in the Sample Editor's context menu. That command offers up a suggested loop length suited to the Set's tempo.

The Warp Sample As… Context Menu Option.

Auto-Warp can be aimed at just one part of a sample as well — pulling and warping a breakbeat out of a longer track, for instance. Do this by dragging across the slice of the sample you want to single out to make a time selection in the Sample Editor. Then call the _Warp Selection as…_ command from the context menu. Auto-Warp settles on what it figures is the best-fitting loop length, drops matching start and end loop markers, and warps the selection so it fills that loop.

Warping a Chosen Portion of a Sample.

Some samples call for tighter command over the Auto-Warp outcome. The surest route there is to warp the audio piece by piece, moving from left to right. Pinning Warp Markers at the start and end of each well-warped stretch holds it in place. [Various shortcuts](https://www.ableton.com/en/live-manual/12/live-keyboard-shortcuts/#clip-view-sample-editor) for the Sample Editor can speed this along — for example, holding the Ctrl (Win) / Cmd (Mac) modifier lets you grab several Warp Markers and shift them as a group.

The Sample Editor's context menu carries a set of _Warp From Here…_ commands, each offering a different way to reset Warp Markers lying to the right of a grid division or Warp Marker while leaving everything to the left alone. You can fire these off anywhere along the timeline, the start marker included.

- _Warp From Here_ applies the Auto-Warp algorithm to the audio sitting right of the selected marker. With no marker selected, one gets dropped at the chosen point on the grid.
- _Warp From Here (Start At …)_ takes the Set's tempo as the reference for auto-warping. To first bring the Set's tempo in line with the clip's BPM, turn warping off for the clip so it plays at its native speed. Next, tap the [Tap Tempo](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#tapping-the-tempo) button in the Control Bar to match the clip's tempo to the Set. Once that's set, switch warping back on for the clip and run the Warp From Here (Start At …) command so your tapped tempo becomes the reference.
- _Warp From Here (Straight)_ is the right pick for samples with no tempo drift. One lone Warp Marker gets placed at the starting point, derived from the sample's estimated original BPM.
- _Warp … BPM From Here_ likewise drops a single Warp Marker at the starting point, but here the clip is treated as sharing the Set's tempo. It's handy when you already know the sample's exact BPM and can enter it into the Control Bar's tempo field ahead of warping.

### 9.2.6 Manipulating Grooves

Beyond locking a sample's musical timing precisely, Warp Markers can just as well be turned to bending the rhythm on purpose for creative ends.

Say you spot a transient arriving late in a percussive sample: pin a Warp Marker onto it and then drag that marker until it lines up with the proper beat. Pinning the transients on either side too can be wise, sparing the neighboring parts of the sample from being disturbed.

Using Warp Markers to Shape the Groove.

Reworking a sample's natural rhythm with Warp Markers makes for a compelling creative move, all the more so when paired with [grooves](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves).

### 9.2.7 Quantizing Audio

On top of time-stretching a sample with Warp Markers, you can have a waveform snap to the grid on its own through [quantization](https://www.ableton.com/en/live-manual/12/editing-midi/#quantizing-notes). Quantization lines the audio up by nudging the closest transient to its nearest grid line.

To quantize audio, click somewhere in the Sample Editor to give it focus; then either pick Quantize under the Edit menu or press the keyboard shortcut CtrlU (Win) / CmdU (Mac). Those options align the audio according to the present quantization settings, which you can tune in the Quantize panel.

The Quantize Panel.

You can quantize audio to the current grid size or to a particular grid division, triplets among them. For a gentler effect, dial back the level of applied quantization with the Amount control, which moves the Warp Markers by a fraction of the chosen quantization value.

### 9.3 Warp Modes

The Warp Modes in Live draw on assorted granular synthesis methods to stretch time by repeating or dropping pieces of the audio; those pieces are known as grains. Every Warp Mode follows its own scheme for picking, overlapping, and crossfading grains, which shapes the way the audio gets stretched or squeezed. As a result, particular Warp Modes fit particular sorts of audio material, hinging on the source's original tonal makeup.

Warping lends itself to exact time-stretching, but it also opens up plenty of creative avenues for bending a sample's rhythm toward more experimental outcomes.

### 9.3.1 Beats Mode

Beats mode shines on audio carrying a strong rhythm, such as drum loops and the bulk of electronic dance music. Here the granulation is tuned to hold onto the audio's transients.
