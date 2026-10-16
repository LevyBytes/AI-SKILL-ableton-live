# MPE Zones And Multichannel Settings

Open when you need guidance on MPE Zones And Multichannel Settings in Ableton Live.

Context: [MPE/Multi-channel Settings](mpe-and-audio-midi-routes.md#126-mpemulti-channel-settings).

<a id="source-1261-accessing-the-mpemulti-channel-settings-dialog"></a>
### 12.6.1 Accessing the MPE/Multi-channel Settings Dialog

Within the Ext. Instrument device, pick your Routing Target from the MIDI To drop-down menu. Next choose MPE in the second drop-down, reopen the menu, and pick MPE Settings…

The MPE Settings in Ext. Instrument.

To reach these settings from the mixer's I/O section, confirm that the device you wish to control is picked in the MIDI To section of the MIDI track’s output. Within the Session or Arrangement Mixer, set the MIDI To drop-down menu to MPE; then reopen that drop-down menu and choose MPE Settings…

The MPE Settings in the I/O Section.

With MPE-enabled plug-ins, these settings live in the context menu of the device’s title bar.

The MPE Settings in a Plug-in Context Menu.

<a id="source-1262-the-mpemulti-channel-settings-dialog"></a>
### 12.6.2 The MPE/Multi-Channel Settings Dialog

The MPE/Multi-channel Settings.

These settings let you:

- Configure the MPE zone and the span of note channels Live employs when it sends MPE out to an external MIDI device or plug-in.
- Select the upper or lower zone and number of note channels.
- Select multi-channel mode, which sets an arbitrary range of note channels.

Options exist for both the lower zone and the upper zone. Since a track outputs to only one zone at a time, you'll need two tracks to drive both zones.

Every zone requires a global channel (used for non-polyphonic controls). For the lower zone that global channel is Channel 1, while Channel 16 serves the upper zone. Beyond that, you can hand a span of the remaining MIDI channels to each zone (broadly speaking, the count of channels you give a zone corresponds to how much polyphony you want there). One sample zone configuration could put channels 1-11 in the lower zone and channels 12-16 in the upper zone.

Note: Live supports zones for MPE output only, which proves especially handy with hardware synths that call for a specific zone configuration.

You could also rely on these settings, for instance, to hook two MPE synths up to a single MIDI interface (once more, with one connected via the MIDI thru of the other), or to arrange a synth that drives two distinct sounds by assigning them to separate zones. Two MIDI tracks in Live, both routed to the same MIDI output device, can be set so that one track handles the lower zone and the other the upper zone.
