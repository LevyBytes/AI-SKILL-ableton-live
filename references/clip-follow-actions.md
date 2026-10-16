# Clip Follow Actions

Open when you need guidance on Clip Follow Actions in Ableton Live.

Context: [Launching Clips](launching-clips.md#16-launching-clips).

<a id="source-167-follow-actions"></a>
### 16.7 Follow Actions

With Follow Actions, clips can be fired in a structured fashion, at random, or as a mix of the two. A clip’s _Follow Action_ spells out what becomes of the other clips in its group once that clip has played. Clips occupying consecutive slots within a single track make up a group, and a track may hold any number of groups, each one separated from the next by vacant slots.

Follow Actions extend to [scenes](https://www.ableton.com/en/live-manual/12/session-view/#tracks-and-scenes) as well, via the controls found in the [Scene View](https://www.ableton.com/en/live-manual/12/session-view/#scene-view).

The Follow Action Controls.

1. Use the Follow Action button to switch Follow Actions on or off for whichever clip or scene is chosen. By default it sits in the off state, and the Shift+Enter keyboard shortcut flips it.
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
