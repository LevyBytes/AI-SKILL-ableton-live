# Rack Routing Recording And Automation Concepts

Open when you need guidance on Rack Routing Recording And Automation Concepts in Ableton Live.

Context: [Live Concepts](live-concepts.md#3-live-concepts).

<a id="source-315-presets-and-racks"></a>
### 3.15 Presets and Racks

Each Live device is able to save and recall specific configurations of parameter values as [presets](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#live-device-presets). Since presets live apart from individual Live Sets, any preset you create joins your User Library and is then reachable from every project.

With Live’s [Instrument, Drum and Effect Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks), you can bundle several devices together with their settings and store the whole thing as one preset. That ability lets you assemble rich multi-device constructions, in effect lending all of Live’s MIDI and audio effects to its native instruments.

<a id="source-316-routing"></a>
### 3.16 Routing

Every track outputs a signal, whether audio or MIDI. You define where those signals go in the mixer’s _In/Out section_, where each track has a chooser for its signal source and another for its destination. Reachable through the In/Out entry in the View menu’s Mixer Controls submenu, the In/Out section acts as Live’s “patchbay.“ The [routing options](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) it offers unlock useful creative and technical workflows — among them resampling, submixing, stacking synths, elaborate effects rigs, and beyond.

Track Routing is configured through the In/Out Section.

A track’s signal can leave Live by way of the computer’s audio and MIDI interfaces, headed for other applications hooked up to tracks or to devices inside Live. You may also fold several tracks into a [_group track_](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks), which acts as a submixer for whichever tracks you chose.

In the same way, a track can be configured to take in an incoming signal and run it through that track’s devices. Once again, a track may draw its input from beyond Live or from a different track or device within Live. The _monitoring_ controls govern exactly when the incoming signal becomes audible through the track.

Signals may also be sent out to external hardware from inside a track’s device chain, which you do with the [External Audio Effect](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#external-audio-effect) and [External Instrument](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#external-instrument) devices.

<a id="source-317-recording-new-clips"></a>
### 3.17 Recording New Clips

Both audio and MIDI tracks are capable of capturing their incoming signal to [create new clips](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips). You switch recording on for a track by clicking its _Arm button_. When several tracks are selected, clicking any one of their Arm buttons arms the whole selection. Alternatively, holding the Ctrl (Win) / Cmd (Mac) modifier as you click the Arm buttons lets you arm a handful of tracks together. Should the Exclusive Arm option be turned on in the [Record, Warp & Launch Settings](https://www.ableton.com/en/live-manual/12/first-steps/#record-warp--launch), dropping an instrument onto a fresh or empty MIDI track arms that track on its own. Once the Control Bar’s Arrangement Record button is lit, each armed track captures its incoming signal into the Arrangement. Each pass produces a fresh clip on every track.

The Arm Buttons on tracks.

You can likewise [record into Session View slots](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-into-session-slots) as you go. Musicians who like to jam find this handy, since recording in the Session never forces the music to stop. Pressing the Session Record button captures a fresh clip into the chosen Session scene across all armed tracks.

The Session Record Button on the Control Bar.

Pressing the Session Record button a second time halts recording and fires off the newly made clips. Since those operations obey real-time _launch\*\*quantization_, the clips that result can snap automatically to the beat.

The Quantization Chooser on the Control Bar.

Pairing Session recording with _overdubbing_ and _Record Quantization_ is the go-to approach for building drum patterns, which grow as you keep layering notes onto the pattern while it cycles in a loop. All you need to pull this off is a MIDI keyboard (or your computer keyboard) plus a MIDI track holding Live’s [Impulse](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#impulse) percussion instrument.

<a id="source-318-automation-envelopes"></a>
### 3.18 Automation Envelopes

It often happens that, while you tweak Live’s mixer and effects, you’d like the changes you make to those control values to be kept as part of the Set. Such shifts in a control’s value as they unfold along the Arrangement timeline or within a Session clip are termed [automation](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#automation-and-editing-envelopes); any control whose value moves over time is said to be _automated_. Live depicts automation as _breakpoint envelopes_, which you can draw, edit, and capture live.

Automated Parameters as seen in the Arrangement View.

Nearly every mixer and effect control in Live is open to automation, the song tempo among them. Capturing automation is simple: whatever you change on a control while the Control Bar’s Automation Arm and Arrangement Record buttons are lit turns into automation in the Arrangement View. When you adjust controls during recording with the Automation Arm button enabled, that automation is written into Session View clips.

Adjusting an automated control’s value while you are _not_ recording resembles firing a Session clip during Arrangement playback: it switches off that control’s automation in favor of whatever you just set. From then on the control ignores its automation and holds the new value until you click the Re-Enable Automation button or trigger a Session clip carrying automation.

<a id="source-319-clip-envelopes"></a>
### 3.19 Clip Envelopes

Tracks and clips alike can hold envelopes. You use [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) to automate or modulate the controls of devices and the mixer. Audio clips carry further clip envelopes that affect a clip’s pitch, volume, and other traits — handy for reshaping the melody and rhythm of recorded sound. MIDI clips, for their part, gain extra clip envelopes that stand in for MIDI controller data. You can _unlink_ a clip envelope from its clip so it follows its own loop settings, allowing sweeping moves (such as fade-outs) or finer gestures (such as an arpeggio) to be layered over the clip’s content.

An Envelope used for Clip Transposition.

<a id="source-320-midi-and-key-remote"></a>
### 3.20 MIDI and Key Remote

So the musician need not stay tied to the mouse, the bulk of Live’s controls can be driven remotely from an outboard MIDI controller. You set up these remote links in [MIDI Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#assigning-midi-remote-control), which you enter by clicking the MIDI switch in the Control Bar.

While in this mode, click any mixer or effect control and bind it to a controller just by transmitting the MIDI message you want (say, by twisting a knob on your MIDI control box). The moment you exit MIDI Map Mode, your bindings go live. You can also map Session clips to a single MIDI key or to a whole keyboard range for chromatic performance.

Once MIDI keys and controllers are mapped to Live’s controls, they can no longer be used to record through MIDI tracks. Those messages get stripped out before the arriving MIDI reaches the MIDI tracks.

The Key/MIDI Map Controls.

Session clips, switches, buttons, and radio buttons can likewise be tied to keys on the computer keyboard. You do this in [Key Map Mode](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control), which operates exactly like MIDI Map Mode.

Beyond this all-purpose mapping approach, Live provides built-in support specifically for [Ableton Push 1](https://www.ableton.com/en/live-manual/12/using-push-1/#using-push-1), [Push 2](https://www.ableton.com/en/live-manual/12/using-push-2/#using-push-2), and [Push 3](https://www.ableton.com/push/manual/).
