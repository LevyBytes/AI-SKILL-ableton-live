# Audio To MIDI Conversion Quality

Open when you need guidance on Audio To MIDI Conversion Quality in Ableton Live.

Context: [Converting Audio to MIDI](mpe-and-audio-midi-routes.md#13-converting-audio-to-midi).

<a id="source-132-convert-harmony-to-new-midi-track"></a>
### 13.2 Convert Harmony to New MIDI Track

This command detects the pitches within a polyphonic audio recording and deposits them into a clip on a new MIDI track. That track arrives preloaded with an [Instrument Rack](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks) producing a piano sound (which you're free to swap for a different instrument if you prefer).

Bear in mind that this command, like the rest of the Convert commands, parts ways with slicing because the resulting MIDI clip doesn't reproduce the original _sound_; rather it pulls out the _notes_ and uses them to drive a completely different sound.

The Convert Harmony command handles music from your library, but you can equally land strong results by generating MIDI from your own recordings of harmonic instruments like guitar or piano.

<a id="source-133-convert-melody-to-new-midi-track"></a>
### 13.3 Convert Melody to New MIDI Track

This command detects the pitches in monophonic audio and drops them into a clip on a new MIDI track.

That track ships preloaded with an Instrument Rack that plays a synthesizer sound. With the Rack’s “Synth to Piano” Macro Control, you can morph this sound's timbre somewhere between an analog-style synth and an electric piano. The instrument was built to be flexible enough for a solid preview, yet you can naturally swap it for another instrument if you wish.

The Melody to MIDI Instrument Rack.

The Convert Melody command handles music from your library, and it also lets you record yourself singing, whistling, or playing a solo instrument like a guitar, then turn that recording into MIDI notes.

<a id="source-134-convert-drums-to-new-midi-track"></a>
### 13.4 Convert Drums to New MIDI Track

This command pulls the rhythms out of unpitched, percussive audio and sets them into a clip on a new MIDI track. It also tries to recognize kick, snare and hihat sounds, placing them into the new clip so they trigger the right sounds in the preloaded Drum Rack.

Just as with the Convert Melody command, you can tweak the transient markers in the audio clip before converting to steer where notes land in the converted MIDI clip.

Convert Drums performs nicely on recorded breakbeats, and equally on your own recordings like beatboxing or tapping a surface.

<a id="source-135-optimizing-for-better-conversion-quality"></a>
### 13.5 Optimizing for Better Conversion Quality

The Convert commands can yield compelling results on existing recordings from your library, and just as well on material you've recorded yourself. As an example, you might record yourself singing, playing guitar, or even beatboxing, then use the Convert commands to make MIDI that serves as a springboard for new music.

To get the most precise results, here's what we suggest:

- Pick music with crisp attacks. Notes that fade in or “swell” might slip past the conversion process undetected.
- Stick to recordings of single, isolated instruments. The Convert Drums command, for one, does best on solo drum breaks; if other instruments are in the mix, their notes get picked up as well.
- Reach for uncompressed, high-quality audio files like .wav or .aiff. Lossy data formats like mp3 can lead to erratic conversions, unless those recordings sit at high bitrates.

To work out where one note ends and the next begins in the converted MIDI clip, Live reads the [transient markers](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#transients-and-pseudo-warp-markers) in the source audio clip. That lets you “tune” the conversion's outcome by adding, shifting, or removing transient markers in the audio clip ahead of running any Convert command.

Even though each command targets a specific kind of musical material, the “wrong” command can occasionally hand you very intriguing results. Take Convert Harmony, which typically builds chords. Running it across a monophonic clip (a vocal recording, say) will frequently produce notes that the original audio never held. That can be a fine way to kick-start your creativity.
