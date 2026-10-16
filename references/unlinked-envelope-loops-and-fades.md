# Unlinked Envelope Loops And Fades

Open when you need guidance on Unlinked Envelope Loops And Fades in Ableton Live.

Context: [Unlinking Clip Envelopes From Clips](clip-envelopes.md#265-unlinking-clip-envelopes-from-clips).

<a id="source-2651-programming-a-fade-out-for-a-live-set"></a>
### 26.5.1 Programming a Fade-Out for a Live Set

Begin with an uncomplicated case. Picture yourself building a Live Set where you want an eight-bar fade-out to fire whenever one particular audio clip starts — except the only material on hand is a single one-bar loop.

Employing a Clip Envelope to Build a Fade-Out Across Several Passes of a Loop.

1. Pick either the Clip Gain or the Mixer Track Volume envelope, then _unlink_ it from the sample.
2. The clip envelope's loop braces take on color, signaling that this envelope now carries local loop/region settings of its own. Over in the Envelopes tab the loop/region controls “come to life.“ Flip the envelope's Loop switch and you'll see the Clip tab/panel's Loop switch stays put — the sample goes on looping even as the envelope plays back as a “one-shot.”
3. Enter “8“ in the leftmost box for the envelope's loop length.
4. Pull the envelope view fully out by clicking the Envelope's time ruler and dragging upward.
5. Drop a breakpoint where the region ends and pull it down to the bottom.

Play the clip now and you'll hear that one-bar loop fade away across eight bars.

<a id="source-2652-creating-long-loops-from-short-loops"></a>
### 26.5.2 Creating Long Loops from Short Loops

Now push the idea one notch further. Elsewhere in your set you'd like to reuse that very same one-bar loop — it sounds terrific — but hearing it repeat over and over wears thin. What you want is to stretch it into a longer loop somehow.

Pick up from the clip we just rigged to fade out across eight bars. Switch on the Loop switch of the clip volume envelope. Play the clip now and the eight-bar fade-out repeats. You're free to draw or reshape any envelope to lay over the sample loop. None of this is limited to volume, of course — it applies to any other control too; why not a filter sweep every four bars?

Keep in mind that the Envelope Editor lets you carve out as much time as you require, whether by hauling the loop braces past the edge of the view or by typing figures into the numeric region/loop controls.

For every envelope you're free to set whatever loop length you fancy, odd ones like 3.2.1 included. It's easy enough to picture serious intricacy (and bewilderment!) emerging once a single clip holds several envelopes of odd length.

The Sample (Left) and Envelope (Right) Start Marker.

Reining in that intricacy calls for a shared point of reference. The start marker pins down the spot from which sample or envelope playback sets off whenever the clip begins.

Be aware that, like envelope drawing itself, the start/end markers and the loop brace get quantized by the [zoom-adaptive grid](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid).

<a id="source-2653-imposing-rhythm-patterns-onto-samples"></a>
### 26.5.3 Imposing Rhythm Patterns onto Samples

Up to this point our discussion has centered on laying long envelopes over short loops. There are equally interesting uses that run in the opposite direction. Take a sample holding a song that stretches several minutes long. A clip could play that sample using a one-bar volume envelope loop, where the loop now behaves as a pattern that keeps “punching“ holes through the music — knocking out every third beat, say. You can surely picture other parameters such a pattern might modulate to intriguing effect.

<a id="source-2654-clip-envelopes-as-lfos"></a>
### 26.5.4 Clip Envelopes as LFOs

For anyone drawn to sound synthesis, it can help to regard a clip envelope carrying a local loop as an LFO. That LFO runs locked to the project tempo, though you can equally pick a loop period quirky enough to leave the envelope out of sync. Hide the grid and you're able to set the clip envelope's loop start and end points free of any meter grid.

Between the [Stretch/Skew Envelope handles](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#stretching-and-skewing-envelopes) and the [automation shapes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#inserting-automation-shapes), you have the means to craft inventive LFO contours.

<a id="source-2655-warping-linked-envelopes"></a>
### 26.5.5 Warping Linked Envelopes

While Linked mode is active, clip envelopes react to whatever happens to the clip's Warp Markers. In practice this means dragging a warp marker stretches or compresses the clip envelope to match. On top of that, you can tweak Warp Markers right inside the envelope editor.

Clip Envelopes and Warp Markers Can Be Adjusted Together.
