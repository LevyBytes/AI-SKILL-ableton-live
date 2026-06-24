# Midi Tools (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 11. MIDI Tools

For anyone shaping MIDI material, MIDI Tools unlock a broader range of editing options. You reach these scale-aware helpers through the Transform and Generate panels found in the Clip View. Transformations concentrate on focused edits to MIDI notes that already exist, whereas Generators lean toward experimentation and end up producing fresh musical material.

[Transformation Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#transformation-tools) reshape a range of properties on notes that are already present, MPE data included. Before a transformation can run, you have to feed it a selection of notes.

A particular family within Transformations, the MPE MIDI Tools let you introduce note expression or reshape expression data you already have. To inspect what these MIDI Tools produce, look at the MIDI Note Editor’s [MPE view mode](https://www.ableton.com/en/live-manual/12/editing-mpe/#viewing-mpe-data).

By contrast, [Generative Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#generative-tools) take nothing as input; they simply place fresh notes into the clip loop or time selection. Keep in mind that whenever notes are already sitting in the clip or time selection, whatever is generated will overwrite them.

Both Transformations and Generators split further into the native MIDI Tools and the Max for Live variety. The native ones ship inside Live and expose no editable internals. The bundled Max for Live MIDI Tools, on the other hand, are open to editing, and beyond that you can [build additional MIDI Tools](https://www.ableton.com/en/live-manual/12/max-for-live/#building-max-for-live-midi-tools) of your own or [install MIDI Tools from third-party creators](https://www.ableton.com/en/live-manual/12/midi-tools/#using-max-for-live-midi-tools) to grow how much you can transform and generate notes. Any Max for Live MIDI Tools you have created or stored turn up fast inside [the browser](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#working-with-the-browser), thanks to a purpose-made MIDI Tools [filter group](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#filter-groups) along with the MIDI Tool [tag](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#tags) under the Content filter group.

### 11.1 Using MIDI Tools

To put a MIDI Tool to work transforming or generating notes, bring up the Transform or Generate panel, pick a tool from the Transformation/Generator Selector chooser, and adjust the controls inside the chosen MIDI Tool’s interface. Every MIDI Tool ships with the Auto Apply button switched on out of the box. With it active, your edits to a MIDI Tool’s settings transform or generate MIDI notes the moment you make them.

The Auto Apply Button.

From then on, every tweak you make to a MIDI Tool’s parameters shows up in the MIDI Note Editor without delay. Should you prefer that the Transformations and Generators not act right away, switch the Auto Apply button off. Bear in mind that flipping this button off returns the notes to how they started.

Once the Auto Apply button is off, take your time dialing in a MIDI Tool’s parameters; when the settings feel right, hit the Apply button so the changes are committed.

The Apply Button.

There’s also a way to apply whichever MIDI Tool is selected without stepping out of the MIDI Note Editor — just press CtrlEnter (Win) / CmdEnter (Mac).

Whenever you run a Transformation, it targets the time selection, the note selection, or the clip loop (in cases where neither a time nor a note selection exists). Running a Transformation swaps the original notes out for the transformed ones.

A Generator, meanwhile, targets the time selection or, lacking one, the clip loop. Should notes already be sitting in the MIDI Note Editor as a Generator runs, the new notes will either join the current material (when the old and new notes steer clear of each other) or take its place (when the existing and generated notes overlap).

Because MIDI Tools respect scale, enabling a scale on a clip causes every pitch-related parameter across the MIDI Tools to read in scale degrees rather than semitones.

Whatever transforming or generating you do to notes is reversible through the Undo and Redo commands in the Edit menu. Keep in mind that those commands touch only the edits made to MIDI notes, leaving any changes to a MIDI Tool’s parameters untouched. To send the parameters back to how they began, use the Reset button, which dims out the moment the MIDI Tool returns to default.

An Active Reset Button.

Bear in mind the Reset button reaches only the parameters of the chosen MIDI Tool; the MIDI notes themselves are left alone.

### 11.1.1 Using Max for Live MIDI Tools

Beyond the native MIDI Tools that come with Live, the Max for Live MIDI Tools are also at your disposal for transforming and generating notes inside clips. These Max for Live MIDI Tools take the form of AMXD files and slot into the Transform or Generative Tools tab/panel within the Clip View. Just as you would with any other Max device, you can open a Max patcher to edit or build Max for Live MIDI Tools.

Live Standard and Suite arrive with two ready-made Max for Live MIDI Tools: [Velocity Shaper](https://www.ableton.com/en/live-manual/12/midi-tools/#velocity-shaper) along with [Euclidean](https://www.ableton.com/en/live-manual/12/midi-tools/#euclidean). Running the Suite edition, or the Standard edition paired with the Max for Live add-on, additionally lets you craft and edit your own [Max for Live MIDI Tools](https://www.ableton.com/en/live-manual/12/max-for-live/#building-max-for-live-midi-tools) or pull in Max for Live MIDI Tools made by third parties.

For third-party Max for Live MIDI Tools to appear in the Transform and Generative tabs/panels of the Clip View, store them in the following folders on your machine:

- _Transformations_: ~/Music/Ableton/User Library/MIDI Tools/Max Transformations
- _Generators_: ~/Music/Ableton/User Library/MIDI Tools/Max Generators

As another option, the AMXD files of third-party MIDI Tools may be placed in any folder sitting under Places in Live’s browser.

### 11.2 Transformation Tools

What follows is a rundown of every MIDI Transformation that ships with Live.

### 11.2.1 Arpeggiate

Following the pattern settings you choose, the Arpeggiate Transformation breaks the note selection apart into arpeggiated notes. Under the hood it draws on the same machinery as the [Arpeggiator MIDI effect](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#arpeggiator).

The Arpeggiate MIDI Tool.

Through the Style drop-down menu you pick an arpeggiated sequence to lay over the selected notes. The very same 18 style patterns you know from Arpeggiator are offered by the Arpeggiate Transformation.

How far steps in the pattern are transposed is governed by the Distance control, which works in scale degrees or semitones according to whether the clip has a scale assigned.

Use the Steps slider to choose how many transposed steps the pattern contains.

Working as a pair, the Rate and Gate controls govern how notes spread across a timeline: Rate fixes the pattern’s rate (and along with it note length), while Gate shapes how long notes last. Push Gate beneath 100% and notes grow shorter; raise it past 100% and they stretch longer.

Notes Before and After Applying the Arpeggiate Transformation.

### 11.2.2 Chop

Selected MIDI notes are split by the Chop Transformation into as many as 64 parts. Beyond that, it serves to sculpt note division patterns; you might, for instance, build a pattern in which certain notes run longer than their neighbors, or one where a random wobble is folded into note start or end times.

The Chop MIDI Tool.

To build a note chopping pattern, dial in how many parts the chopped note(s) should have using the Parts control, anywhere from 2 to 64 parts. Spaces enter the pattern via the Gaps control, whose exact minimum and maximum gap counts ride on how many parts the pattern holds. Given a positive value, the control stands for how many notes pass before a gap appears. Given a negative value, it instead stands for how many gaps follow each note. As an illustration, a setting of 2 swaps a gap in for a note once two notes in a row have played, while a setting of -2 tacks two gaps onto the end of each note. Keep in mind a pattern tops out at 16 parts; set Parts above that and the pattern loops around.

Acting as a picture of the pattern shaped by the Parts and Gaps controls, the Pattern toggles also let you hand-place or remove gaps inside the pattern, a handy route to rhythmic variation. Adjusting the gap count through the Pattern toggles makes the Gaps control display a dash. Touch that control again and any hand-added gaps give way to whatever the Gaps control specifies.

Which notes or gaps stand out in the pattern is up to the Emphasis toggles. Pattern elements you emphasize respond to the Stretch Chunk(s) value, which lengthens the relative span of notes or gaps by 2 to 8 times. Once a note or gap is emphasized, its matching Pattern toggle dims out.

To sprinkle random variation across the note start and end times, reach for the Variation slider.

Notes Before and After Applying the Chop Transformation.

### 11.2.3 Connect

By creating fresh notes that bridge the spaces between notes already there, the Connect Transformation fills in the gaps. Where these interpolated notes land is random, yet certain facets of the pattern stay under your control via Connect’s parameters.

The Connect MIDI Tool.

How far the connecting notes can stray in pitch — measured against the original note pitches and expressed in scale degrees or semitones — is capped by the Spread control.

With Density you state what percentage of the time gap between original notes should be packed with interpolated notes. Set to 100%, every space between existing notes gets filled.

Reach for the Rate control to fix how long the interpolated notes run, and turn to the Tie control to govern the likelihood that a generated note stretches all the way to the next original note.

Notes Before and After Applying the Connect Transformation.

### 11.2.4 Glissando

An MPE MIDI Tool, the Glissando Transformation links one note’s pitch to that of the note after it along a pitch bend curve, binding the pair into one. You need a minimum of two selected notes for a glissando to form.

The Glissando MIDI Tool.

Where the pitch bend curve begins is fixed by the Start control, given as a percentage of the note length. Reshaping that pitch bend curve is the job of the Curve control. Inside Glissando’s display you can grab the yellow breakpoint and slide it left or right to move where pitch bend starts, or grab the line and pull it up or down to reshape the pitch bend curve.

Notes Before and After Applying the Glissando Transformation.

Keep in mind the pitch bend curve only shows up in the MPE Editor. With the MIDI Note Editor open, Glissando’s Transformation still takes effect, yet the pitch bend curve stays hidden.

While dealing with [folded notes](https://www.ableton.com/en/live-manual/12/editing-midi/#folding-and-scales), you can surface the pitch bend curve underneath the MIDI Note Editor by switching on the Pitch Bend expression lane.

Pitch Bend Curve Displayed in a Dedicated Expression Lane.

### 11.2.5 LFO

As an MPE Transformation, LFO leans on a low-frequency oscillator to drive the value of one among three MPE parameters: pitch bend, slide, or pressure. You tailor the oscillator’s shape, its rate, and its overall amplitude all through the Transformation’s parameters.

The LFO MIDI Tool.

Through the Target chooser you point the LFO at Pitch Bend, Slide, or Pressure as its modulation target. Meanwhile the LFO curve display draws the shape of the LFO serving as the modulation source.

How quickly the oscillator’s amplitude envelope rises and falls — relative to the oscillation’s full length — comes from the Envelope Attack and Decay sliders. Be aware that the envelope’s attack and decay values are linked: drive Attack to 100%, for instance, and Decay snaps to 0% on its own.

Whatever you pick in the Shape Type chooser, the Shape control then tunes the oscillator’s form. Four types are on offer: Sine, Square, Triangle, or Random. With Random in play, the Reseed button spins up new random shapes for the LFO.

The Reseed Button.

In musical time, the Rate control fixes the oscillator’s period across a span from 1 to 1/128 — a rate of 1, for example, lines up with 4 beats. Sitting beneath Rate, the Time Shift slider nudges the LFO along the time axis: positive values push back when the oscillation begins, and negative values shift its phase.

Setting the oscillator’s amplitude falls to the Amount control. With Pitch Bend chosen as the modulation target, Amount reaches any value spanning double the clip’s current pitch bend range — so for a range of ±60 st, Amount runs from -120 st to 120 st. Pick Slide or Pressure instead and Amount ranges from -127 to 127. The amplitude’s base value comes from the Amplitude Base slider sitting under the Amount control. When Pitch Bend is the modulation target, Amplitude Base may take any value inside the clip’s current pitch bend range — given a range of ±60 st, that means -60 st to 60 st. For Slide or Pressure, Amplitude Base instead spans -127 to 127.

Notes Before and After Applying the LFO Transformation.

For the Pitch Bend modulation target, the MPE curve appears in the MIDI Note Editor. You may also opt to show it beneath the MIDI Note Editor by switching on the Pitch Bend expression lane, which proves useful with [folded notes](https://www.ableton.com/en/live-manual/12/editing-midi/#folding-and-scales). The modulation curves for Slide and Pressure each appear in their own expression lanes.

Be aware the modulation the LFO Transformation produces shows only in the MPE Editor. While the MIDI Note Editor is open, the Transformation still runs, but its expression curves remain out of sight.

### 11.2.6 Ornament

Through its Flam and Grace Notes options, the Ornament Transformation lets you tack ornamental notes onto the front of selected notes. Run the Transformation over the same selection a second time and yet more flam or grace notes get slipped in.

The Ornament MIDI Tool.

Choose which kind of ornamental notes to layer on by flipping on either the Flam or the Grace Notes toggle.

The Flam and Grace Notes Toggles.

With Flam, one lone note is tacked onto the front of every selected note.

Where that flam note sits is set by the Flam Position parameter: positive values have the flam note overwrite the front of the original note, whereas negative values slot the flam note ahead of the selected note’s start. Since the parameter’s value is a percentage of the current grid setting, the flam note’s length keys off the grid size rather than the original note’s length. As a result, at 100% / -100% the flam note spans one grid division — sitting at the original note’s start or just before it — and shrinks proportionally as Flam Position drifts toward 0%.

The velocity of the flam notes, measured against the velocity of the original notes, is what the Flam Velocity parameter sets.

Notes Before and After Adding Flam.

With Grace Notes, several notes of matching length are tacked onto the front of each original note.

Using the Grace Notes Pitch buttons you decide the pitch of the added grace notes relative to the original note. Choose High and every other grace note lands one semitone (or scale degree, where a scale is active) above the original notes; choose Low and every other grace note sits one semitone or scale degree under the existing notes. Pick Same and the grace notes share the original notes’ pitch.

Whether the added grace notes overwrite the front of the selected notes (with the parameter at positive values) or sit ahead of the original notes (at negative values) is decided by the Grace Notes Position parameter. Expressed as a share of whatever grid size is active, its value works like this: at 100% / -100% the inserted graces notes span a single grid division, landing either at the original note’s start or right before it.

How loud the grace notes are relative to the velocity of the original notes is set by the Grace Notes Velocity parameter.

The Grace Notes Chance control fixes the odds that each grace note sounds, gauged against the original note’s Chance values.

With the Grace Notes Amount parameter you state how many grace notes to attach to each selected note. Every individual grace note always comes out the same size.

Note Selection Before and After Adding Grace Notes.

### 11.2.7 Quantize

By shifting or stretching the selected notes to match the quantization settings you specify, the Quantize MIDI Tool tightens their timing. Be aware that a matching Quantize tool is available for [audio clips](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#quantizing-audio) too.

The Quantize Transformation.

You may quantize notes to the current grid size or instead name a particular meter value (triplets included). It’s open to you to quantize the note start time, the note end time, or both at once. Quantizing a note’s end stretches it until it terminates on the meter subdivision you chose. The Amount control even lets you quantize notes while sidestepping that fully “quantized” feel, since it shifts notes by only a fraction of the set quantization value.

Notes Before and After Applying Quantization.

Besides reaching the Transformation through Clip View’s tabs/panels, you can call up the Quantize MIDI Tool to adjust its parameters via the Quantize Settings… command in the Edit menu, or fire the CtrlShiftU (Win) / CmdShiftU (Mac) shortcut to quantize the selected notes without ever opening the Transform tab/panel.

### 11.2.8 Recombine

For a chosen group of notes, the Recombine MIDI Tool reshuffles the position, pitch, duration, or velocity so that a parameter value belonging to one note in the group ends up applied to another note.

The Recombine Transformation.

The Dimension chooser is where you settle on which one of four note parameters Recombine will permute: Position, Pitch, Duration, or Velocity.

The Dimension Chooser.

Recombine offers three approaches to reordering note parameters: 1. Shuffle, in which note parameters are permuted at random. 2. Mirror, in which note parameters are permuted so they run opposite to the note selection. 3. Rotate, in which note parameters are permuted in a circular fashion.

You flip on the Shuffle and Mirror permutation types with their own toggles, while Rotate only kicks in once you give Rotation Steps a value other than 0.

To set Rotation Steps, drag your mouse across the columns inside Recombine’s display, or use the Rotate Step Down/Up buttons beneath the display. The count of available steps always sits one below the number of selected notes. Positive numbers spin parameter values clockwise; negative numbers spin them counter-clockwise.

Pick Position in the Dimension chooser and the Rotate on Grid toggle becomes available. Switched on, it has Recombine count grid cells in the selection — rather than notes — to figure how many Rotation Steps exist. Exactly how many Rotation Steps are available then hinges on the current grid settings.

You can call on each permutation type on its own or stack several together. They run in a fixed order: first Shuffle, then Mirror, then Rotate. Bear in mind that with Shuffle on, a fresh parameter permutation is born every time you hit the Apply button.

Note Velocities Before and After Applying the Shuffle Transformation Mode.

### 11.2.9 Span

Drawing on three articulation types — legato, tenuto and staccato — the Span MIDI Tool reshapes the durations of selected notes.

The Span Transformation.

A couple of extra parameters let you bring some variety to how the notes are transformed:

- Offset shifts note end times by up to a grid step. Positive values lengthen the note; negative values shorten it.
- Variation sprinkles random spread across note lengths. Positive values shorten the note, while negative values lengthen it. Set to anything other than 0%, it brews up fresh note length variation each time you reapply the Transformation.

With Legato, each selected note grows until it reaches the start time of the note that follows. The final selected note runs to the close of the time selection or, where there is none, to the end of the loop.

Notes Before and After Applying Legato.

Tenuto leaves the original note length intact unless you touch the Offset and Variation parameters.

Under the Staccato articulation type, note length follows from the spacing between the selected notes’ start times. The tightest gap between start times is cut in half, and that span becomes the new note length for the transformed notes. From there, the Offset and Variation parameters let you tweak note length further.

### 11.2.10 Strum

Following a shape laid out by the Strum Low, Strum High and Tension parameters, the Strum MIDI Tool nudges the start times of the notes within a chord.

The Strum Transformation.

Working from the lowest note upward, the Strum Low parameter sets how far the successive notes are offset. Positive values push the note start times earlier, while negative values pull them back. At 100% / -100% the lowest note’s start time shifts by as much as one grid step. The remaining notes follow proportionally, tracing the shape shown in the Strum Position display. Should the Tension parameter sit at 0.0%, the notes spread out at equal spacing from one another.

Starting instead from the highest note, the Strum High parameter governs the offset across the original chord. Positive values move the note start times earlier, and negative values move them back. At 100% / -100% the highest note shifts by up to a grid step. The other notes spread proportionally to mirror the shape in the display. With the Tension parameter at 0.0%, the notes land at even spacing between each other.

For the Transformation to do anything, the Strum Low and/or Strum High parameters have to hold a value other than 0.0%. You can alter either parameter by dragging its breakpoint in the Strum Position display, or by typing a value for each on your computer keyboard.

What the Tension parameter does is reshape the offset of note start times so they stop sitting at uniform spacing and instead trace a curve, with the gaps between notes widening or narrowing according to the setting. Positive Tension values make the gap between notes widest at the start of the sequence before it tapers off exponentially. Negative values make the gap narrow at the start of the sequence and then grow exponentially.

Notes Before and After Applying the Strum Transformation.

### 11.2.11 Time Warp

A time-stretching MIDI Tool, Time Warp reworks selected notes by following a speed curve, which opens the door to tempo shifts like accelerando or ritardando.

The Time Warp Transformation.

The speed curve is something you build inside the Breakpoints display, where the curve’s time range lines up with the time selection. Using their individual toggles, you can turn on anywhere from one to three breakpoints along the speed curve. To position a breakpoint, either drag it in the display or select it and reach for the Breakpoint Time and Breakpoint Speed sliders, which set its timeline position and speed in turn. Whatever the sliders read always mirrors the breakpoint you currently have selected.
