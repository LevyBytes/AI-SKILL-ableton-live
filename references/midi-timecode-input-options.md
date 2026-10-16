# MIDI Timecode Input Options

Open when you need guidance on MIDI Timecode Input Options in Ableton Live.

Context: [Synchronizing Live to External MIDI Devices](synchronizing-with-link-tempo-follower-and-midi.md#3632-synchronizing-live-to-external-midi-devices).

<a id="source-36321-midi-timecode-options"></a>
#### 36.3.2.1 MIDI Timecode Options

Timecode options are configured on a per-MIDI-device basis. To reach them, pick a MIDI device out of the MIDI Ports list inside the Tempo & MIDI Settings.

The _MIDI Timecode Frame Rate_ setting matters only when “MIDI Timecode“ has been picked in the MIDI Sync Type menu. Through the MIDI Timecode Rate chooser you decide which sort of Timecode Live should lock onto. Every one of the standard SMPTE frame rates is offered. Set the Rate to “SMPTE All,“ and Live figures out the Timecode format of arriving sync messages on its own, reading them to match. It is also worth knowing that the Timecode format shown in the Arrangement View can be changed: open the Options menu and dig into the Time Ruler Format sub-menu.

The _MIDI Timecode Offset_ setting, too, applies only when “MIDI Timecode“ is the choice in the Sync Type menu. This control lets you enter a SMPTE time offset, and Live reads that figure as the Arrangement’s starting time.
