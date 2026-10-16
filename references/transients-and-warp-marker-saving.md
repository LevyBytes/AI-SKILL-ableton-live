# Transients And Warp Marker Saving

Open when you need guidance on Transients And Warp Marker Saving in Ableton Live.

Context: [Warp Markers](audio-clips-tempo-and-warping.md#923-warp-markers).

<a id="source-9231-transients-and-pseudo-warp-markers"></a>
#### 9.2.3.1 Transients and Pseudo-Warp Markers

The first time a sample lands on a track, Live runs an automatic analysis of the audio and locates its _transients_. Transients are amplitude peaks marking the onset of notes or beats, and they tend to make excellent spots for Warp Markers.

In the Sample Editor, transients show up as small gray markers along the top edge.

Transient Markers Shown in the Sample Editor.

Creating or deleting transients by hand is done through the matching commands in the Create menu, or with the shortcuts Ctrl+Shift+I (Win) / Cmd+Shift+I (Mac) and Ctrl+Shift+Backspace (Win) / Cmd+Shift+Delete (Mac). Clearing every hand-made transient is handled by the _Reset Transients_ option in the Sample Editor's context menu.

To lay down Warp Markers across all transients within a time selection, reach for the Insert Warp Markers command in the Create menu or the shortcut Ctrl+I (Win) / Cmd+I (Mac). Where the chosen region holds no transients, Warp Markers land at the selection's start and end instead.

Hovering over transient markers reveals _Pseudo-Warp Markers_. These resemble ordinary Warp Markers except that they appear gray rather than yellow. A double-click or a drag converts a pseudo-marker into a genuine Warp Marker. When no Warp Markers exist beyond the one just made, the clip's tempo shifts as well. Holding the Ctrl (Win) / Cmd (Mac) modifier as you turn a pseudo-marker into a Warp Marker also drops Warp Markers on the neighboring transients. Holding Shift and dragging a pseudo-marker relocates the transient to a fresh spot within the Sample Editor.

<a id="source-9232-saving-warp-markers-with-a-sample-file"></a>
#### 9.2.3.2 Saving Warp Markers with a Sample File

Although Warp Markers get stored with the Live Set on their own, you can additionally write them into the sample file itself, so they turn up in the Sample Editor every time that file is dragged onto a track. Accomplish this by clicking the [Save button](https://www.ableton.com/en/live-manual/12/clip-view/#saving-default-audio-clip-settings-with-the-sample) on the clip's title bar. Bear in mind that saving default clip settings works only for samples you own, not for anything drawn from Live's Core Library or Pack content.

After a sample carries saved Warp Markers, Auto-Warp does nothing to it. Even so, you can still kick off auto-warping by hand through any of the [Warp From…](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#auto-warping-long-samples) context menu options.
