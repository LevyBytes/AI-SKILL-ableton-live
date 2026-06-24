# Synchronizing With Link Tempo Follower And Midi

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 36. Synchronizing with Link, Tempo Follower, and MIDI

Whenever you collaborate across several machines, pair Live up with other Ableton products or additional copies of Live, or bring outside hardware into the picture, keeping the timing aligned between those apps and devices becomes a concern. To handle this, Live gives you a handful of distinct methods for holding everything together rhythmically.

### 36.1 Synchronizing via Link

As a technology, Ableton Link locks the musical beat, tempo, and phase together for several apps or devices that share a wired or wireless network. On top of that, it lets you carry live audio in real time among the members of a Link session, also known as _peers_, with no extra gear and none of the fiddly routing such a setup would otherwise demand.

Every Ableton product ships with Link already inside, and an ever-larger pool of [third-party apps and hardware devices](https://www.ableton.com/en/link/products/) supports it too. Each member of a Link session is free to begin or halt playback on its own while still holding time and phase with the other connected peers, since playback honors the global launch quantization. Likewise, anyone may nudge the tempo, and that adjustment carries through to every connected app or device. Members are also welcome to drop in or out whenever they please, leaving the session undisturbed.

Link sync can run side by side with either [Tempo Follower](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-via-tempo-follower) or [MIDI](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-via-midi) synchronization. Either way, the tempo Live picks up from the external input is the one it feeds to the Link session.

### 36.1.1 Setting up Link

To set Link up, head to its own dedicated tab inside Live’s Settings.

The Link Tab in Live’s Settings.

By default the Link toggle that switches Link on sits in the Control Bar, but should you have no plans to use the feature, you can tuck the toggle out of the Control Bar by flipping the _Show Link Toggle_ option to _Hide_.

Where the Link Toggle sits within the Control Bar.Hiding that Link Toggle from Live’s Settings.

Beside the Link toggle is a drop-down menu that lets you flip the central Link and Link Audio capabilities on or off in a hurry. That menu also shows every connected peer running the Link Audio option, plus a _Configure Link…_ entry that jumps straight to the Link tab in Live’s Settings.

To keep start and stop commands aligned among peers, switch on the _Start Stop Sync_ option. Keep in mind that those commands travel only to peers who have likewise turned this option on.

Enable the Start Stop Sync Option.

The remaining controls on this page tie into the [Link Audio](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#using-link-audio) feature.

Link Audio Settings.

Turning the Audio option on or off activates or deactivates Link Audio. Bear in mind that it functions solely while Link itself is switched on.

The Name field is where you type the label that other peers in a Link session will see for you.

With the Latency slider you dial in how much input latency gets applied to audio coming in. Each tweak to that latency refreshes the quantity of buffered audio shown for every participant in the peer roster underneath.

Switching on the Sync to Incoming Audio option keeps any audio arriving over Link and monitored inside Live lined up with Live’s own audio and clips. Live pulls this off by holding back its playback by the latency figure you set. Take note that, for Link Audio to operate correctly, only a single participant in the session ought to turn this option on.

Every connected Link Audio peer shows up in the peers list, together with its status and how much audio it has buffered.

### 36.1.2 Using Link

Before running Link in Live, confirm that your computer shares a network with whatever other devices you intend to sync. A dependable WiFi network works, and so does a wired link. After that, hit the Link toggle at the top-left corner of the Live window to switch Link on, and Live will, on its own, either launch a Link session or join one already running.

As soon as Link comes on, the toggle reports how many peers are present in the Link session.

Link Toggle Shows The Number of Link Session Peers.

Provided that one or more other Link-enabled apps or copies of Live are connected, the Arrangement Position control displays a progress bar any time Live’s transport sits idle. That bar charts the Live Set’s global launch quantization against the same quantization of the other members in the Link session. Once you fire off playback, Live holds until the progress bar finishes before it actually begins playing.

Arrangement Position Shows Relation to Link Timeline.

Whichever device enters a Link session first establishes the opening tempo for the rest of the connected peers. From there, any Link-enabled app, device, or copy of Live may alter its tempo whenever it likes, and the others fall in line. Should several members reach for the tempo at once, everyone else still tries to keep up, yet the value ends up wherever the most recent change put it. Any tempo move by a Link session member takes precedence over the tempo automation in your Live Set.

Bear in mind that the metronome’s [recording count-in](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-with-count-in) is unavailable while Link is switched on.

For the most part Link behaves flawlessly the moment you enable it and delivers dependable sync under almost any circumstances. Should something go wrong, take a look at the [Link FAQ](https://help.ableton.com/hc/en-us/articles/209776125) over in the Knowledge Base.

### 36.1.3 Using Link Audio

Once it is on, Link Audio lets you pipe audio in real time among Link-enabled devices that share a network. That, in turn, lets you monitor and capture audio from other devices and apps right inside Live. For Link Audio to work, double-check that every peer has both Link and Link Audio switched on.

After that, audio coming from the other members of the Link session shows up as an input source within Live. To monitor or record what is arriving, pick a peer through the Input Type chooser on an armed audio track, then choose the source track you want with the Input Channel chooser.

Choose a Link Peer as the Input Type.

Any track that produces audio output may be streamed out to connected peers. Worth noting: with Live and Push you can both transmit and receive audio over Link Audio, whereas certain other apps only handle the sending side.

Should Link Audio give you trouble, glance through the [Link Audio FAQ](https://help.ableton.com/hc/en-us/articles/25425913328924-Link-Audio-FAQ) in the Knowledge Base.

### 36.2 Synchronizing via Tempo Follower

There are moments when neither a Link connection nor MIDI Clock is on hand. Other times you simply may not want a stiff, machine-driven clock at all. Perhaps you would rather have Live’s tempo ride along with the organic ebb and flow of a drummer in your group, or maybe you are aiming to lock onto a pair of turntables in the middle of a DJ set. That is exactly the job Tempo Follower handles. It examines an incoming audio signal as it happens and reads its tempo, so that Live can trail behind and stay on beat.

### 36.2.1 Setting Up Tempo Follower

Pointing Tempo Follower at an external audio input begins by opening Live’s Tempo & MIDI Settings. Within the Tempo Follower section, dial the Input Channel (Ext. In) to whichever input on your audio interface is wired to the source you mean to track. With a drum kit, that may well be an overhead microphone set aside for the purpose. With turntables, you might instead route a record output or an effects loop off a DJ mixer. Bear in mind that, although the Tempo Follower algorithm is tuned for audio carrying a distinct rhythm, nothing stops you from getting inventive and trying out other kinds of sources.

Tempo Follower Settings in Live’s Settings.

Turn on the _Show Tempo Follower Toggle_ option and the Tempo Follower toggle pops into view in the Control Bar, sitting on the left next to the rest of the tempo-related parameters.

The Tempo Follower Toggle in the Control Bar.

Click the “Follow” button and Tempo Follower springs to life, with Live tuning in to the audio source you configured and reading its tempo. Be aware that Tempo Follower stays idle whenever the Follow button is out of sight.

If Tempo Follower is unable to reach the audio input device channel you named in the Settings, the feature shuts off and the Follow button shows up grayed out.

Keep in mind that Tempo Follower and External Sync cannot both be on at once; turning Tempo Follower on disables the External Sync option. While Tempo Follower runs, Live can still push MIDI clock information out to external gear, though it has no way to take any in.

### 36.3 Synchronizing via MIDI

When the gear you are using has no Link support, MIDI offers another route to sync. The MIDI protocol lays out two methods for synchronizing sequencers, and Live handles both. Each method rests on the idea of a sync _host_ that puts out a sync signal, which the sync _device(s)_ then follow.

MIDI Clock: think of MIDI Clock as a metronome that ticks very quickly. How fast those incoming ticks arrive depends on the tempo: nudging the tempo on the sync host (a drum machine, say) makes the device track that move. On top of the ticks, the MIDI Clock protocol carries messages that report where you are in the song. As far as MIDI Clock goes, Live is able to serve as either a MIDI sync host or a device.

MIDI Timecode: this is the MIDI flavor of the SMPTE protocol, the customary way of locking tape machines and computers together throughout the audio and film world. Each MIDI Timecode message pins down a time stated in seconds and frames (fractions of a second). Live treats such a Timecode message as a spot within the Arrangement. Because those messages hold nothing about meter, slaving Live to another sequencer over MIDI Timecode means you must set the tempo yourself by hand. Tempo shifts can’t be tracked. The full rundown of MIDI Timecode Settings appears [later in this chapter](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#midi-timecode-options). Where MIDI Timecode is concerned, Live can serve solely as a MIDI sync device and never as a host.

### 36.3.1 Synchronizing External MIDI Devices to Live

Live is capable of transmitting MIDI Clock messages out to an external MIDI sequencer (or drum machine). Once the sequencer is hooked up to Live and configured to accept MIDI sync, switch that device on as a sync destination within Live’s Tempo & MIDI Settings.

Choosing a MIDI Device for Live.

Whenever Live is pushing sync messages out to external sequencers, the lower indicator LED beside the Control Bar’s EXT button blinks.

### 36.3.2 Synchronizing Live to External MIDI Devices

Going the other way, Live itself can be slaved over MIDI to an external sequencer. Once the sequencer is connected to Live and set up to transmit sync, point Live at that connection using Live’s Tempo & MIDI Settings.

Setting up Live as a MIDI Device.

As soon as an external sync source is turned on, the EXT button shows up in the Control Bar. From there you engage external sync either by clicking that button on or by invoking the External Sync command from the Options menu. The upper indicator LED beside the EXT button blinks whenever Live takes in usable sync messages.

The External Sync Switch.

While Live is locked to an external MIDI device, it can take in song position pointers from that device, lining itself up not just by tempo but by where it sits in the song. Should the host leap to a different spot in the song, Live jumps right along with it. That said, if the Control Bar’s Loop switch is on, playback loops and those song position pointers simply get “wrapped“ to fit the loop’s length.

#### 36.3.2.1 MIDI Timecode Options

Timecode options are configured on a per-MIDI-device basis. To reach them, pick a MIDI device out of the MIDI Ports list inside the Tempo & MIDI Settings.

The _MIDI Timecode Frame Rate_ setting matters only when “MIDI Timecode“ has been picked in the MIDI Sync Type menu. Through the MIDI Timecode Rate chooser you decide which sort of Timecode Live should lock onto. Every one of the standard SMPTE frame rates is offered. Set the Rate to “SMPTE All,“ and Live figures out the Timecode format of arriving sync messages on its own, reading them to match. It is also worth knowing that the Timecode format shown in the Arrangement View can be changed: open the Options menu and dig into the Time Ruler Format sub-menu.

The _MIDI Timecode Offset_ setting, too, applies only when “MIDI Timecode“ is the choice in the Sync Type menu. This control lets you enter a SMPTE time offset, and Live reads that figure as the Arrangement’s starting time.

### 36.3.3 Sync Delay

Provided individually for every MIDI device, the _Sync Delay_ controls let you shift Live’s internal time base relative to the sync signal. That comes in handy for making up the delays that signal transmission introduces. A given device’s Sync Delay becomes visible once you choose that MIDI device from the MIDI Ports list in the Tempo & MIDI Settings. To set it, get both Live and the other sequencer playing a rhythmic figure full of sharp percussive hits. Listening to the two outputs together, work the Sync Delay control until the sounds land in flawless sync.

Adjusting Sync Delay.
