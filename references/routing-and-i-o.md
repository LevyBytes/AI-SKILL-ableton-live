# Routing And I O (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 17. Routing and I/O

Within Live, the word “routing“ refers to how each track’s signal sources and destinations — that is, its inputs and outputs — get configured. The bulk of this configuration takes place in the mixer’s _track In/Out section_, where each track presents choosers for picking a source and a destination. Think of the mixer’s In/Out section as Live’s “patchbay.“

The Mixer’s In/Out Section.

From both Session and Arrangement View you can reveal or conceal the mixer’s I/O section: pick the In/Out entry within the mixer’s view control menu down in Live’s lower-right corner, or choose the In/Out option under the View menu’s Mixer Controls submenu, or press the shortcut CtrlAltI (Win) / CtrlOptionI (Mac).

The Mixer View Control’s Options Menu.

Any track capable of playing clips shares this identical In/Out layout:

- The top chooser pair (“Audio/MIDI From“) defines what feeds the track. An audio track takes an audio input, while a MIDI track takes a MIDI input. A Return track draws its feed from the [respective sends](https://www.ableton.com/en/live-manual/12/mixing/#return-tracks-and-the-main-track).
- The Monitor radio button sets the monitor mode — namely, the circumstances in which you hear the track’s input passing through it.
- The bottom chooser pair (“Audio/MIDI To“) defines where the track sends its signal. Every track produces audio output, with the lone exception of a MIDI track lacking an instrument. Keep in mind that [instruments convert MIDI to audio](https://www.ableton.com/en/live-manual/12/live-concepts/#audio-and-midi).

Inside a chooser pair, the top one — known as the Input/Output Type chooser — picks the signal category (for example “Ext.,“ which covers external hookups through an audio or MIDI interface). Should that signal type carry sub-selections or channels, you reach them from the bottom chooser, the Input/Output Channel chooser. Sticking with the “Ext.“ case, those would be the separate audio/MIDI inputs and outputs.

### 17.1 Monitoring

Inside Live, “Monitoring“ describes the act of routing a track’s incoming signal through to that track’s output. Imagine you have configured an audio track so its input arrives from a guitar. In that case, monitoring means the sound of your live guitar performance genuinely makes it to the track’s output by way of the track’s device chain. With the track’s output assigned to “Main,“ that guitar signal — shaped by whichever effects are in play (and pushed back by however much latency the audio hardware interface adds) — comes out of your speakers.

On each audio track and MIDI track, the In/Out section supplies a _Monitor_ radio button presenting these three choices:

-

For the majority of simple recording situations, the default _Auto_-monitoring setting behaves sensibly: it switches monitoring on while the track is [armed](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips), yet holds monitoring back whenever the track happens to be playing clips.

-

Selecting _In_ keeps the track’s input monitored at all times, no matter whether the track is armed or its clips are playing. In practice this makes the track behave like what certain systems label an “Aux“: rather than serving for recording, it brings a signal in from somewhere else. Under this choice, any output from the clips gets muted. You can spot an “In“ monitoring choice at a glance — even with the In/Out section collapsed — thanks to the blue color of the track’s Activator switch.

-

Picking the _Off_ option disables monitoring entirely. That comes in handy while recording acoustic instruments heard “through the air,“ while relying on an outboard mixing console to monitor, or while using an audio hardware interface whose “direct monitoring“ feature skips the computer to sidestep latency. As a rule, an audio interface capable of nearly imperceptible latencies (a few milliseconds) is the better choice. Should you record into Live with monitoring set to “Off,“ consider applying the Audio Settings’ Overall Latency adjustment, covered in the built-in program tutorial about configuring the Audio Settings.

With monitoring set to either “In” or “Auto,” the “Keep Monitoring Latency in Recorded Audio” option is on by default. It shifts the recording’s timing so it lines up with what you hear through Live’s monitoring. The usual advice is to keep this option on while recording software instruments or effects, and to turn it off while recording acoustic instruments or leaning on external monitoring. A right-click on the “In” or “Auto” monitor buttons lets you toggle “Keep Monitoring Latency in Record Audio” on or off by hand.

When several tracks are highlighted, clicking one of the Monitor buttons pushes that choice out to every selected track.

You can likewise bring the Monitor buttons back to how they began. While the In/Out section is open, press the Delete key, which restores each Monitor button to its default — that being “Off” on audio tracks and “Auto” on MIDI tracks — or instead choose the Edit menu option “Return to Default.”

### 17.2 External Audio In/Out

To pick the inputs of an audio interface, choose “Ext. In“ in an audio track’s Input Type chooser. From there, the Input Channel chooser presents the separate input channels. Each entry in that chooser carries a meter beside its label, which helps you spot whether a signal is present and whether it overloads (the meter turns red at that point). Configuring the audio interface’s outputs follows the same pattern through the output chooser pair. With several tracks highlighted, whatever edits you make in these choosers reach all of the selected tracks.

Which inputs and outputs show up is governed by the Audio Settings, reachable through the “Configure…“ option in the Input and Output Channel choosers. Bear in mind that the Audio Settings additionally open the Channel Configuration dialogs, which set which inputs and outputs are active and whether Live treats them as mono or as stereo pairs. In short, the Channel Configuration dialog supplies Live with the details it requires about how your computer hooks up to the rest of the audio gear in your studio.

Any input and output channels listed in the Channel Configuration dialogs may be renamed. Once you do, the revised name appears in the matching Input / Output Channel chooser drop-down. Renaming goes faster if you jump from one channel to the next with the Tab key. Keep in mind that a changed name stays tied to its particular audio device.

### 17.2.1 Mono/Stereo Conversions

Select a mono signal as the input of an audio track and the track captures mono samples; pick anything else and it captures stereo samples. Regardless, the signals flowing through the track’s device chain remain stereo, whether the track’s input is mono or the track is playing mono samples.

Conversion from mono to stereo is nothing more than feeding the same signal to both the left and right channels. Conversely, when a track feeds a mono output, the left and right signals get summed and then trimmed by 6 dB to keep clipping at bay.

### 17.3 External MIDI In/Out

External MIDI reaches Live by the same means as audio does. In a MIDI track’s Input Type chooser, you may pick a particular MIDI input port or choose “All Ins,“ the combined feed of every external MIDI port. The Input Channel chooser then lists the separate input channels of whichever MIDI port you selected, along with “All Channels,“ the merged signal across them all. Just like audio inputs, the Input Channel chooser places a meter alongside each entry to indicate activity on that input channel. Should several MIDI tracks be highlighted, any edits in these choosers carry over to all selected tracks.

### 17.3.1 MIDI Port Inputs and Outputs

Deciding which MIDI ports Live can reach is handled through the _Inputs_ and _Outputs_ options found in the MIDI section of the Link, Tempo & MIDI Settings. Every available input and output port shows up there. There is no limit on how many MIDI ports you employ for track input and output; the mixer’s In/Out choosers let each one be targeted on its own.

The MIDI Port Inputs and Outputs List in the Settings.

#### 17.3.1.1 Track

Switching on _Track_ lets Live transmit or accept note and CC (Control Change) messages — say, while you use a MIDI keyboard to perform or punch in pitches.

Turn on Track for a MIDI port’s input when: - Performing instruments inside Live by way of a MIDI keyboard. - Capturing notes into MIDI clips. - Capturing MIDI CC messages into MIDI clips, for instance to log parameter moves from an outboard hardware synthesizer.

Turn on Track for a MIDI port’s output when: - Driving an outboard hardware device (such as a synthesizer, drum machine, and so on). - Pushing MIDI notes to a different application (over a virtual MIDI bus). - Pushing MIDI CC automation out to an external device or application.

Note: Enabling Track on the output port of a MIDI controller is only necessary if that controller houses a built-in sound generator.

#### 17.3.1.2 Sync

_Sync_ lets Live transmit or accept MIDI Clock, as well as accept MIDI Timecode. Note: Short of having a built-in sequencer or arpeggiator, a MIDI controller never requires Sync to be turned on at either its input or its output ports.

Turn on Sync for a MIDI port’s input when: - Locking Live to an outboard sequencer, drum machine or groove box. - Locking Live to a different DAW via MIDI.

Turn on Sync for a MIDI port’s output when: - Locking an outboard sequencer, drum machine or groove box to Live by way of MIDI Clock. - Locking a different DAW to Live by way of MIDI Clock. - Locking the LFO and arpeggiator of an outboard synthesizer or MIDI controller to Live.

Once Sync is turned on for a port’s output, an extra batch of options becomes reachable by clicking the triangle beside that port’s name.

Sync Output Options.

Tweaking the _MIDI Clock Sync Delay_ value lets you tack a delay, measured in milliseconds, onto the MIDI sync signals heading out. Doing so can iron out timing discrepancies that crop up between Live and the outboard hardware.

_MIDI Clock Type_ may be set to either Song to Pattern. Under Song Mode, Live transmits MIDI Song Position Pointer (SPP) and Continue messages whenever the play position shifts. Under Pattern Mode, Live restricts itself to Start messages, dispatched as the next bar begins. Reach for Pattern Mode whenever your MIDI device fails to understand SPP messages.

By way of the _Hardware Resync_ drop-down, you decide the manner in which a resync message goes out once the _Resync External Hardware_ option is turned on.

Resync External Hardware Option.

After it is turned on, the Resync External Hardware button shows up in Live’s Control bar, where it serves to push resync messages out toward external gear. That proves handy whenever synced hardware slips out of time with the Live Set as it plays.

The Resync External Hardware Button in the Control Bar.

By default the option sits at _Stop and Start_, whose resync message is a MIDI Clock Stop event trailed by a MIDI Clock Start event; this suits the majority of MIDI devices. Choose _Start Only_ and the resync message carries nothing but the MIDI Clock Start event, which a few devices may prefer. Choose _Don’t Resync_ and no resync messages go out at all.

#### 17.3.1.3 Remote

With the _Remote_ switch you can build mappings that link a MIDI controller to Live’s parameters, or route feedback back to a MIDI controller.

Turn on Remote for a MIDI port’s input when: - Building your own MIDI mappings so you can drive parameters in Live. - Relying on a MIDI keyboard to launch MIDI Clips.

Turn on Remote for a MIDI port’s output when: - Working with MIDI controllers whose LEDs mirror the state of mapped Live parameters. - Working with MIDI controllers whose motorized faders mirror the state of mapped Live parameters.

### 17.3.2 Playing MIDI With the Computer Keyboard

Your computer keyboard doubles as a way to produce MIDI notes from its keystrokes. Switch the computer MIDI keyboard on by clicking the Control Bar’s Computer MIDI Keyboard button, by ticking the “Computer MIDI Keyboard” entry in the Options menu, or by pressing the M shortcut.

Activating the Computer MIDI Keyboard.

Across the middle row of letter keys, you trigger notes that match a piano’s white keys, starting at the left end with the note C3. A piano’s black keys line up with the top row of computer keys instead. On the bottom row, the four leftmost letters (Z,X,C, and V on a U.S.-English keyboard) handle shifting the note range and dialing in velocity, in this way:

- The two leftmost keys (Z and X) move the keyboard’s octave range.
- The following pair (C and V) shift incoming note velocity in steps of twenty (20, 40, 60, and so on).

With the computer keyboard configured to deliver notes spanning C3 to C4, the key-to-MIDI-note layout places the middle row (ASDF…) onto the [Impulse percussion sampler’s](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#impulse) sample slots. As a result, you can perform and capture drum patterns straight off the computer keyboard.

Keep in mind that switching on the computer MIDI keyboard causes it to “steal“ keys that might otherwise be tied to [remote-control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control) parts of the Live interface. Avoid this by turning the computer MIDI keyboard off whenever you don’t need it. On top of that, single-letter shortcuts — for example S for soloing tracks — stay reachable while the Computer MIDI Keyboard is on if you tack on Shift, as in ShiftS.

### 17.3.3 Connecting External Synthesizers

Sending MIDI to an outboard synthesizer is simple: aim the Output Type chooser at whichever MIDI port the synthesizer plugs into, then use the Output Channel chooser to pick the MIDI channel you transmit on.

Beyond routing through a track’s In/Out section, you can also route from inside a track’s device chain with the [External Instrument](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#external-instrument) device. Handled this way, the MIDI heads out to the outboard synthesizer and its audio comes back — the whole loop living in one track.

_Important_: Whenever a keyboard synthesizer serves both as a keyboard for playing into Live and as a sound generator, be sure to check the synthesizer’s “Local Off“ function. Present on every synthesizer, this function essentially cuts the keyboard apart from the sound generator, letting you handle the two parts as though they were independent devices. With that done, Live can act as the center of your MIDI studio: it takes in MIDI from the keyboard and forwards both that incoming MIDI and the MIDI from the clips wherever it belongs.

### 17.3.4 MIDI In/Out Indicators

Within Live’s Control Bar sit three pairs of indicator LEDs reporting on MIDI as it arrives and departs. Beyond merely confirming that signals exist, these indicators also reveal how they are being used. For each pair, the top indicator blinks as a MIDI message comes in, while the bottom one blinks as a MIDI message goes out.

The Control Bar’s MIDI Indicators.

Reading the three indicator pairs from left to right, they stand for:

1. MIDI Clock and Timecode signals devoted to [synchronizing Live with other sequencers](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-with-link-tempo-follower-and-midi). Bear in mind this pair only appears once an external sync source has been turned on for a MIDI port within the Link, Tempo & MIDI Settings;
2. MIDI messages devoted to [remote-controlling](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) Live’s user-interface elements;
3. MIDI messages traveling to and from Live’s MIDI tracks.

Any MIDI messages assigned to remote-control Live’s user-interface elements get “eaten up“ by that remote control assignment, so they never reach the MIDI tracks. This trips people up often, yet a quick glance at the indicators clears it right up.

### 17.4 Resampling

You can feed Live’s Main output into a single audio track and record it — in other words, resample it. Resampling makes for an enjoyable and handy technique, since it turns whatever is happening right now in a Live Set into samples you can fold back in straight away. It serves for capturing tracks loaded with CPU-hungry devices so those devices can be removed afterward, or for a fast preview ahead of [rendering to disk](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video).

Selecting the “Resampling“ option in any audio track’s Input Type chooser steers the Main output onto that track. From there you settle on precisely what to resample, muting, soloing, or otherwise tweaking the tracks that feed the Main output. It is wise to watch the Main Volume meter so your level stays as hot as it can without clipping (shown by red in the meter). After that, arm the track and record into one of its [empty clip slots](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-into-session-slots). Bear in mind that the recording track’s own output stays muted throughout resampling and is left out of the recording.

Whatever samples resampling produces land inside the current Set’s [Project folder](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#live-projects), within Samples/Recorded. As long as the Set stays unsaved, they sit instead at the spot named by the [Temporary Folder](https://www.ableton.com/en/live-manual/12/recording-new-clips/#where-are-the-recorded-samples).

### 17.5 Internal Routings

Both Live’s mixer and its external routing devices make inter-track routings possible. While such routings can be a bit bewildering, they unlock a wealth of useful creative and technical possibilities. Through the mixer, inter-track routing happens in two ways:

1. Track A is configured to push its output signal over to Track B. That works because any track able to accept an output signal of the right type from Track A turns up in its Output Type chooser.
2. Track B is configured to pull its input signal from Track A. That works because any track furnishing a signal of the right type shows up in Track B’s Input Type chooser.
   Two Ways to Route Track A into Track B.

Either route ends with Track A’s output flowing into Track B. Approach 1 keeps Track B’s in/out settings untouched and, whenever we like, lets us bring in further tracks that send their output into Track B. It is the go-to technique for “many-to-one“ routings — submixes, say, or a handful of MIDI tracks driving the same instrument. Here, soloing Track B still lets you hear the output of every track feeding it. You can equally solo Track A and hear its output signal. When you do, all the other tracks fall silent, even the ones that may also feed Track B. Strictly speaking, what reaches your ears is Track B’s output stripped of everything but Track A’s signal.

Approach 2, by contrast, leaves Track A untouched apart from Track B tapping its output. Adding more tracks akin to Track B, each tapping Track A’s output, is just as easy. Layering instruments is a fine illustration of this kind of “one-to-many“ routing arrangement.

### 17.5.1 Internal Routing Points

A signal leaves each of Live’s tracks, moves through that track’s device chain, and arrives at the track mixer, where the tracks’ faders may pan it or change its level.

Anytime a track’s Audio From input chooser points at another track (the previous section’s Approach 2), you can tap the incoming signal at one of three spots picked in the Input Channel chooser: _Pre FX, Post FX_ or _Post Mixer_.

Tap Points for Track Routing.

- _Pre FX_ grabs the signal straight off a track before it has reached the track’s device chains (FX) or mixer. Because of that, edits to the tapped track’s devices or mixer leave the tapped signal unchanged. Soloing a track that taps another one Pre FX lets you hear that tapped track.
- _Post FX_ grabs the signal at the end of a track’s device chains (FX) but ahead of its return to the track mixer. Consequently, edits to the tapped track’s devices reshape the tapped signal, whereas edits to its mixer settings do not. Soloing a track that taps another one Post FX lets you hear that tapped track.
- _Post Mixer_ grabs a track’s final output once it has run through its device chains and mixer. Soloing a track that taps another one Post Mixer does _not_ let you hear that tapped track.

#### 17.5.1.1 Routing Points in Racks

Tap Points for Every Chain in a Track.

Should a track hold one or more [Instrument or Effect Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks) in its device chain, the internal routing points (Pre FX, Post FX and Post Mixer) become available for each chain inside the Rack as well. Should a track hold one or more [Drum Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#drum-racks), the internal routing points open up for any of the Rack’s return chains. Every Rack likewise turns up in the Input Channel chooser:

- _(Rack Name) | (Chain Name)_ | Pre FX — Taps the signal where it first enters the Rack, ahead of the chain’s devices.
- _(Rack Name) | (Chain Name)_ | Post FX — Taps the signal at the chain’s end, ahead of the chain’s mixer.
- _(Rack Name) | (Chain Name)_ | Post Mixer — Taps the signal from the chain mixer’s output, right before all of the Rack’s chains get summed into the Rack’s output.

Soloing a track that taps a Chain at any one of these spots still lets you hear the output there.

### 17.5.2 Making Use of Internal Routing

A handful of internal routing examples are walked through more thoroughly in this section.

#### 17.5.2.1 Post-Effects Recording

Picture yourself sending a guitar into Live, assembling a song one track at a time, stacking take upon take. Granted, keeping a distinct effects chain on each track — so you can apply different effects to different takes after the fact — is powerful. Even so, you may prefer to pass the guitar signal through effects (a noise gate or an amp model, perhaps) _before_ it ever gets recorded, then capture the post-effects signal.

An Example Setup for Post-Effects Recording.

Pulling this off is simple: set aside a dedicated audio track that processes and monitors the arriving guitar signal. We name that track “Guitar“ and drop the effects we want into its device chain. Rather than record straight into the Guitar track, we spin up a couple of extra tracks for recording. Each of those is configured to take its input Post FX from the Guitar track. Note that tapping the Guitar track Post Mixer would be an option too, should we want to capture any of its level or panning.

On the monitoring side, the Guitar track’s Monitor radio button goes to In, since we always want our guitar audible through this track regardless of whatever else Live is doing. The remaining tracks’ Monitor radio buttons go to Off.

#### 17.5.2.2 Recording MIDI as Audio

While dealing with MIDI alongside elaborate software instruments, capturing the audio that results can sometimes beat capturing the MIDI going in. One lone MIDI note might, for instance, drive Native Instruments’ _Absynth_ to generate something closer to a passage of music than to a single tone. Such output suits depiction as an audio waveform far better than a solitary note in a MIDI clip, all the more so once you weigh the editing options.

Recording the Output of a Complex Instrument in Audio Tracks.

An arrangement much like the one [described above](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#post-effects-recording) gets the job done. A single MIDI track holds the virtual instrument, and one more audio track captures the audio output while the instrument plays.
