# Tuning System Loading And Track Options

Open when you need guidance on Tuning System Loading And Track Options in Ableton Live.

Context: [Using Tuning Systems](grooves-and-tuning-routes.md#15-using-tuning-systems).

<a id="source-151-loading-a-tuning-system"></a>
### 15.1 Loading a Tuning System

Bringing a tuning system into a Set is done by double-clicking a tuning file in the browser, or by highlighting the file and hitting Enter. Either approach opens the browser's Tuning section by itself, since that section stays hidden until then.

The Tuning section in the Browser.

The browser’s view control menu offers another way to reveal the Tuning section.

The Browser View Control Menu.

You may likewise drag ASCL or SCL files stored elsewhere on your computer and drop them into the Tuning section. Provided the file is present in the [Tuning section](https://www.ableton.com/en/live-manual/12/using-tuning-systems/#the-tuning-section), its tuning gets stored alongside the Live Set.

After a tuning system joins a Live Set, the piano roll notes stop standing for ordinary MIDI notes and instead display the matching notes of the tuning.

Updated Notes in the MIDI Note Editor.

Hovering over a piano roll note surfaces helpful details in the Status Bar, including that note’s pitch and frequency. The stated pitch sounds whenever a note is triggered from the piano roll or through a keyboard.

Hover Over a Note in the Piano Roll for Pitch Information.

Normally, when you drop a tuning system or swap it for another, the existing notes hold their spots in the piano roll while the note ruler's pitches refresh to fit the new tuning. As a result, those original notes might no longer sound the same pitch.

Switch on the “Retune Set On Loading Tuning Systems” item in the Options menu, and loading or swapping a tuning system makes the notes hew tightly to the pitches of the originals, so a melody stays as faithful to the source as it can be. A dialog pops up to confirm the operation as you load a tuning system.

Existing MIDI Clips May Be Modified when Loading a Tuning System.

With automatic note retuning turned on, taking out a tuning system or moving between them can alter or wipe out original notes. The situation arises when a pair of notes that overlap in time and started on different pitches both end up assigned to a single pitch in the new tuning system, that pitch being the nearest match to each of them. Should that occur, one of the two notes might be trimmed or removed.

Bear in mind that once a tuning system is loaded the Scale Mode choosers in Clip View and the Control Bar disappear, while every [scale aware](https://www.ableton.com/en/live-manual/12/live-concepts/#scale-awareness) device has its Use Current Scale toggle switched off.

<a id="source-152-the-tuning-section"></a>
### 15.2 The Tuning Section

A range of pitch settings belonging to a tuning system can be reached through the Tuning section.

The Tuning Section Expanded.

Click the triangle beside the tuning file's name to open the section up and get at extra settings governing the lowest and highest notes for the reference pitch.

- _Tuning_ shows the tuning system's name.
- _Octave_ picks the octave of the note serving as the reference pitch.
- _Note_ picks the note within that octave serving as the reference pitch.
- _Ref. Pitch/Freq_ fixes the reference pitch's frequency. Shifting this frequency raises or lowers the pitch of every note in the Set.
- _Lowest Note_ defines what the lowest note sounds by tying it to an octave and pitch class. Adjusting the lowest note moves the highest note too, keeping the same count of notes between them.
- _Highest Note_ defines what the highest note sounds; altering the highest note likewise revises the lowest note.

Bear in mind that only the Ref. Pitch/Freq value alters the reference pitch in a way you can hear. Editing the Octave or Note values does refresh the frequency shown in the Ref. Pitch/Freq slider to fit the newly chosen notes, yet nothing audible shifts until you change the reference pitch frequency value itself. The point is to head off any abrupt pitch jumps while you set the Octave or Note values.

Use the floppy disk button just right of the reference pitch frequency to store the tuning that's loaded as an .ascl file under the browser's Tunings label.

Click the arrow button beside the Save Tuning System button to follow a link to [Ableton’s Tuning website](https://tuning.ableton.com/), which holds further details on the loaded tuning system plus an interactive editor for experimenting with variants of its pitches. Any custom tuning systems you build there can be exported as well. Keep in mind that not every tuning system has an external page, and the arrow button is greyed out when no matching link exists.

Highlight a file inside the Tuning section and hit the Delete key to clear it and revert to 12TET tuning.

<a id="source-153-midi-track-options-for-tuning-systems"></a>
### 15.3 MIDI Track Options for Tuning Systems

Loading a tuning system brings a handful of tuning-specific options into the I/O section of MIDI tracks, giving you ways to tailor your track and controller arrangements.
