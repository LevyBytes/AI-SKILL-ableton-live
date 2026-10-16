# Follow Action Performance Recipes

Open when you need guidance on Follow Action Performance Recipes in Ableton Live.

Context: [Follow Actions](launching-clips.md#167-follow-actions).

<a id="source-1671-looping-parts-of-a-clip"></a>
### 16.7.1 Looping Parts of a Clip

Suppose you'd like a longer clip to play but want only its final eight bars to repeat. Follow Actions make this possible:

1. Pull the clip into the Arrangement View, confirming the Clip View’s Loop switch is off. Then reach for the Edit menu’s [Split command](https://www.ableton.com/en/live-manual/12/arrangement-view/#splitting-clips) and cut the clip at the boundary between its non-looping and looping portions.
2. Drag the two clips you've produced over to the Session View by holding the mouse cursor above the Session View selector. Release them onto a track, and at that point they constitute a Follow Action group.
   Creating a Group With the Two Clips.
3. Configure Follow Actions on the first clip. Here you'll want Follow Action Time matched to the length of the clip. Put the Follow Action A chooser on “Next“ with its Chance setting at 100%, and put Follow Action B on “No Action“. The clip is now arranged to move forward to the looping clip once it finishes.
4. Switch on the Loop switch for the second clip.

From here the first clip will hand off to the second after running all the way through, and the second will keep looping until you halt it.

<a id="source-1672-creating-cycles"></a>
### 16.7.2 Creating Cycles

Among the most apparent things Follow Actions make possible is turning a bunch of samples into a looping musical cycle. Arrange a handful of clips or scenes into a group, give every one of them the “Next“ Follow Action, and they'll sound in succession endlessly — or until you stop them.

You can sprinkle the occasional reshuffle into these cycles by layering in other Follow Actions, “Any,“ say, set to comparatively low Chance values.

Another route to making all your selected clips loop together: right-click a clip and choose the Create Follow Action Chain command from its context menu. Bear in mind your chosen clips needn't sit next to one another.

<a id="source-1673-temporarily-looping-clips"></a>
### 16.7.3 Temporarily Looping Clips

Follow Actions also lend themselves to some intriguing uses when you're after temporary musical loops.

Picture a group made of just one clip. Its Follow Action A reads “Play Again,“ carrying a Chance of 80%, while Follow Action B reads “No Action,“ carrying a Chance of 20%. The clip draws on a lengthy sample, and Follow Time stands at one bar. Click the clip and the opening bar plays; odds are strong it then repeats that opening bar. Yet after several passes it will sooner or later land on Action B — “No Action“ — and roll on through the remainder of the sample.

A clip can alternatively run from its beginning up to a chosen spot, at which point its Follow Action directs it to “Next.“ You can reuse the very same file in the group's following clip, only this one is configured to loop. That second clip is free to carry whatever Follow Action settings you like, so it may go on indefinitely, run for a set time, or hand off to the next clip in the group by random chance.

<a id="source-1674-adding-variations-in-sync"></a>
### 16.7.4 Adding Variations in Sync

Combined with [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) and [warping](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping), Follow Actions become a way to spin up every kind of fascinating variation across a group of related clips. As one instance, you might have Follow Actions randomly fire clips that each carry distinct MIDI controller clip envelopes, letting subtle shifts in an instrument or synth's pitch bend or modulation emerge as the group's clips played off one another. Audio clips, meanwhile, could shift between assorted effect or clip transposition settings.

Bringing Follow Actions and Legato Mode together gives you a potent means of nudging a melody or beat along bit by bit. Suppose a group is built from several matching clips of one melody, all configured for Legato Mode playback. Each time their Follow Actions send them onward to a different clip in the group, the melody stays intact, because Legato Mode aligns the fresh play position with the prior one in beat-time. From there the settings and clip envelopes of every clip — or even the literal notes inside a MIDI clip — can be eased into new values, putting the melody through a slow transformation.

<a id="source-1675-mixing-up-melodies-and-beats"></a>
### 16.7.5 Mixing up Melodies and Beats

Follow Actions can be turned loose to spin out unexpected remixes and solos on your behalf. Duplicate a clip that holds a beat or melody until you have a number of copies. Or else gather up several different beats or melodies that you'd like blended together. Every clip's [start and end](https://www.ableton.com/en/live-manual/12/clip-view/#clip-start-and-end-fades) can differ, and so can its [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) and the rest of its settings. Provided that each clip's Follow Action Time matches the length of whatever clip you mean to hear, you can give every clip a couple of Follow Actions bearing different Chance values, trigger one, and catch yourself off guard.

<a id="source-1676-creating-nonrepetitive-structures"></a>
### 16.7.6 Creating Nonrepetitive Structures

For sound installations, Follow Actions really shine, letting you build arrangements that run on for weeks or even months without ever repeating precisely. Dial the Follow Action Time controls across a run of clips to irregular values, and those clips will play off each other such that their order and musical placement never line up quite the same way twice. Keep in mind each clip can hold a pair of separate Follow Actions, each with its own Chance setting… enjoy!
