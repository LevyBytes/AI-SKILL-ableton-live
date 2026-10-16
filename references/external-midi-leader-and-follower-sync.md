# External MIDI Leader And Follower Sync

Open when you need guidance on External MIDI Leader And Follower Sync in Ableton Live.

Context: [Synchronizing via MIDI](synchronizing-with-link-tempo-follower-and-midi.md#363-synchronizing-via-midi).

<a id="source-3631-synchronizing-external-midi-devices-to-live"></a>
### 36.3.1 Synchronizing External MIDI Devices to Live

Live is capable of transmitting MIDI Clock messages out to an external MIDI sequencer (or drum machine). Once the sequencer is hooked up to Live and configured to accept MIDI sync, switch that device on as a sync destination within Live’s Tempo & MIDI Settings.

Choosing a MIDI Device for Live.

Whenever Live is pushing sync messages out to external sequencers, the lower indicator LED beside the Control Bar’s EXT button blinks.

<a id="source-3632-synchronizing-live-to-external-midi-devices"></a>
### 36.3.2 Synchronizing Live to External MIDI Devices

Going the other way, Live itself can be slaved over MIDI to an external sequencer. Once the sequencer is connected to Live and set up to transmit sync, point Live at that connection using Live’s Tempo & MIDI Settings.

Setting up Live as a MIDI Device.

As soon as an external sync source is turned on, the EXT button shows up in the Control Bar. From there you engage external sync either by clicking that button on or by invoking the External Sync command from the Options menu. The upper indicator LED beside the EXT button blinks whenever Live takes in usable sync messages.

The External Sync Switch.

While Live is locked to an external MIDI device, it can take in song position pointers from that device, lining itself up not just by tempo but by where it sits in the song. Should the host leap to a different spot in the song, Live jumps right along with it. That said, if the Control Bar’s Loop switch is on, playback loops and those song position pointers simply get “wrapped“ to fit the loop’s length.
