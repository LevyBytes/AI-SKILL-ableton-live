# MPE Overview

Open when you need guidance on MPE Overview in Ableton Live.

<a id="source-editing-mpe-converting-audio-to-midi"></a>

<a id="source-overview"></a>

<a id="source-12-editing-mpe"></a>
## 12. Editing MPE

<a id="source-12-editing-mpe-1"></a>
### 12. Editing MPE

MIDI Polyphonic Expression (MPE) extends the MIDI specification so that parameter control data can be tied to single notes rather than applied across an entire MIDI channel at once. Because of this approach, MPE-capable devices are able to shape several parameters of each note live, opening the door to richer, more expressive playing.

Before Live can take in per-note expression coming from an MPE-capable MIDI controller, switch on MPE Mode within that controller's Link, Tempo & MIDI Settings.

Enabling MPE Mode for a MIDI Controller.

Keep in mind that once you pick a MIDI controller with MPE turned on as a track's input device, its channel input routing locks to “All Channels’’ and you cannot pick out single channels.

If you'd like additional guidance on handling MIDI controllers, consult the [MIDI and Key Remote Control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) chapter. After your controller is configured, it can drive the process of [record new MIDI clips](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips) that hold MPE data.

Through the Clip View’s Note Expression tab, for every note in a clip, you can inspect and adjust these five MPE dimensions: Pitch (per-note pitch bend); next comes Slide (per-note Y-Axis); after that, Pressure (Poly Aftertouch/MPE Pressure); plus the two velocity-based ones, Velocity and Release Velocity (Note Off Velocity). With these controls you can polish how recorded passages express themselves, or program polyphonic timbral movement for MPE-capable instruments.

Bear in mind that MPE data for notes is viewable and editable in every MIDI clip, no matter if those clips originated from an MPE-capable device or through [other methods](https://www.ableton.com/en/live-manual/12/editing-midi/#creating-a-midi-clip). The sections that follow walk through inspecting and adjusting MPE data.
