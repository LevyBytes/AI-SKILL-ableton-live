# Track Audio And MIDI Concepts

Open when you need guidance on Track Audio And MIDI Concepts in Ableton Live.

Context: [Live Concepts](live-concepts.md#3-live-concepts).

<a id="source-37-tracks"></a>
### 3.7 Tracks

Clips live on tracks, which also govern how signals move and how fresh clips come into being through recording, sound synthesis, effects processing, and mixing.

A Track in the Arrangement View.

One common pool of tracks is shared by the Session and the Arrangement. Within the Session View, tracks line up as columns, whereas within the Arrangement View they stack one above another, with time running from the left toward the right.

Only a single clip plays on a track at any given moment. That's why clips meant to play as alternatives usually go in one Session View column, while clips meant to sound together get spread across tracks into rows, which we term [scenes](https://www.ableton.com/en/live-manual/12/session-view/#tracks-and-scenes).

A Scene in the Session View.

A track at any given moment plays either a Session clip or an Arrangement clip, yet never the two together. Priority goes to Session clips. Firing a Session clip halts whatever is currently sounding so the freshly launched clip can play. Specifically, an Arrangement clip playing on that track will cease so the Session clip can sound instead — meanwhile the remaining tracks carry on playing their Arrangement clips. On the track where you fired the Session clip, the Arrangement clips stay silent until you restart them by hand with the _Back to Arrangement_ button.

You'll find the Back to Arrangement button on the _Main track_ within the Session View, plus at the upper right of the scrub area within the Arrangement View. Its lit state signals that one or more tracks are at that moment _not_ following the Arrangement, but are instead sounding a clip out of the Session.

Session View's Back to Arrangement Button.Arrangement View's Back to Arrangement Button.

Pressing this button returns every track to playing the Arrangement. Within the Arrangement View, each track carries its own Back to Arrangement button too, so you can bring just some tracks back to Arrangement playback.

A Single Track's Back to Arrangement Button.

There's also the option of committing the present Session state into the Arrangement, done by switching on the _Arrangement Record_ button from within the Session View.

The Arrangement Record Button.

By recording into the Arrangement tracks, you can cut several [takes](https://www.ableton.com/en/live-manual/12/comping/#recording-takes) of a clip and afterward assemble them into a single [composite track](https://www.ableton.com/en/live-manual/12/comping/#comping).

Tracks can also be [linked](https://www.ableton.com/en/live-manual/12/arrangement-view/#linked-track-editing) so that one action applies across several tracks together.

Creating a Fade in Two Linked Tracks.

<a id="source-38-audio-and-midi"></a>
### 3.8 Audio and MIDI

Two kinds of signal occupy Live: audio and MIDI. Digitally speaking, an audio signal amounts to a string of numbers standing in for a smooth waveform. That signal might come from any number of places — a microphone's audio, a sound built or sampled in software, or a feed sent out to a loudspeaker. A MIDI signal, by contrast, is a string of commands, along the lines of "now play a C4 at mezzo piano." MIDI stands as a symbolic depiction of musical content, nearer to notation on paper than to a recorded sound. Hardware input gear such as MIDI or USB keyboards, or software devices, produce MIDI signals.

Turning MIDI signals into audio signals you can actually hear takes an [instrument](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects). Certain instruments, Live's [Simpler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#simpler) among them, exist for chromatic performance of a single sound across the keyboard. Others, such as Live's [Impulse](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#impulse), place a separate percussion sound under each key.

Capturing and playing audio signals is the job of _audio tracks_, while capturing and playing MIDI signals is the job of _MIDI tracks_. A matching clip type belongs to each of the two track types. You cannot put audio clips onto MIDI tracks, nor the reverse.

Details on adding, rearranging, and removing audio and MIDI tracks appear in the [Audio and MIDI Tracks](https://www.ableton.com/en/live-manual/12/mixing/#audio-and-midi-tracks) section of the Mixing chapter.

<a id="source-39-audio-clips-and-samples"></a>
### 3.9 Audio Clips and Samples

Inside an audio clip is a pointer to a _sample_ (which you might also call a "sound file" or "audio file") or to a _compressed sample_ (an MP3 file, say). That clip records where on your drives the sample sits, which portion of the sample should play, and _how_ it ought to play.

Drag a sample in from Live's built-in browser and Live builds a clip on its own to sound that sample. Before you drag a sample in, you can audition or _preview_ it right inside the browser. With the Browser File Preview button bearing the headphones icon switched on, the preview begins on its own the instant you pick a sample.

A Selected Sample with Audio Preview in the Browser.

Live gives you a wealth of ways to play samples in fresh and surprising fashions, so you can conjure a wide array of new sounds while the original sample stays untouched — every alteration is figured in real time as the sample sounds. You'll find those settings in the [_Clip View_](https://www.ableton.com/en/live-manual/12/live-concepts/#clip-and-device-view), which appears once you double-click a clip.

An Audio Clip's Properties as Displayed in the Clip View.

A great deal of this power flows from Live's [warping capabilities](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping). To warp is to alter how fast a sample plays apart from its pitch, in order to fit the song tempo. You can shift the tempo on the fly using the Control Bar's Tempo field.

The Control Bar's Tempo Field.

The simplest application of this approach, which generally needs no hand-tuning at all, is locking sample loops to whatever tempo you've picked. Indeed, Live's Auto-Warp algorithm makes it straightforward to align _any_ sample with the song tempo, even a recording of some drunken jazz band's playing. Pushing the warp settings to extremes can also reshape a sound's sonic character drastically.

<a id="source-310-midi-clips-and-midi-files"></a>
### 3.10 MIDI Clips and MIDI Files

Within a MIDI clip lives musical content expressed as MIDI notes and controller envelopes. Bring MIDI in from a [MIDI file](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#midi-files) and that data folds into the Live Set, with the source file no longer referenced from then on. Inside Live's browser, a MIDI file shows up with a distinct icon and the .mid file extension.

A MIDI File in the Browser.

What a MIDI clip holds can be [accessed and edited](https://www.ableton.com/en/live-manual/12/editing-midi/#editing-midi) through the Clip View — to reshape a melody or build a drum groove, for example.

A MIDI Clip's Properties as Displayed in the Clip View.

Beyond capturing MIDI signals arriving from outside gear, Live also lets you place MIDI notes into clips with [Draw Mode](https://www.ableton.com/en/live-manual/12/editing-midi/#draw-mode), [MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#midi-tools), or [audio-to-MIDI converters](https://www.ableton.com/en/live-manual/12/converting-audio-to-midi/#converting-audio-to-midi).
