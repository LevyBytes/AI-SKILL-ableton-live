# Audio MIDI Group Return And Main Tracks

Open when you need guidance on Audio MIDI Group Return And Main Tracks in Ableton Live.

Context: [Mixing](mixing.md#18-mixing).

<a id="source-182-audio-and-midi-tracks"></a>
### 18.2 Audio and MIDI Tracks

In Live, audio and MIDI tracks exist to hold and play back clips, a topic covered in the [Live Concepts](https://www.ableton.com/en/live-manual/12/live-concepts/#live-concepts) chapter.

Fresh audio and MIDI tracks can be brought into your Live Set through the relevant Create menu commands, or via the shortcuts Ctrl+T (Win) / Cmd+T (Mac) for an audio track and Ctrl+Shift+T (Win) / Cmd+Shift+T (Mac) for a MIDI track.

You can also make tracks by double-clicking or hitting Enter on browser files to load them, or by dragging items out of the browser into the area to the right of Session View tracks or beneath Arrangement View tracks. Devices or files brought into Live this way generate tracks matching their type (for instance, dragging in a MIDI file or effect produces a MIDI track).

Pulling one clip, or several, from an existing track into the area to the right of Session View tracks or beneath Arrangement View tracks builds a new track holding those clips along with the original track's devices.

Each track is shown by its _track title bar_.

Tracks are Represented by Track Title Bars.

Clicking a track title bar selects the track, after which an Edit menu command can be run on it to make changes. Rename is one such command that is available. A whole series of tracks can be renamed quickly by running this command, or the Rename shortcut Ctrl+R (Win) / Cmd+R (Mac), then pressing Tab to jump from one title bar to the next.

If a name begins with a # symbol, the track receives a number that refreshes on its own as the track gets moved. Each extra # symbol pads the track number with another leading zero. You may also supply your own [info text](https://www.ableton.com/en/live-manual/12/first-steps/#info-view) for a track through the Edit Info Text command found in the Edit menu or in that track's context menu.

To reorder tracks, drag them by their title bars; to alter their width (in Session View) or height (in Arrangement View), click and drag along their edges.

Several adjacent or nonadjacent tracks may be picked at the same time by Shift-clicking or Ctrl-clicking, respectively. Dragging a group of nonadjacent tracks causes them to merge together upon being dropped. To shift nonadjacent tracks while keeping them apart, rely on Ctrl + arrow keys rather than the mouse.

While more than one track is selected, modifying one of their mixer controls modifies that same control across the others. Should the tracks in the multi-selection hold different values for some knob or slider parameter (volume, say), that gap stays intact as you move the parameter.

Dragging a track's title bar onto a folder within the Places section of the browser stores it as a new Set. When a track holds audio clips, Live handles copying the referenced samples into this fresh location according to the choice made in the [Collect Files on Export](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#collect-files-on-export) chooser. You may then enter a name for the new Set or accept the one Live proposes by pressing Enter.

To remove tracks, use the Delete command in the Edit menu.

<a id="source-183-group-tracks"></a>
### 18.3 Group Tracks

Any quantity of separate audio or MIDI tracks can be merged into a special summing container known as a Group Track. Building a Group Track is a matter of selecting the tracks you want included and running the Group Tracks command in the Edit menu. The same command also nests one or more existing Group Tracks inside a new Group Track.

Although a Group Track can't hold clips of its own, it resembles an audio track in having mixer controls and the ability to host audio effects.

A fast route to building [submixes](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#creating-submixes) is also provided by Group Tracks. As tracks enter a group, their Audio To [routing choosers](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#internal-routings) get pointed at their Group Track automatically, unless a custom routing was already in place, i.e. aimed at somewhere other than Main. A Group Track can equally serve simply as a “folder“ track by sending the outputs of its member tracks elsewhere.

A group's tracks can be revealed or concealed through the Unfold Group button on the title bar. This is useful for tidying up large Sets by tucking away tracks you have no need to view.

An Unfolded Group Track in Session View.

After a Group Track exists, tracks may be dragged into it or out of it. Removing a Group Track wipes out everything inside it, yet a group can be turned back into separate tracks by running the Ungroup Tracks command in the Edit Menu.

Within Arrangement View, Group Tracks present a summary of the clips held in their member tracks.

A Folded Group Track in Arrangement View

Inside Session View, slots within Group Tracks carry launch and stop buttons as soon as a single clip exists somewhere in a scene. Pressing this button to launch or stop has the same result as launching or stopping every clip it contains. In the same way, picking a Group Slot acts as a shortcut for picking all of the clips inside.

To push a Group Track's color onto every track and clip it contains, run the Assign Track Color to Grouped Tracks and Clips command from the context menu of that Group Track's header.

Keep in mind that, within Session View, invoking the Assign Track Color to Grouped Tracks and Clips command recolors only the Session clips. In the same way, running either command in Arrangement View recolors only the Arrangement clips.

When a Group Track holds a soloed track or a nested Group Track, its Solo button shows up half colored.

Solo Button of a Group Track Containing a Soloed Nested Group Track.

<a id="source-184-return-tracks-and-the-main-track"></a>
### 18.4 Return Tracks and the Main track

Beyond Group Tracks and the tracks that play clips, every Live Set has a _Main track_ together with _return tracks_; while these can't play clips, they enable more versatile signal processing and routing.

Both the return tracks and the Main track sit along the right edge of the Session mixer view and at the lower portion of the Arrangement View.

Keep in mind that the return tracks can be shown or hidden through the _Return Tracks_ entry found in the Mixer Controls submenu of the View menu.

Just like ordinary clip tracks, return tracks are able to host effects devices. The difference is that an effect on a clip track works only on that track's own audio, while return tracks can work on audio routed to them from many tracks at once.

Imagine, for instance, that you wish to produce rhythmic echoes via a delay effect. Drop the effect onto a clip track and only the clips played in that track get echoed. Put that same effect on a return track and it can take in audio from any number of tracks and apply echoes to them.

The Send Controls and Pre/Post Toggles.

A clip or group track's Send control sets how much of that track's output is fed into the input of the linked return track. Beyond that, even a return track's own output can be sent back to its input, which lets you build feedback. Since runaway feedback can spike the level loudly and without warning, the Send controls on Return tracks come disabled by default. Turn them on by right-clicking a Return track's Send knob and choosing Enable Send or Enable All Sends.

A Pre/Post toggle exists on every return track, deciding whether the signal a clip track feeds it is taken before or after the mixer stage (that is, the pan, volume and track-active controls). With the “Pre“ setting, you can build an auxiliary mix that gets processed in the return track, separate from the main mix. Because the return track can be sent to its own output, this works for setting up a dedicated monitor mix for one player in a band.

Signals from all other tracks default to the Main track as their destination. Drag effects onto it to treat the combined signal before it reaches the Main output. Effects placed on the Main track typically handle _mastering_-style tasks like compression and/or EQ.

Several return tracks can be made through the Insert Return Track command in the Create menu, but there is, by definition, just a single Main track.
