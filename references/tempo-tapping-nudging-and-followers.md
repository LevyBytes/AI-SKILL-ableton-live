# Tempo Tapping Nudging And Followers

Open when you need guidance on Tempo Tapping Nudging And Followers in Ableton Live.

Context: [Tempo](audio-clips-tempo-and-warping.md#91-tempo).

<a id="source-911-setting-the-tempo"></a>
### 9.1.1 Setting the Tempo

The Tempo Field in the Control Bar.

Through the tempo field on the Control Bar, you control how fast your Live Set plays back. It is even possible to [automate the tempo](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#editing-the-tempo-automation) so that gradual or abrupt tempo shifts unfold across the song timeline.

Two readouts appear in the tempo field: the coarse value measured in BPM and the fine value given in hundredths of a BPM. Each can be [key or MIDI mapped](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) on its own, which comes in handy when you need exact tempo adjustments while playing live.

Beyond that, the tempo can be synced between Live and outside gear in a number of ways: external hardware can track Live’s tempo, or the opposite, by way of MIDI Clock or Link, and Live’s tempo can also lock onto an incoming audio source through Tempo Follower. The [Synchronizing with Link, Tempo Follower, and MIDI](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-with-link-tempo-follower-and-midi) chapter covers this in greater depth.

<a id="source-912-tapping-the-tempo"></a>
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

<a id="source-913-nudging-the-tempo"></a>
### 9.1.3 Nudging the Tempo

The Phase Nudge Up/Down Buttons.

Even though Live can be [easily synchronized](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-with-link-tempo-follower-and-midi) through Link or to outboard MIDI gear, there are times when you must line a Set up with outside sources that don't hold a steady tempo, like live players or turntables. Provided your Set's tempo is in the ballpark of the outside source, the Phase Nudge Up/Down buttons let you momentarily push Live's playback faster or slower to track those tempo shifts. Just like the Tap Tempo button, the Phase Nudge buttons accept [key or MIDI mapped](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) assignments for tactile control.

<a id="source-914-clip-tempo-followers-and-leaders"></a>
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
