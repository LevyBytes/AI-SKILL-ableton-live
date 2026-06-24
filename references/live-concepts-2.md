# Live Concepts (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

After a signal travels through the device chain, its final stop is Live’s [mixer](https://www.ableton.com/en/live-manual/12/mixing/#the-live-mixer). Because the same pool of tracks underlies both the Session and the Arrangement, those views rely on a single shared mixer too. For convenience, that mixer is available from either view.

The Live Mixer shown within the Arrangement View.

You can declutter the screen by toggling each mixer section on or off — either through the Mixer Controls entries under the View menu or via the choices in the Mixer Config Menu tucked into the lower right of Live’s window.

The options found in the Mixer Config Menu.

Among the mixer’s controls are volume, pan position, and _sends_, the last of which set how large a portion of a track’s output is routed into the matching _return track’s_ input. A return track holds effects exclusively — never clips. Through their sends, every track is able to route some of its signal toward a return track and tap into the effects it carries.

Built into the mixer as well is a [crossfader](https://www.ableton.com/en/live-manual/12/mixing/#using-lives-crossfader) for blending seamlessly between clips that play across separate tracks. Although Live’s crossfader behaves much like the crossfader on a standard DJ mixer, it goes further by letting you blend across any quantity of tracks rather than only two — the returns included.

The Crossfader and the buttons that assign tracks to it.

Picture a MIDI track running a clip. That clip’s MIDI signal flows into the device chain belonging to the track. Inside, it first encounters however many MIDI effects sit there. Each MIDI effect takes in MIDI and passes MIDI back out. After the final MIDI effect comes an instrument, which accepts MIDI and produces audio. Beyond the instrument you may place any quantity of audio effects, just like on an audio track.

A MIDI Effect, an Instrument and a few Audio Effects within a MIDI Track.

When a MIDI track carries neither an instrument nor any audio effects, its output stays a bare MIDI signal that must be routed elsewhere before it can turn into audio. Under those circumstances, the mixer no longer displays that track’s mix and send controls.

The Mixer as it appears for a MIDI Track lacking an Instrument.

### 3.15 Presets and Racks

Each Live device is able to save and recall specific configurations of parameter values as [presets](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#live-device-presets). Since presets live apart from individual Live Sets, any preset you create joins your User Library and is then reachable from every project.

With Live’s [Instrument, Drum and Effect Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks), you can bundle several devices together with their settings and store the whole thing as one preset. That ability lets you assemble rich multi-device constructions, in effect lending all of Live’s MIDI and audio effects to its native instruments.

### 3.16 Routing

Every track outputs a signal, whether audio or MIDI. You define where those signals go in the mixer’s _In/Out section_, where each track has a chooser for its signal source and another for its destination. Reachable through the In/Out entry in the View menu’s Mixer Controls submenu, the In/Out section acts as Live’s “patchbay.“ The [routing options](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) it offers unlock useful creative and technical workflows — among them resampling, submixing, stacking synths, elaborate effects rigs, and beyond.

Track Routing is configured through the In/Out Section.

A track’s signal can leave Live by way of the computer’s audio and MIDI interfaces, headed for other applications hooked up to tracks or to devices inside Live. You may also fold several tracks into a [_group track_](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks), which acts as a submixer for whichever tracks you chose.

In the same way, a track can be configured to take in an incoming signal and run it through that track’s devices. Once again, a track may draw its input from beyond Live or from a different track or device within Live. The _monitoring_ controls govern exactly when the incoming signal becomes audible through the track.

Signals may also be sent out to external hardware from inside a track’s device chain, which you do with the [External Audio Effect](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#external-audio-effect) and [External Instrument](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#external-instrument) devices.

### 3.17 Recording New Clips

Both audio and MIDI tracks are capable of capturing their incoming signal to [create new clips](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips). You switch recording on for a track by clicking its _Arm button_. When several tracks are selected, clicking any one of their Arm buttons arms the whole selection. Alternatively, holding the Ctrl (Win) / Cmd (Mac) modifier as you click the Arm buttons lets you arm a handful of tracks together. Should the Exclusive Arm option be turned on in the [Record, Warp & Launch Settings](https://www.ableton.com/en/live-manual/12/first-steps/#record-warp--launch), dropping an instrument onto a fresh or empty MIDI track arms that track on its own. Once the Control Bar’s Arrangement Record button is lit, each armed track captures its incoming signal into the Arrangement. Each pass produces a fresh clip on every track.

The Arm Buttons on tracks.

You can likewise [record into Session View slots](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-into-session-slots) as you go. Musicians who like to jam find this handy, since recording in the Session never forces the music to stop. Pressing the Session Record button captures a fresh clip into the chosen Session scene across all armed tracks.

The Session Record Button on the Control Bar.

Pressing the Session Record button a second time halts recording and fires off the newly made clips. Since those operations obey real-time _launch\*\*quantization_, the clips that result can snap automatically to the beat.

The Quantization Chooser on the Control Bar.

Pairing Session recording with _overdubbing_ and _Record Quantization_ is the go-to approach for building drum patterns, which grow as you keep layering notes onto the pattern while it cycles in a loop. All you need to pull this off is a MIDI keyboard (or your computer keyboard) plus a MIDI track holding Live’s [Impulse](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#impulse) percussion instrument.

### 3.18 Automation Envelopes

It often happens that, while you tweak Live’s mixer and effects, you’d like the changes you make to those control values to be kept as part of the Set. Such shifts in a control’s value as they unfold along the Arrangement timeline or within a Session clip are termed [automation](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#automation-and-editing-envelopes); any control whose value moves over time is said to be _automated_. Live depicts automation as _breakpoint envelopes_, which you can draw, edit, and capture live.

Automated Parameters as seen in the Arrangement View.

Nearly every mixer and effect control in Live is open to automation, the song tempo among them. Capturing automation is simple: whatever you change on a control while the Control Bar’s Automation Arm and Arrangement Record buttons are lit turns into automation in the Arrangement View. When you adjust controls during recording with the Automation Arm button enabled, that automation is written into Session View clips.

Adjusting an automated control’s value while you are _not_ recording resembles firing a Session clip during Arrangement playback: it switches off that control’s automation in favor of whatever you just set. From then on the control ignores its automation and holds the new value until you click the Re-Enable Automation button or trigger a Session clip carrying automation.

### 3.19 Clip Envelopes

Tracks and clips alike can hold envelopes. You use [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) to automate or modulate the controls of devices and the mixer. Audio clips carry further clip envelopes that affect a clip’s pitch, volume, and other traits — handy for reshaping the melody and rhythm of recorded sound. MIDI clips, for their part, gain extra clip envelopes that stand in for MIDI controller data. You can _unlink_ a clip envelope from its clip so it follows its own loop settings, allowing sweeping moves (such as fade-outs) or finer gestures (such as an arpeggio) to be layered over the clip’s content.

An Envelope used for Clip Transposition.

### 3.20 MIDI and Key Remote

So the musician need not stay tied to the mouse, the bulk of Live’s controls can be driven remotely from an outboard MIDI controller. You set up these remote links in [MIDI Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#assigning-midi-remote-control), which you enter by clicking the MIDI switch in the Control Bar.

While in this mode, click any mixer or effect control and bind it to a controller just by transmitting the MIDI message you want (say, by twisting a knob on your MIDI control box). The moment you exit MIDI Map Mode, your bindings go live. You can also map Session clips to a single MIDI key or to a whole keyboard range for chromatic performance.

Once MIDI keys and controllers are mapped to Live’s controls, they can no longer be used to record through MIDI tracks. Those messages get stripped out before the arriving MIDI reaches the MIDI tracks.

The Key/MIDI Map Controls.

Session clips, switches, buttons, and radio buttons can likewise be tied to keys on the computer keyboard. You do this in [Key Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control), which operates exactly like MIDI Map Mode.

Beyond this all-purpose mapping approach, Live provides built-in support specifically for [Ableton Push 1](https://www.ableton.com/en/live-manual/12/using-push-1/#using-push-1), [Push 2](https://www.ableton.com/en/live-manual/12/using-push-2/#using-push-2), and [Push 3](https://www.ableton.com/push/manual/).

### 3.21 Saving and Exporting

When you save a Live Set, all of its contents are preserved, including every clip together with its placement and settings, plus the settings for devices and controls. That said, an audio clip may break the link to the sample it points to if that sample gets relocated or erased from disk. You can safeguard the connections between samples and their clips through a dedicated command, [Collect All and Save](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#collecting-external-files), which duplicates every sample and tucks the copies into a project folder beside the Live Set.

An audio clip’s Clip Title Bar features its own Save button, which lets you store a batch of [default clip settings](https://www.ableton.com/en/live-manual/12/clip-view/#saving-default-audio-clip-settings-with-the-sample) alongside the sample; that way, every time you drag the sample into the program it loads automatically with those settings. This comes in especially handy when a clip has particular warp settings you intend to reuse across several Live Sets.

You can export audio out of Live from either the Session or Arrangement View — choose ‘Export Audio/Video’ in the File menu, or press the shortcut CtrlShiftR (Win) / CmdShiftR (Mac). Out of the box, Live renders whatever arrives at the Main output into an audio file matching the specifications you set in the [Export Audio/Video](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video) dialog options.

Individual MIDI clips can be exported from Live as [MIDI files](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-midi-files) as well.

A very handy way to export and store material for reuse in Live is the [Live Clip](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-clips) format. You can drag Session View clips straight out of a Live Set into the User Library, exporting them to disk as Live Clips in the process.

A Live Clip displayed in the Browser.

[Live Clips](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-clips) make an especially potent way to bank ideas, because they preserve not just the clip’s Clip View settings but also the instruments and effects chain belonging to its track. From the browser you can audition Live Clips and drop them into any open Live Set the same way you would sample files. After they load into a Live Set, they come back with their original envelope and device settings intact.

By means of Live Clips, you can assemble a personal library of your own consisting of:

- MIDI sequences paired with their instruments and effects — for instance, a MIDI drum pattern carrying the related Impulse and effects settings;
- Different [regions or loops](https://www.ableton.com/en/live-manual/12/clip-view/#clip-gain-and-pitch) that reference one and the same source file;
- Variations on a sample loop made by applying [Warp Markers](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping), [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes), and [effects](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects);
- Ideas that might not suit your present project yet could prove handy down the line.
