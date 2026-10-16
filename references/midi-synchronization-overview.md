# MIDI Synchronization Overview

Open when you need guidance on MIDI Synchronization Overview in Ableton Live.

Context: [Synchronizing with Link, Tempo Follower, and MIDI](synchronizing-with-link-tempo-follower-and-midi.md#36-synchronizing-with-link-tempo-follower-and-midi).

<a id="source-363-synchronizing-via-midi"></a>
### 36.3 Synchronizing via MIDI

When the gear you are using has no Link support, MIDI offers another route to sync. The MIDI protocol lays out two methods for synchronizing sequencers, and Live handles both. Each method rests on the idea of a sync _host_ that puts out a sync signal, which the sync _device(s)_ then follow.

MIDI Clock: think of MIDI Clock as a metronome that ticks very quickly. How fast those incoming ticks arrive depends on the tempo: nudging the tempo on the sync host (a drum machine, say) makes the device track that move. On top of the ticks, the MIDI Clock protocol carries messages that report where you are in the song. As far as MIDI Clock goes, Live is able to serve as either a MIDI sync host or a device.

MIDI Timecode: this is the MIDI flavor of the SMPTE protocol, the customary way of locking tape machines and computers together throughout the audio and film world. Each MIDI Timecode message pins down a time stated in seconds and frames (fractions of a second). Live treats such a Timecode message as a spot within the Arrangement. Because those messages hold nothing about meter, slaving Live to another sequencer over MIDI Timecode means you must set the tempo yourself by hand. Tempo shifts can’t be tracked. The full rundown of MIDI Timecode Settings appears [later in this chapter](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#midi-timecode-options). Where MIDI Timecode is concerned, Live can serve solely as a MIDI sync device and never as a host.
