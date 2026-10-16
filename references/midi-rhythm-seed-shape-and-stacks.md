# MIDI Rhythm Seed Shape And Stacks

Open when you need guidance on MIDI Rhythm Seed Shape And Stacks in Ableton Live.

Context: [Generative Tools](midi-generation-and-velocity-routes.md#113-generative-tools).

<a id="source-1131-rhythm"></a>
### 11.3.1 Rhythm

Driven by its parameters, the Rhythm MIDI Tool builds a note pattern and loops it across whatever time selection you provide.

The Rhythm Generator.

You can target a single pitch when generating notes, or an individual drum pad if you are working inside Drum Racks. Pick that pitch or pad through the Pitch control, or alternatively hold Alt (Win) / Option (Mac) and click on the piano ruler.

The Steps control sets how many steps make up the pattern, with a ceiling of 16 steps.

Where the generated notes land — that is, the pattern's shape — is governed by the Pattern knob. How many patterns you can choose from is tied to the current Steps and Density settings.

How many notes a pattern holds is set by the Density knob. Keep in mind that its ceiling follows whatever you entered with the Steps control.

With the Step Duration slider you control how often the pattern recurs inside the time selection. Take a one-bar time selection as an example: at a Step Duration of 1/8 with Steps at 8, the pattern plays through a single time. Switch Step Duration to 1/16 under the same conditions and it plays through twice. Bear in mind that Step Duration also constrains the highest Steps value you can dial in.

A probability that any given step in the pattern gets split in two is set through the Split control.

When given positive values, Shift nudges the generated notes rightward by a chosen number of steps; negative values push them leftward instead.

Velocities for the generated notes — along with a separate velocity reserved for accented ones — are dialed in with the Velocity and Accent sliders. How many accents land in the pattern is governed by the Accent Frequency parameter, which counts the notes that sit between one accent and the next. Its range runs from 0 up to however many notes the Density parameter specifies. Bear in mind that an accent itself counts as one of those note occurrences — so at an Accent Frequency of 1, each note ends up accented. The placement of accents within the pattern can be nudged using the Accent Offset arrows.

If you want to build the rhythmic pattern up further, clear the selection of notes you already made and tweak Rhythm’s parameters once more for another pitch or drum pad.

A Rhythmic Pattern Generated in a Drum Track.

<a id="source-1132-seed"></a>
### 11.3.2 Seed

Within pitch, length, and velocity boundaries you define, the Seed MIDI Tool produces notes at random. Further parameters let you state how many notes may sound together, plus the total count of notes that get produced.

The Seed Generator.

Set the pitch span for newly produced notes by dragging the Minimum and Maximum Pitch or Key Track sliders, or by moving the triangular handles within the Pitch Range slider. Should you drag one handle so far that it overlaps the other, the two fuse together, and from then on notes appear at just a single pitch. Splitting them back into two handles is done by clicking somewhere in the Pitch Range slider or by entering distinct values in the Minimum and Maximum Pitch or Key Track sliders. Another route is to hold Alt (Win) / Option (Mac) and click the piano ruler to pin one pitch for note generation, or to click and drag there to mark out a span of pitches. Keep in mind that an active clip scale tints the slider purple; without one, it matches the coloring of the remaining two sliders.

Just like the Pitch Range slider, the Duration and Velocity Range sliders define the length and velocity boundaries for the notes produced. The shortest note the duration range accepts is a 1/128 note and the longest is a single note. Velocity spans 1 to 127.

How many notes get added is also yours to govern through the Voices and Density controls: Voices caps how many notes can sound at once, while Density sets the total number produced, expressed as a percentage of the pitch range you want filled.

Notes Added Using Seed.

<a id="source-1133-shape"></a>
### 11.3.3 Shape

As a MIDI Tool, Shape produces a run of notes inside a chosen pitch span. Those notes are laid out to trace a shape you set up in the MIDI Tool’s display.

The Shape Generator.

To settle on the shape that drives note generation, either pick from the Shape Presets drop-down menu or sketch your own directly in the display. The pitch span where notes get added is set with the Minimum and Maximum Pitch sliders. You can likewise hold Alt (Win) / Option (Mac) and click-drag to mark a span. Bear in mind that an active clip scale renders the shape in purple.

The Rate control fixes the shortest length the produced notes can have. A note's duration is also swayed by the Tie parameter, which governs the likelihood that one produced note stretches into the following one.

With the Density knob you decide how many notes get added, given as a percentage of how much of the shape you want filled.

To scatter the pitches of the produced notes, reach for the Jitter parameter. Held at 0%, the notes trace the contour in the Shape Levels display precisely, and they drift ever further from it as you raise Jitter. Bear in mind that these scattered pitches never stray outside the span fixed by the Minimum and Maximum Pitch sliders.

Notes Generated with Shape.

<a id="source-1134-stacks"></a>
### 11.3.4 Stacks

Stacks is a MIDI Tool for dropping in single chords or building chord progressions that stay within a scale you pick. Whatever chords it produces span the time selection, or the loop's span when no time selection exists.

The Stacks Generator.

A chord pattern is chosen by click-dragging the Chord Selector Pad, or with Ctrl (Win) / Cmd (Mac) together with the up and down arrow keys. Each chord pattern diagram is a plain depiction of how a chord's intervals relate to one another, drawing on the Tonnetz system. Hover over a Chord Selector Pad and the Status Bar surfaces extra detail about that chord.

Stacks also accepts custom chords once you build chord banks of your own. Such banks are text files that lay out particular chord rules using the JSON format and carry the .stacks extension. Read more about how to create chord banks in [this Knowledge Base article](https://help.ableton.com/hc/en-us/articles/14789643520668).

Bringing a custom chord bank into the Stacks Generator means dropping a .stacks file into a folder you have registered with [the browser’s Places section](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#places). After that, double-click its name in the browser so it supersedes the default bank inside Stacks.

Finding every chord file quickly is a matter of the browser’s dedicated Stacks tag under the MIDI Tool filter group, or alternatively the MIDI Tool tag under the Content filter group.

Build a chord progression with the Add Chord plus button positioned to the right of the Chord Selector Pad/s, choosing a pattern for each extra chord. Trim the chord count back down with the Delete Chord minus button.

A chord's root note is set with the Chord Root knob. You may instead hold Alt (Win) / Option (Mac) and click the piano ruler to choose it, or step through the root notes with the up and down arrow keys. Should the clip already carry a scale, the Chord Root snaps automatically to that scale's root note. Picking a different root for the chord remains possible, yet while a clip scale is active the chord's available root notes are confined to the pitches inside that clip scale.

Rearranging a chord into one of its inversions is what the Chord Inversion knob is for. Stepping up through positive values walks across the inversions open to the chosen chord, and negative values run through those same inversions one octave below. A chord's length and placement are governed by Chord Duration and Offset, each adjustable in eighths of the chord's original length.

Bear in mind that whatever parameters the Stacks Generator’s display shows at any moment belong solely to the chord that is currently selected. Consequently, selecting a different chord refreshes the display so it presents that chord’s parameters instead.

Chord Progression Generated with Stacks.
