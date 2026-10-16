# MIDI Arpeggiate Chop Connect Glissando LFO

Open when you need guidance on MIDI Arpeggiate Chop Connect Glissando LFO in Ableton Live.

Context: [Transformation Tools](midi-tools.md#112-transformation-tools).

<a id="source-1121-arpeggiate"></a>
### 11.2.1 Arpeggiate

Following the pattern settings you choose, the Arpeggiate Transformation breaks the note selection apart into arpeggiated notes. Under the hood it draws on the same machinery as the [Arpeggiator MIDI effect](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#arpeggiator).

The Arpeggiate MIDI Tool.

Through the Style drop-down menu you pick an arpeggiated sequence to lay over the selected notes. The very same 18 style patterns you know from Arpeggiator are offered by the Arpeggiate Transformation.

How far steps in the pattern are transposed is governed by the Distance control, which works in scale degrees or semitones according to whether the clip has a scale assigned.

Use the Steps slider to choose how many transposed steps the pattern contains.

Working as a pair, the Rate and Gate controls govern how notes spread across a timeline: Rate fixes the pattern’s rate (and along with it note length), while Gate shapes how long notes last. Push Gate beneath 100% and notes grow shorter; raise it past 100% and they stretch longer.

Notes Before and After Applying the Arpeggiate Transformation.

<a id="source-1122-chop"></a>
### 11.2.2 Chop

Selected MIDI notes are split by the Chop Transformation into as many as 64 parts. Beyond that, it serves to sculpt note division patterns; you might, for instance, build a pattern in which certain notes run longer than their neighbors, or one where a random wobble is folded into note start or end times.

The Chop MIDI Tool.

To build a note chopping pattern, dial in how many parts the chopped note(s) should have using the Parts control, anywhere from 2 to 64 parts. Spaces enter the pattern via the Gaps control, whose exact minimum and maximum gap counts ride on how many parts the pattern holds. Given a positive value, the control stands for how many notes pass before a gap appears. Given a negative value, it instead stands for how many gaps follow each note. As an illustration, a setting of 2 swaps a gap in for a note once two notes in a row have played, while a setting of -2 tacks two gaps onto the end of each note. Keep in mind a pattern tops out at 16 parts; set Parts above that and the pattern loops around.

Acting as a picture of the pattern shaped by the Parts and Gaps controls, the Pattern toggles also let you hand-place or remove gaps inside the pattern, a handy route to rhythmic variation. Adjusting the gap count through the Pattern toggles makes the Gaps control display a dash. Touch that control again and any hand-added gaps give way to whatever the Gaps control specifies.

Which notes or gaps stand out in the pattern is up to the Emphasis toggles. Pattern elements you emphasize respond to the Stretch Chunk(s) value, which lengthens the relative span of notes or gaps by 2 to 8 times. Once a note or gap is emphasized, its matching Pattern toggle dims out.

To sprinkle random variation across the note start and end times, reach for the Variation slider.

Notes Before and After Applying the Chop Transformation.

<a id="source-1123-connect"></a>
### 11.2.3 Connect

By creating fresh notes that bridge the spaces between notes already there, the Connect Transformation fills in the gaps. Where these interpolated notes land is random, yet certain facets of the pattern stay under your control via Connect’s parameters.

The Connect MIDI Tool.

How far the connecting notes can stray in pitch — measured against the original note pitches and expressed in scale degrees or semitones — is capped by the Spread control.

With Density you state what percentage of the time gap between original notes should be packed with interpolated notes. Set to 100%, every space between existing notes gets filled.

Reach for the Rate control to fix how long the interpolated notes run, and turn to the Tie control to govern the likelihood that a generated note stretches all the way to the next original note.

Notes Before and After Applying the Connect Transformation.

<a id="source-1124-glissando"></a>
### 11.2.4 Glissando

An MPE MIDI Tool, the Glissando Transformation links one note’s pitch to that of the note after it along a pitch bend curve, binding the pair into one. You need a minimum of two selected notes for a glissando to form.

The Glissando MIDI Tool.

Where the pitch bend curve begins is fixed by the Start control, given as a percentage of the note length. Reshaping that pitch bend curve is the job of the Curve control. Inside Glissando’s display you can grab the yellow breakpoint and slide it left or right to move where pitch bend starts, or grab the line and pull it up or down to reshape the pitch bend curve.

Notes Before and After Applying the Glissando Transformation.

Keep in mind the pitch bend curve only shows up in the MPE Editor. With the MIDI Note Editor open, Glissando’s Transformation still takes effect, yet the pitch bend curve stays hidden.

While dealing with [folded notes](https://www.ableton.com/en/live-manual/12/editing-midi/#folding-and-scales), you can surface the pitch bend curve underneath the MIDI Note Editor by switching on the Pitch Bend expression lane.

Pitch Bend Curve Displayed in a Dedicated Expression Lane.

<a id="source-1125-lfo"></a>
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
