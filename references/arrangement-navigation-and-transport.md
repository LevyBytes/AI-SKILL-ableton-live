# Arrangement Navigation And Transport

Open when you need guidance on Arrangement Navigation And Transport in Ableton Live.

Context: [Arrangement View](arrangement-view.md#6-arrangement-view).

<a id="source-61-layout"></a>
### 6.1 Layout

The Upper Area of the Arrangement View.

1. Spanning the Arrangement’s full set of clips from beginning to end, the _Overview_ serves for navigating and zooming. A black outline marks whichever portion is on screen at the moment. Horizontal dragging scrolls the view sideways, while vertical dragging zooms it closer or farther. Double-clicking inside that black outline anywhere snaps the zoom back out to the whole Arrangement.
2. The _beat-time ruler_ presents time as bars-beats-sixteenths. Dragging here behaves just like it does in the Overview: pull sideways to scroll along the timeline, or pull up and down to zoom. A double-click on the beat-time ruler zooms onto the active selection. With nothing selected, that same double-click zooms back out to the whole Arrangement.
3. A click at any spot in the _scrub area_ begins [playback](https://www.ableton.com/en/live-manual/12/arrangement-view/#transport-and-playback) right there. Holding the left mouse button at a given spot in the scrub area instead loops that region, governed by the current global launch quantization value.
4. _Locators_ may be dropped at any spot in the scrub area so that you can fire playback from [multiple areas](https://www.ableton.com/en/live-manual/12/arrangement-view/#launching-the-arrangement-with-locators) of the Arrangement. They come in handy for breaking a track into sections you can trigger.
5. The _Set Locator_ button drops locators into the scrub area as you play back or record. Once a locator is selected, that same Set Locator button turns into the Delete Locator button for removing locators.
6. Playback for locators is triggered by the _Previous and Next Locator_ buttons. The leap from one fired locator to the next follows the global launch quantization value.
7. Toggle [automation lanes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) on or off with the _Automation Mode_ control.
8. With the _Lock Envelopes_ toggle, you can pin envelopes to the song position rather than to the clips themselves. That way, shifting clips leaves the automation envelopes where they are.
   Track, Mixer, and Additional Zoom Controls in the Arrangement View.
9. A track’s _main lane_ holds and lines up its clips. While following the [comping workflow](https://www.ableton.com/en/live-manual/12/comping/#comping), clips drawn from the various take lanes can be brought into that main lane.
10. The _Arrangement Track Controls_ expose volume, panning, I/O, and further mixer settings. Which of these appear is configurable through the Arrangement Track Controls submenu under the View menu.
11. Within the Arrangement View, [_tracks_](https://www.ableton.com/en/live-manual/12/live-concepts/#tracks) sit in a vertical stack. To reorder them, select and drag a track above or below its neighbors.
12. Dropping instruments and devices into the _Mixer Drop Area_ below the tracks adds fresh tracks to the Arrangement. An instrument or MIDI effect dropped here spawns a MIDI track, whereas an audio effect spawns an audio track.
13. With the _Optimize Height_ and _Optimize Width_ toggles, every track is sized to fit the Arrangement’s present height or width. The matching keyboard shortcuts are H and W.
14. The _Waveform Vertical Zoom Level_ slider grows the waveform shown inside audio clips. That helps you spot transients and waveform detail while leaving the clip gain untouched. This zoom carries across every audio track in the Arrangement and applies to new clips at the moment they record.
15. The _time ruler_ expresses time as minutes-seconds-milliseconds. Drag within it to scroll the view sideways.
16. The [_mixer_](https://www.ableton.com/en/live-manual/12/mixing/#mixing) can be revealed in Arrangement View through the Mixer entry in the View menu, or with the Mixer View toggle down in the lower right corner of Live’s window.

<a id="source-62-navigation-and-zooming"></a>
### 6.2 Navigation and Zooming

Beyond several of the choices laid out in the [Layout section](https://www.ableton.com/en/live-manual/12/arrangement-view/#layout), these further ways of navigating and zooming are on hand as well:

- For gradual zoom in and out centered on the active selection, tap the + and - keys, or roll the mouse wheel or trackpad while holding Ctrl (Win) / Cmd (Mac). Panning the view is done by dragging while you hold the Ctrl+Alt (Win) / Cmd+Option (Mac) modifier.
- For a full zoom onto the active selection, hit Z or pick the Zoom to Arrangement Time Selection command from the View menu. Pressing the X key restores the zoom you had before. Bear in mind that after several successive Z zooms, repeated X presses step back through them one level at a time.
- When you select time over a clip in the Arrangement, the Clip View editor will [zoom in](https://www.ableton.com/en/live-manual/12/clip-view/#zooming-and-scrolling-in-the-clip-views-editor) to match that selected time too.
- For vertical zoom on a chosen track, roll the mouse wheel or trackpad inside that track’s main lane while holding the Alt (Win) / Option (Mac) modifier. Keep in mind that with a time selection present in the Arrangement, every track holding selected content zooms vertically.
- So that the Arrangement view trails the song position and scrolls on its own, flip on the _Follow_ switch in the Control Bar, or invoke the Follow command from the Options menu. Follow halts whenever you edit, scroll the Arrangement sideways, or click the beat-time ruler. It resumes once playback stops or restarts, or when you click within the Arrangement or a clip scrub area.
  The Follow Switch in the Control Bar.

<a id="source-63-transport-and-playback"></a>
### 6.3 Transport and Playback

Playback of the Arrangement is launched by the transport controls sitting in the Control Bar.

A click on the Play button gets playback going; clicking the Stop button halts it. The space bar offers another route, switching playback on and off.

The Play and Stop Buttons in the Control Bar.

You may additionally assign [computer keyboard keys or MIDI messages](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) to those transport controls, giving you a tailored setup for kicking off playback however you like.

Where playback begins is governed by the blinking blue insert marker on a track. Out of the box, that marker sits at the Arrangement’s start. Clicking somewhere inside a track relocates the insert marker, setting a fresh play position. To send the insert marker back to its starting play position, either double-click the Stop button or hit the Home key (Win) or Function + left arrow key (Mac).

Arrangement Playback Begins from the Insert Marker.

If you would rather resume from wherever playback last halted instead of the insert marker, hold Shift as you press the space bar.

You can also reach the play position through the Control Bar’s Arrangement Position fields.

Set the Play Position in the Arrangement Position Fields.

Within the Arrangement Position fields, the play position reads out as bars-beats-sixteenths. With one field selected, its value is editable in several ways:

- Drag the mouse up or down to change it.
- Key in a number, then hit Enter.
- Press the up and down arrow keys to raise or lower it.

Editing the Arrangement Position fields shifts the insert marker right along with it.

The scrub area above the tracks gives you yet another way to begin playback. By default the Permanent Scrub Areas option stays on in Live’s Display & Input Settings, so a click anywhere in the scrub area kicks off playback from that spot.

Use the Scrub Area to Launch Playback.

As you click from one point in the scrub area to another, the leap between fired play positions is quantized by the Quantization Menu’s setting in the Control Bar. Holding the left mouse button at a chosen spot in the scrub area instead repeats a portion of the Arrangement, following the global launch quantization value.

Should the Permanent Scrub Areas option be turned off, you can still scrub the Arrangement by Shift-clicking somewhere in the scrub area or along the beat-time ruler.

The editor in [the Clip View](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view) carries its own per-clip scrub area as well, which can fire playback.

So that MIDI notes still sound when playback begins partway into a note, Live chases MIDI notes by default. That behavior can be switched off or back on through the Chase MIDI Notes command in the Options menu.
