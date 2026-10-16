# MIDI Port Track Sync Remote Settings

Open when you need guidance on MIDI Port Track Sync Remote Settings in Ableton Live.

Context: [MIDI Port Inputs and Outputs](routing-and-i-o.md#1731-midi-port-inputs-and-outputs).

<a id="source-17311-track"></a>
#### 17.3.1.1 Track

Switching on _Track_ lets Live transmit or accept note and CC (Control Change) messages — say, while you use a MIDI keyboard to perform or punch in pitches.

Turn on Track for a MIDI port’s input when:

- Performing instruments inside Live by way of a MIDI keyboard.
- Capturing notes into MIDI clips.
- Capturing MIDI CC messages into MIDI clips, for instance to log parameter moves from an outboard hardware synthesizer.

Turn on Track for a MIDI port’s output when:

- Driving an outboard hardware device (such as a synthesizer, drum machine, and so on).
- Pushing MIDI notes to a different application (over a virtual MIDI bus).
- Pushing MIDI CC automation out to an external device or application.

Note: Enabling Track on the output port of a MIDI controller is only necessary if that controller houses a built-in sound generator.

<a id="source-17312-sync"></a>
#### 17.3.1.2 Sync

_Sync_ lets Live transmit or accept MIDI Clock, as well as accept MIDI Timecode. Note: Short of having a built-in sequencer or arpeggiator, a MIDI controller never requires Sync to be turned on at either its input or its output ports.

Turn on Sync for a MIDI port’s input when:

- Locking Live to an outboard sequencer, drum machine or groove box.
- Locking Live to a different DAW via MIDI.

Turn on Sync for a MIDI port’s output when:

- Locking an outboard sequencer, drum machine or groove box to Live by way of MIDI Clock.
- Locking a different DAW to Live by way of MIDI Clock.
- Locking the LFO and arpeggiator of an outboard synthesizer or MIDI controller to Live.

Once Sync is turned on for a port’s output, an extra batch of options becomes reachable by clicking the triangle beside that port’s name.

Sync Output Options.

Tweaking the _MIDI Clock Sync Delay_ value lets you tack a delay, measured in milliseconds, onto the MIDI sync signals heading out. Doing so can iron out timing discrepancies that crop up between Live and the outboard hardware.

_MIDI Clock Type_ may be set to either Song to Pattern. Under Song Mode, Live transmits MIDI Song Position Pointer (SPP) and Continue messages whenever the play position shifts. Under Pattern Mode, Live restricts itself to Start messages, dispatched as the next bar begins. Reach for Pattern Mode whenever your MIDI device fails to understand SPP messages.

By way of the _Hardware Resync_ drop-down, you decide the manner in which a resync message goes out once the _Resync External Hardware_ option is turned on.

Resync External Hardware Option.

After it is turned on, the Resync External Hardware button shows up in Live’s Control bar, where it serves to push resync messages out toward external gear. That proves handy whenever synced hardware slips out of time with the Live Set as it plays.

The Resync External Hardware Button in the Control Bar.

By default the option sits at _Stop and Start_, whose resync message is a MIDI Clock Stop event trailed by a MIDI Clock Start event; this suits the majority of MIDI devices. Choose _Start Only_ and the resync message carries nothing but the MIDI Clock Start event, which a few devices may prefer. Choose _Don’t Resync_ and no resync messages go out at all.

<a id="source-17313-remote"></a>
#### 17.3.1.3 Remote

With the _Remote_ switch you can build mappings that link a MIDI controller to Live’s parameters, or route feedback back to a MIDI controller.

Turn on Remote for a MIDI port’s input when:

- Building your own MIDI mappings so you can drive parameters in Live.
- Relying on a MIDI keyboard to launch MIDI Clips.

Turn on Remote for a MIDI port’s output when:

- Working with MIDI controllers whose LEDs mirror the state of mapped Live parameters.
- Working with MIDI controllers whose motorized faders mirror the state of mapped Live parameters.
