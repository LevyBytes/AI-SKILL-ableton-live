# Simpler Classic One Shot And Slicing

Open when you need guidance on Simpler Classic One Shot And Slicing in Ableton Live.

Context: [Playback Modes](sampler-modulation-and-simpler-routes.md#30111-playback-modes).

<a id="source-301111-classic-playback-mode"></a>
#### 30.11.1.1 Classic Playback Mode

The Sample Tab in Classic Playback Mode.

Under Classic Playback Mode, the assorted sample position controls govern which part of the sample is played. Among them are the Start and Length parameters together with the two “flags” shown on the waveform display. The left flag fixes the absolute spot in the sample where playback may begin, and the End control fixes where playback may stop. Start and Length are then expressed as percentages of the full sample length that the flags allow. A Length value of 50%, for instance, sounds precisely half of the region lying between the flags. The Loop slider sets what portion of the available sample loops. It only does anything when the Loop switch is on.

You can build sustaining loops short enough to acquire a glitchy or granular quality, or even to ring out as a pitch from looping at audio rates. That may be precisely the effect you are after, yet it can drive CPU very high, especially under the Complex or Complex Pro Warp Modes.

Frequently you will begin with a wide region of a sample and wind up keeping just a sliver of it. You can zoom and pan Simpler’s waveform display the same way you do elsewhere in Live — to zoom, drag up and down or scroll on the mousewheel or trackpad while holding the Ctrl (Win) / Cmd (Mac) modifier, and to pan, drag sideways to bring other parts of the sample into view. The zooming behaves identically across all three playback modes.

Clicking the Loop On/Off button decides whether the sample loops while a note is held. Clicks or pops can arise at a looped sample’s start and end points because of the jump in waveform amplitude (that is, the sample’s loudness). The Snap switch helps reduce these by pinning Simpler’s loop and region markers to _zero-crossing_ spots within the sample (spots where the amplitude reads zero). Snapping uses the left channel of a stereo sample as its reference. As a result, glitches with stereo samples remain possible even when Snap is on.

You can smooth the jump from loop end back to loop start using the Fade control, which crossfades the two points together. The technique pays off particularly with lengthy, textural samples.

With the Gain slider you can raise or lower the sample’s level. Keep in mind that it is a gain stage apart from Simpler’s Volume knob, which fixes the instrument’s final output level (once the signal has passed through Simpler’s filter). The parameter is present in all three playback modes.

How many voices Simpler can sound at once is capped by the Voices parameter. Should more voices be required than the Voices chooser permits, “voice stealing“ kicks in, dropping the oldest voice(s) so the newest ones can sound. If, say, your Voices parameter sits at 8 while ten voices all compete to play, the two oldest get dropped. (Simpler does its best to keep voice stealing unobtrusive.)

When Retrig is on, replaying a note that is still sustaining cuts off the prior instance. With Retrig off, several copies of the same note may layer over one another. Bear in mind that Retrig produces an audible difference only when the sample has a long release time and Voices is set above one.

Across all three playback modes the assorted [warp parameters](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#warp-controls) behave identically and are covered below.

<a id="source-301112-one-shot-playback-mode"></a>
#### 30.11.1.2 One-Shot Playback Mode

The Sample Tab in One-Shot Playback Mode.

Under One-Shot Playback Mode, the left and right flags delimit the available playback region exactly as in Classic Mode, but Loop and Length controls are absent. A Voices control is missing too, since One-Shot Mode is purely monophonic.

When Trigger is on, the sample keeps sounding after you let go of the note; how long you hold the pad makes no difference while Trigger is on.

The Fade In and Fade Out controls let you contour the sample’s loudness. Fade In sets how long the sample takes to reach full volume once a note is struck, and Fade Out starts fading the specified span before the sample region finishes.

When Gate is on, the sample starts to fade the moment you release the note. The Fade Out time fixes how long it takes to reach silence following release.

Snap operates much as it does in Classic Mode, except here it influences only the start and end flags (since there are no loop options.)

<a id="source-301113-slicing-playback-mode"></a>
#### 30.11.1.3 Slicing Playback Mode

The Sample Tab in Slicing Playback Mode.

Under Slicing Playback Mode (just like One-Shot Playback Mode), the left and right flags delimit the available playback region.

Which method governs slice creation is set by the Slice By chooser:

- _Transient_ - Slices land automatically on the sample’s transients. The Sensitivity slider controls how responsive Simpler is to transient levels in the sample, and therefore how many slices it makes on its own. Larger values yield more slices, capped at 64 slices.
- _Beat_ - Slices land at musical beat divisions. The Division chooser picks the beat division Simpler uses to slice the sample region.
- _Region_ - Slices land at uniform time divisions. The Regions chooser picks how many equally spaced slices get created.
- _Manual_ - Slices are made by hand through double-clicking inside the sample region. With Manual chosen, no slices appear automatically.

How many slices can sound at the same time is set by the Playback chooser. Mono is monophonic, allowing one slice to play at any moment. With Poly chosen, several slices can fire together. The Voices and Retrig controls become available under Poly and operate just as in Classic Playback Mode. With Thru chosen, playback stays monophonic, yet triggering a single slice carries playback onward through the remainder of the sample region.

The Trigger/Gate switch operates identically to its behavior in One-Shot Playback Mode. The Fade In and Out controls act a bit differently according to the Playback chooser’s setting. Under Mono or Poly, the Fade times span from the start to the finish of each separate slice, whereas under Thru they span from the triggered slice to the region’s end. Consequently the fade times can sound unlike one another depending on where within the region you trigger.

Slices generated automatically show up as vertical blue lines across the waveform display. A double-click on a slice removes it. Should Simpler’s automatic slice positions not please you, you can drag a slice to relocate it. Double-clicking on the waveform in the gap between slices adds manual slices, which display in white. While in Transients mode, holding Alt (Win) / Option (Mac) and clicking a slice flips it between a manual and an automatic slice. Manual slices made in Transients mode survive no matter what the Sensitivity amount is.
