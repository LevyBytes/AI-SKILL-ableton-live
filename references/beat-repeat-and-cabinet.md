# Beat Repeat And Cabinet

Open when you need guidance on Beat Repeat And Cabinet in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-285-beat-repeat"></a>
### 28.5 Beat Repeat

The Beat Repeat Effect.

With Beat Repeat you can spin out either tightly controlled or randomized echoes of whatever signal feeds it.

How frequently Beat Repeat grabs fresh audio and starts looping it is governed by the Interval control. Locked to the song tempo, Interval takes values from ”1/32” up to ”4 Bars.” The Offset control nudges the moment that Interval marks later in time. Say Interval reads ”1 Bar” and Offset reads ”8/16”: audio is then grabbed for repetition once each bar at the third beat — that is, halfway, or eight-sixteenths, into the bar.

Inject some unpredictability with the Chance control, which governs how probable it is that repetitions actually fire when Interval and Offset call for them. Set Chance to 100 percent and a repetition fires every time at the chosen Interval/Offset moment; drop it to zero and none occur at all.

In sixteenth notes, Gate fixes how long all the repetitions run in total. With Gate at ”4/16”, the repeats span a single beat, kicking off from wherever Interval and Offset place them.

Pressing the Repeat button overrides everything above, instantly grabbing audio and looping it for as long as the button stays engaged.

Grid size — how big each repeated slice is — is set with the Grid control. At ”1/16”, a one-sixteenth-note slice gets grabbed and looped for the Gate length you specified (or until Repeat is switched off). Big grid settings spawn rhythmic loops, whereas tiny ones yield sonic artifacts. Pressing No Triplets forces the grid divisions to stay binary.

The Variation control randomizes grid size. Leave Variation at ”0” and the size stays locked; raise it and the grid swings widely around your chosen Grid value. The chooser underneath offers several Variation modes: Trigger spawns grid variations each time repetitions fire; 1/4, 1/8 and 1/16 spawn them on a steady clock; and Auto makes Beat Repeat roll a fresh random variation after every repetition — the densest grid variation the device offers, all the more so when triplets are permitted.

For unusual textures, the repetitions can be dropped in pitch. Beat Repeat handles this by resampling — stretching the segments to lower their pitch and then leaving them long rather than squeezing them back to compensate. The upshot is that the rhythm can grow rather murky at steep Pitch settings. The Pitch Decay control slopes the pitch curve so each successive slice plays lower than the one before. Warning: This is the most obscure parameter of Beat Repeat.

A joint low-pass and high-pass filter is built in to carve out the frequency range the device lets through. Dedicated controls let you toggle the filter and dial in the center frequency along with the width of that passed band.

The dry input that arrived at Beat Repeat gets blended with its repetitions through one of three mix modes: Mix lets the dry signal continue through with repetitions layered on top; Insert silences the dry signal while repetitions sound but lets it through otherwise; and Gate emits the repetitions alone and never the dry signal. That Gate mode comes in handy when the device sits on a return track.

The Volume control sets the device’s output level, and Decay lets you taper the repetitions so they fade away gradually.

<a id="source-286-cabinet"></a>
### 28.6 Cabinet

The Cabinet Effect.

Cabinet is a device that recreates the tone of five vintage guitar cabinets. Built together with Softube, it relies on physical modelling to deliver a spread of convincing tones, complete with well-chosen mics and mic placement.

A range of speaker sizes and configurations is available from the Speaker chooser, whose entries spell out how many speakers there are and their size in inches. ”4x12,” for instance, denotes four 12-inch speakers. As in actual rigs, more speakers and bigger ones tend to push higher volume.

Where the virtual mic sits relative to the cabinet is governed by the Microphone chooser. Near On-Axis micing yields a bright, tightly focused tone, whereas Near Off-Axis comes across as more resonant and slightly duller. Pick the Far position for an even tone that also carries a touch of the simulated ”room.”

Cabinet Mic Positions.

Sitting under the Microphone chooser, a switch flips between a Dynamic and Condenser mic. Dynamic mics sound a little rougher and are the usual pick for close-micing guitar cabinets, since they cope with far louder levels. Condenser mics capture more faithfully and are the typical choice when micing at a distance. Naturally, Cabinet’s virtual condenser mic shrugs off loud levels unharmed, so experiment freely.

Mono versus stereo (Dual) processing is selected with the Output switch. Bear in mind that Dual mode doubles Cabinet’s CPU draw.

Balance between the processed and dry sound is handled by the Dry/Wet control.
