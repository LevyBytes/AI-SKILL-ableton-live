# Launching Clips

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 16. Launching Clips

What distinguishes the Live Session View is its on-the-fly nature, offering performers a space that invites live playing and improvising. Getting the most from the Session View depends heavily on how you set up each of its clips. The settings covered in this chapter determine the way a given Session View clip responds when it is fired off, or “launched.“

### 16.1 The Launch Controls

Keep in mind that Session View clips get fired off via their [Clip Launch buttons](https://www.ableton.com/en/live-manual/12/session-view/#session-view-clips) or through [remote control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control). You will locate the relevant launch parameters in each clip's [clip panel](https://www.ableton.com/en/live-manual/12/clip-view/#follow-action-and-launch-controls). These launch parameters are relevant solely to Session View clips; Arrangement View clips aren't launched at all but instead sound according to where they sit in the Arrangement.

You reach these launch parameters by opening a Session View clip's Clip View — double-click the clip — and then selecting the clip tab/panel marked with the Clip Launch button icon.

The Clip Launch Settings in a Clip Tab.

Keep in mind that several clips' launch parameters can be adjusted together: select all the clips you want first, then bring up the Clip View.

### 16.2 Launch Modes

The Clip Launch Chooser.

Several choices appear in the Launch Mode chooser, each governing how a clip reacts to mouse clicks, presses on the computer keyboard, or incoming MIDI notes:

- Trigger: _down_ sets the clip going; _up_ has no effect.
- Gate: _down_ sets the clip going; _up_ halts it.
- Toggle: _down_ sets the clip going; _up_ has no effect. A further down press will halt the clip.
- Repeat: while you hold the mouse switch/key down, the clip retriggers over and over at the clip quantization rate.

### 16.3 Legato Mode

The Legato Mode Switch.

Imagine you've collected several looping clips on a single track and would like to switch between them while keeping everything in sync. One route is a coarse quantization value (a bar or more), but that approach can hem in what you're able to play.

A different route, one that holds up even when quantization is switched off entirely, is turning on Legato Mode for those clips. Launching a clip that has Legato Mode active makes it inherit the play position held by whichever clip ran on that track just before. As a result, switching between clips at any time and tempo never breaks the sync.

For building breaks, Legato Mode comes in very handy, since you can briefly drop into other loops and then return to whatever the track had been playing.

You may encounter dropouts when launching clips in Legato Mode unless every clip in question uses the identical sample (varying only in clip settings). The cause is that you've suddenly landed at a spot in the sample that Live had no opportunity to stream from disk ahead of time. The fix is to switch on [Clip RAM Mode](https://www.ableton.com/en/live-manual/12/clip-view/#clip-ram-mode) for those clips.

### 16.4 Clip Launch Quantization

The Clip Quantization Chooser.

Use the Clip Quantization chooser to set a correction for when triggered clips actually begin. Picking “None“ switches clip quantization off entirely.

If you'd rather follow the Control Bar’s Global Quantization value, pick “Global.“ You can rapidly alter global quantization through the Ctrl6, 7, 8, 9, and 0 (Win) / Cmd6, 7, 8, 9, and 0 (Mac) shortcuts.

Bear in mind that anything besides “None“ also quantizes a clip's launch whenever [Follow Actions](https://www.ableton.com/en/live-manual/12/launching-clips/#follow-actions) fire it.

### 16.5 Velocity

The Velocity Amount Field.

With the Velocity Amount control you dial in how strongly MIDI note velocity shapes a clip’s volume: a value of zero means no effect at all, while at 100 percent the quietest notes will trigger the clip with no sound. To learn more about driving clips from MIDI, see the [MIDI and Key Remote Control chapter](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control).

### 16.6 Clip Offset and Nudging

The Nudge Backward/Forward buttons let you leap around inside a clip that's playing, with each step equal to the global quantization period.

Using the Nudge Backward/Forward Buttons to Jump Through a Clip.

You can likewise assign these buttons to [keys or MIDI controllers](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#the-mapping-browser). While in MIDI Map Mode, a scrub control shows up between the Nudge Backward/Forward buttons, ready to be linked to a rotary encoder wheel so you can scrub continuously.

The Scrub Control in MIDI Map Mode.

When quantization sits below one bar, shifting a clip's playback away from Live’s master clock becomes straightforward — just launch clips, work the Nudge Backward/Forward buttons, or do some [scrubbing within the clip](https://www.ableton.com/en/live-manual/12/clip-view/#playing-and-scrubbing-clips).

### 16.7 Follow Actions

With Follow Actions, clips can be fired in a structured fashion, at random, or as a mix of the two. A clip’s _Follow Action_ spells out what becomes of the other clips in its group once that clip has played. Clips occupying consecutive slots within a single track make up a group, and a track may hold any number of groups, each one separated from the next by vacant slots.

Follow Actions extend to [scenes](https://www.ableton.com/en/live-manual/12/session-view/#tracks-and-scenes) as well, via the controls found in the [Scene View](https://www.ableton.com/en/live-manual/12/session-view/#scene-view).

The Follow Action Controls.

1. Use the Follow Action button to switch Follow Actions on or off for whichever clip or scene is chosen. By default it sits in the off state, and the ShiftEnter keyboard shortcut flips it.
2. With the Follow Action choosers you pick a pair of separate Follow Actions, labeled A and B. Fuller descriptions of the choices appear further down.
3. How likely each Follow Action is to fire — expressed as a percentage — comes from the Chance A and Chance B controls. Should a clip or scene carry Chance A at 100% alongside Chance B at 0%, then every single launch of that clip or scene produces Follow Action A. This illustrates that a 0% Chance value keeps an action from ever taking place. If you instead push Chance B up to 90% here, Follow Action A starts showing up far less frequently — roughly one launch in every ten for the clip or scene. Besides the Chance A and Chance B controls themselves, the slider sitting between the two can be dragged to tune the Chance values.
4. Offered for clips only, the Linked/Unlinked switch carries a pair of modes and arrives set to Linked. Under Linked mode, the Follow Action fires once the clip reaches its end, or once it has cycled through the loop count entered in the Follow Action Multiplier field. Under Unlinked mode, the Follow Action waits until the clip has run for the span of the Follow Action Time. That Follow Action Time control — present for both clips and scenes — states, in bars-beats-sixteenths measured from where playback begins in the clip or scene, the moment the Follow Action occurs. Its default value is one bar. Over in the Sample/MIDI Notes Editor a marker shows a clip's Follow Action Time, and you reshape the clip’s Follow Action Time by dragging that marker.

There are ten Follow Actions available:

indicates that nothing will follow. After a clip fires with No Action set, every other Follow Action picked for it loses its opportunity to run, even where its Follow Action Chance reads 100%.

just halts the clip once it has run for the Follow Action Time you picked. Be aware this takes priority over clip loop/region settings.

sends the clip back to its beginning.

fires the clip just above this one — the previous one.

fires the clip directly below in the group. Where a clip carrying this setting sits at the bottom of its group, the Follow Action instead fires the group's opening clip.

fires the topmost clip of a group.

fires the bottommost clip of a group.

fires any of the group's clips.

resembles “Any,“ except that whenever the present clip isn't the group's only member, the same clip won't sound twice in a row.

hands you a target clip slot or scene that the Follow Action will jump to. Choosing Jump brings up a Jump Target slider beside the Follow Action chooser. Set the target clip slot or scene by dragging that Jump Target slider up or down, or by clicking and entering a number.

A striped Clip/Scene Launch button flags any clip or scene that has Follow Actions assigned, making such items easier to spot.

Assigning a Follow Action to a Clip Changes Its Clip Launch Button.

Keep in mind that a clip Follow Action fires precisely once the span given by the Follow Action Time controls has elapsed — unless clip quantization holds some value besides “None“ or “Global.“ Follow Actions sidestep global quantization, yet clip quantization still applies to them.

Beside the Back to Arrangement button sits an Enable Follow Actions Globally button, through which you turn every clip and scene Follow Action in the Live Set on or off. Switching the Enable Follow Actions Globally button off lets you tweak clips as they play without having playback leap off to other clips. Keep in mind that the Enable Follow Actions Globally button shows up grayed out whenever a Live Set holds no clip or scene Follow Actions at all.

The Enable Follow Actions Globally button.

Keep in mind that clip Follow Actions keep running even after a scene Follow Action gets made or queued; nonetheless, once a scene Follow Action fires, it always wins out.

What's the point of Follow Actions, then? Music lives in repetition and change. When a piece rests on loops or brief melodic snippets, it tends toward a static feel. Follow Actions let you build patterns that recur and yet still hold surprises. Bear in mind you can at any time [record](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips) whatever your experimenting yields, which makes a fine well of fresh ideas.

The sections that come next walk through hands-on examples and concepts for Follow Actions.

### 16.7.1 Looping Parts of a Clip

Suppose you'd like a longer clip to play but want only its final eight bars to repeat. Follow Actions make this possible:

1. Pull the clip into the Arrangement View, confirming the Clip View’s Loop switch is off. Then reach for the Edit menu’s [Split command](https://www.ableton.com/en/live-manual/12/arrangement-view/#splitting-clips) and cut the clip at the boundary between its non-looping and looping portions.
2. Drag the two clips you've produced over to the Session View by holding the mouse cursor above the Session View selector. Release them onto a track, and at that point they constitute a Follow Action group.
   Creating a Group With the Two Clips.
3. Configure Follow Actions on the first clip. Here you'll want Follow Action Time matched to the length of the clip. Put the Follow Action A chooser on “Next“ with its Chance setting at 100%, and put Follow Action B on “No Action“. The clip is now arranged to move forward to the looping clip once it finishes.
4. Switch on the Loop switch for the second clip.

From here the first clip will hand off to the second after running all the way through, and the second will keep looping until you halt it.

### 16.7.2 Creating Cycles

Among the most apparent things Follow Actions make possible is turning a bunch of samples into a looping musical cycle. Arrange a handful of clips or scenes into a group, give every one of them the “Next“ Follow Action, and they'll sound in succession endlessly — or until you stop them.

You can sprinkle the occasional reshuffle into these cycles by layering in other Follow Actions, “Any,“ say, set to comparatively low Chance values.

Another route to making all your selected clips loop together: right-click a clip and choose the Create Follow Action Chain command from its context menu. Bear in mind your chosen clips needn't sit next to one another.

### 16.7.3 Temporarily Looping Clips

Follow Actions also lend themselves to some intriguing uses when you're after temporary musical loops.

Picture a group made of just one clip. Its Follow Action A reads “Play Again,“ carrying a Chance of 80%, while Follow Action B reads “No Action,“ carrying a Chance of 20%. The clip draws on a lengthy sample, and Follow Time stands at one bar. Click the clip and the opening bar plays; odds are strong it then repeats that opening bar. Yet after several passes it will sooner or later land on Action B — “No Action“ — and roll on through the remainder of the sample.

A clip can alternatively run from its beginning up to a chosen spot, at which point its Follow Action directs it to “Next.“ You can reuse the very same file in the group's following clip, only this one is configured to loop. That second clip is free to carry whatever Follow Action settings you like, so it may go on indefinitely, run for a set time, or hand off to the next clip in the group by random chance.

### 16.7.4 Adding Variations in Sync

Combined with [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) and [warping](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping), Follow Actions become a way to spin up every kind of fascinating variation across a group of related clips. As one instance, you might have Follow Actions randomly fire clips that each carry distinct MIDI controller clip envelopes, letting subtle shifts in an instrument or synth's pitch bend or modulation emerge as the group's clips played off one another. Audio clips, meanwhile, could shift between assorted effect or clip transposition settings.

Bringing Follow Actions and Legato Mode together gives you a potent means of nudging a melody or beat along bit by bit. Suppose a group is built from several matching clips of one melody, all configured for Legato Mode playback. Each time their Follow Actions send them onward to a different clip in the group, the melody stays intact, because Legato Mode aligns the fresh play position with the prior one in beat-time. From there the settings and clip envelopes of every clip — or even the literal notes inside a MIDI clip — can be eased into new values, putting the melody through a slow transformation.

### 16.7.5 Mixing up Melodies and Beats

Follow Actions can be turned loose to spin out unexpected remixes and solos on your behalf. Duplicate a clip that holds a beat or melody until you have a number of copies. Or else gather up several different beats or melodies that you'd like blended together. Every clip's [start and end](https://www.ableton.com/en/live-manual/12/clip-view/#clip-start-and-end-fades) can differ, and so can its [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) and the rest of its settings. Provided that each clip's Follow Action Time matches the length of whatever clip you mean to hear, you can give every clip a couple of Follow Actions bearing different Chance values, trigger one, and catch yourself off guard.

### 16.7.6 Creating Nonrepetitive Structures

For sound installations, Follow Actions really shine, letting you build arrangements that run on for weeks or even months without ever repeating precisely. Dial the Follow Action Time controls across a run of clips to irregular values, and those clips will play off each other such that their order and musical placement never line up quite the same way twice. Keep in mind each clip can hold a pair of separate Follow Actions, each with its own Chance setting… enjoy!
