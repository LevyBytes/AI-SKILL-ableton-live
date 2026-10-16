# Link Setup Sync And Audio

Open when you need guidance on Link Setup Sync And Audio in Ableton Live.

Context: [Synchronizing via Link](synchronizing-with-link-tempo-follower-and-midi.md#361-synchronizing-via-link).

<a id="source-3611-setting-up-link"></a>
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

<a id="source-3612-using-link"></a>
### 36.1.2 Using Link

Before running Link in Live, confirm that your computer shares a network with whatever other devices you intend to sync. A dependable WiFi network works, and so does a wired link. After that, hit the Link toggle at the top-left corner of the Live window to switch Link on, and Live will, on its own, either launch a Link session or join one already running.

As soon as Link comes on, the toggle reports how many peers are present in the Link session.

Link Toggle Shows The Number of Link Session Peers.

Provided that one or more other Link-enabled apps or copies of Live are connected, the Arrangement Position control displays a progress bar any time Live’s transport sits idle. That bar charts the Live Set’s global launch quantization against the same quantization of the other members in the Link session. Once you fire off playback, Live holds until the progress bar finishes before it actually begins playing.

Arrangement Position Shows Relation to Link Timeline.

Whichever device enters a Link session first establishes the opening tempo for the rest of the connected peers. From there, any Link-enabled app, device, or copy of Live may alter its tempo whenever it likes, and the others fall in line. Should several members reach for the tempo at once, everyone else still tries to keep up, yet the value ends up wherever the most recent change put it. Any tempo move by a Link session member takes precedence over the tempo automation in your Live Set.

Bear in mind that the metronome’s [recording count-in](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-with-count-in) is unavailable while Link is switched on.

For the most part Link behaves flawlessly the moment you enable it and delivers dependable sync under almost any circumstances. Should something go wrong, take a look at the [Link FAQ](https://help.ableton.com/hc/en-us/articles/209776125) over in the Knowledge Base.

<a id="source-3613-using-link-audio"></a>
### 36.1.3 Using Link Audio

Once it is on, Link Audio lets you pipe audio in real time among Link-enabled devices that share a network. That, in turn, lets you monitor and capture audio from other devices and apps right inside Live. For Link Audio to work, double-check that every peer has both Link and Link Audio switched on.

After that, audio coming from the other members of the Link session shows up as an input source within Live. To monitor or record what is arriving, pick a peer through the Input Type chooser on an armed audio track, then choose the source track you want with the Input Channel chooser.

Choose a Link Peer as the Input Type.

Any track that produces audio output may be streamed out to connected peers. Worth noting: with Live and Push you can both transmit and receive audio over Link Audio, whereas certain other apps only handle the sending side.

Should Link Audio give you trouble, glance through the [Link Audio FAQ](https://help.ableton.com/hc/en-us/articles/25425913328924-Link-Audio-FAQ) in the Knowledge Base.
