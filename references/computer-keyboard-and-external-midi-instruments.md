# Computer Keyboard And External MIDI Instruments

Open when you need guidance on Computer Keyboard And External MIDI Instruments in Ableton Live.

Context: [External MIDI In/Out](routing-and-i-o.md#173-external-midi-inout).

<a id="source-1732-playing-midi-with-the-computer-keyboard"></a>
### 17.3.2 Playing MIDI With the Computer Keyboard

Your computer keyboard doubles as a way to produce MIDI notes from its keystrokes. Switch the computer MIDI keyboard on by clicking the Control Bar’s Computer MIDI Keyboard button, by ticking the “Computer MIDI Keyboard” entry in the Options menu, or by pressing the M shortcut.

Activating the Computer MIDI Keyboard.

Across the middle row of letter keys, you trigger notes that match a piano’s white keys, starting at the left end with the note C3. A piano’s black keys line up with the top row of computer keys instead. On the bottom row, the four leftmost letters (Z,X,C, and V on a U.S.-English keyboard) handle shifting the note range and dialing in velocity, in this way:

- The two leftmost keys (Z and X) move the keyboard’s octave range.
- The following pair (C and V) shift incoming note velocity in steps of twenty (20, 40, 60, and so on).

With the computer keyboard configured to deliver notes spanning C3 to C4, the key-to-MIDI-note layout places the middle row (ASDF…) onto the [Impulse percussion sampler’s](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#impulse) sample slots. As a result, you can perform and capture drum patterns straight off the computer keyboard.

Keep in mind that switching on the computer MIDI keyboard causes it to “steal“ keys that might otherwise be tied to [remote-control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#computer-keyboard-remote-control) parts of the Live interface. Avoid this by turning the computer MIDI keyboard off whenever you don’t need it. On top of that, single-letter shortcuts — for example S for soloing tracks — stay reachable while the Computer MIDI Keyboard is on if you tack on Shift, as in Shift+S.

<a id="source-1733-connecting-external-synthesizers"></a>
### 17.3.3 Connecting External Synthesizers

Sending MIDI to an outboard synthesizer is simple: aim the Output Type chooser at whichever MIDI port the synthesizer plugs into, then use the Output Channel chooser to pick the MIDI channel you transmit on.

Beyond routing through a track’s In/Out section, you can also route from inside a track’s device chain with the [External Instrument](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#external-instrument) device. Handled this way, the MIDI heads out to the outboard synthesizer and its audio comes back — the whole loop living in one track.

_Important_: Whenever a keyboard synthesizer serves both as a keyboard for playing into Live and as a sound generator, be sure to check the synthesizer’s “Local Off“ function. Present on every synthesizer, this function essentially cuts the keyboard apart from the sound generator, letting you handle the two parts as though they were independent devices. With that done, Live can act as the center of your MIDI studio: it takes in MIDI from the keyboard and forwards both that incoming MIDI and the MIDI from the clips wherever it belongs.

<a id="source-1734-midi-inout-indicators"></a>
### 17.3.4 MIDI In/Out Indicators

Within Live’s Control Bar sit three pairs of indicator LEDs reporting on MIDI as it arrives and departs. Beyond merely confirming that signals exist, these indicators also reveal how they are being used. For each pair, the top indicator blinks as a MIDI message comes in, while the bottom one blinks as a MIDI message goes out.

The Control Bar’s MIDI Indicators.

Reading the three indicator pairs from left to right, they stand for:

1. MIDI Clock and Timecode signals devoted to [synchronizing Live with other sequencers](https://www.ableton.com/en/live-manual/12/synchronizing-with-link-tempo-follower-and-midi/#synchronizing-with-link-tempo-follower-and-midi). Bear in mind this pair only appears once an external sync source has been turned on for a MIDI port within the Link, Tempo & MIDI Settings;
2. MIDI messages devoted to [remote-controlling](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) Live’s user-interface elements;
3. MIDI messages traveling to and from Live’s MIDI tracks.

Any MIDI messages assigned to remote-control Live’s user-interface elements get “eaten up“ by that remote control assignment, so they never reach the MIDI tracks. This trips people up often, yet a quick glance at the indicators clears it right up.
