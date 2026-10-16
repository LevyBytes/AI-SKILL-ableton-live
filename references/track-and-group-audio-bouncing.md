# Track And Group Audio Bouncing

Open when you need guidance on Track And Group Audio Bouncing in Ableton Live.

Context: [Bounce to Audio](bouncing-and-comping-routes.md#20-bounce-to-audio).

<a id="source-201-bouncing-individual-tracks"></a>
### 20.1 Bouncing Individual Tracks

Two routes exist for rendering to audio, supplied by the _Bounce Track in Place_ and _Bounce to New Track_ commands.

Bounce Track in Place renders a source track into a new audio track that takes the source's place. Keep in mind this command now stands in for what earlier Live versions called the Freeze and Flatten Track command (along with the Flatten command for frozen tracks). The Bounce Track in Place command is reachable from the track’s title bar or the clip context menu.

A Track Shown Before and After the Bounce Track in Place Command Has Been Applied.

Bounce to New Track renders single clips or a time selection into new audio clips on a separate track while muting the source clips or selection. Reach the Bounce to New Track command through the clip or selection context menu, or trigger it with the Ctrl+B (Win) / Cmd+B (Mac) shortcut.

The Source Track Alongside a New Track Produced by the Bounce to New Track Command.

Rendering to audio happens post-FX yet pre-mixer. So the resulting audio carries every bit of device processing while dropping the devices themselves from the track, and it leaves out mixer changes (namely volume, panning, and sends), which instead carry over into the new track’s settings.

If the time selection you bounce stretches across several Arrangement tracks, the Bounce to New Track command produces one audio track per track that has a clip selected on it.

What Bounce to New Track Produces from a Multi-Track Time Selection.

Be aware that even though the bouncing commands act on the Arrangement and Session at once, the outcome varies a bit by command. Run Bounce Track in Place from one view, say the Arrangement, and the new audio track also takes over the source track in the Session, with the clips on both the Arrangement and Session being rendered to audio. By contrast, running the Bounce to New Track command in a view, say the Session, still creates a new audio track in the Arrangement, but only the chosen Session clips get rendered to audio and the fresh Arrangement View track stays empty.

Any track or clip the bouncing commands produce adopts the name of its source track or clip with “(Bounce)” appended. When a source clip carries no name, its counterpart on the new track simply becomes “(Bounce).” The new track likewise picks up the color of the source track.

The audio files from a bounce live inside the Current Project folder at /Samples/Processed/Bounce.

<a id="source-202-bouncing-group-tracks"></a>
### 20.2 Bouncing Group Tracks

Beyond individual tracks, Live also lets you bounce [Group Tracks](https://www.ableton.com/en/live-manual/12/mixing/#group-tracks). Two commands handle Group Tracks: _Bounce Group in Place_ and _Bounce Group to New Track_.

Bounce Group in Place renders a new audio track that stands in for the entire Group Track. Three menus expose the command: a Group Track’s title bar context menu; in Session View, a group slot’s context menu; and within Arrangement View, the Group Track’s main lane context menu.

A Track Shown Before and After the Bounce Group in Place Command Has Been Applied.

Bounce Group to New Track renders single clips or a time selection taken from inside the Group Track into a new audio clip on a separate track, muting the source clips or selection. Two spots hold the Bounce Group to New Track command: in Session View, a group slot’s context menu; in Arrangement View, the Group Track’s main lane context menu. The Ctrl+B (Win) / Cmd+B (Mac) shortcut applies the command as well.

The Source Track Alongside a New Track Produced by the Bounce Group to New Track Command.

Keep in mind that bouncing Group Tracks behaves unlike bouncing individual tracks. Where the individual-track case bounces pre-mixer and transfers the source track’s mixer settings onto the bounced track, Group Tracks instead get bounced post-mixer. Practically, the audio is taken from the Main track’s output, capturing every effect and send applied within the Group while leaving out any processing on the Main track itself. Your actual results hinge on the routings: tracks routed away from the Group Track stay out of the bounce and can leave silence in the rendered audio, whereas return tracks sitting in the Group Track’s signal path make it into the bounce only when their final output lands on the Main track.

Bounce Group to New Track Results When One Track Is Routed Outside of the Group Track.

<a id="source-203-pasting-bounced-audio"></a>
### 20.3 Pasting Bounced Audio

The _Paste Bounced Audio_ command offers another option besides bouncing onto a new track. With this command, the source material is rendered as it stands at the moment Paste Bounced Audio runs, so you can tweak that source and rapidly bounce and paste the audio again without reselecting and recopying the source each time. It comes in handy for whipping up quick variations of one piece of material through different effects, or for collapsing several selections drawn from different tracks into one track.

Bounced Audio Drawn from Several Tracks and Pasted Into a Single Track.

For pasting bounced audio, copy clips within a single Session View track, a time selection or clips in the Arrangement, or a time selection along a Group Track’s main lane in the Arrangement. The Copy command or the Ctrl+C (Win) / Cmd+C (Mac) shortcut handles this. After that, on an audio track, an empty MIDI track, or a take lane, invoke the Paste Bounced Audio command. Two ways reach it: the track’s main lane context menu, or else the Ctrl+Alt+V (Win) / Cmd+Opt+V (Mac) shortcut. Your copied content then gets bounced and pasted onto the track. Should you paste bounced audio onto a MIDI track, that track converts to an audio track automatically.

Bear in mind that deleting the copied source material grays out the Paste Bounced Audio command until you copy something new.
