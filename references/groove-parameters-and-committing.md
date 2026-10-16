# Groove Parameters And Committing

Open when you need guidance on Groove Parameters And Committing in Ableton Live.

Context: [Groove Pool](grooves-and-tuning-routes.md#141-groove-pool).

<a id="source-1411-adjusting-groove-parameters"></a>
### 14.1.1 Adjusting Groove Parameters

Listed within the Groove Pool, each groove exposes several parameters you can change live to reshape how the clips relying on it behave. Buttons placed beside the Groove’s name also let you save and hot-swap it.

Here is what each control in the Groove Pool does:

- _Base_ — This chooser fixes the timing grid the groove's notes are gauged against. Pick a 1/4 Base and the groove file's note positions are judged relative to the closest quarter note, with every note in the clips tied to that groove sliding proportionally toward the groove note positions. Set a 1/8th base and the groove’s notes are gauged from their closest eighth note. Where a groove note lands precisely on the grid it stays put, so the matching notes in your clips also remain in place.
- _Quantize_ — governs how much “straight“ quantization is imposed ahead of the groove. Push it to 100% and the notes in your clips snap to the closest values per the Base chooser. Leave it at 0% and clip notes keep their starting positions until the groove acts on them.
- _Timing_ — controls the degree to which the groove pattern influences whichever clips employ it.
- _Random_ — sets how much random timing jitter reaches clips that use the chosen groove. Used sparingly, it lends a faint “humanization“ to tightly quantized electronic loops. Bear in mind that Random hands a distinct randomization to each voice in your clip, so notes that once landed together end up randomly displaced from the grid and from one another.
- _Velocity_ — dictates how strongly the velocity data held in the groove file reshapes the velocity of the clip's notes. This slider spans -100 to +100. Below zero the groove’s velocity effect flips, with loud notes sounding soft and the reverse.
- _Global Amount_ — this control scales the combined strength of Timing, Random and Velocity across all of the groove files on hand. Held at 100%, the parameters take their set values. The Amount slider reaches 130%, opening the door to even more pronounced groove effects. Whenever grooves are active on clips in your Set, the Global Amount slider turns up in Live’s Control Bar too.
  The Global Groove Amount Slider in the Control Bar

<a id="source-1412-committing-grooves"></a>
### 14.1.2 Committing Grooves

The Commit Groove Button.

Hitting the Commit button above the Clip Groove chooser “writes“ the current groove parameters into the clip. On a MIDI clip the notes shift to match. On an audio clip it lays down Warp Markers at the right spots in the clip.

Once you press Commit, the clip’s Groove chooser is reset to None on its own.
