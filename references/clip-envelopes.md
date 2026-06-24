# Clip Envelopes

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 26. Clip Envelopes

Any clip in Live may carry its own set of _clip envelopes_. Which facets of a clip these envelopes act on varies with the clip's type and configuration; their reach spans everything from carrying MIDI controller data to _automating_ or _modulating_ device parameters. This chapter begins by covering the shared mechanics of drawing and editing every clip envelope, and afterward turns to the specifics of each individual use.

### 26.1 The Clip Envelope Editor

Begin editing clip envelopes by opening the Clip View's Envelopes tab — click its tab header (the one bearing the icon) within the Clip View. Inside the Envelopes tab sit two choosers that let you pick which envelope to display and modify.

The Clip View's Envelopes Tab for a Session Clip.

On the left sits the Device chooser, used to pick a broad family of controls to operate on. What appears in the Device chooser shifts according to the clip's type:

- For an audio clip you'll see “Clip” (the sample controls belonging to that clip), each effect along the track's device chain, plus the mixer.
- For a MIDI clip the listing covers “MIDI Ctrl“ (its MIDI controller data), each device along the track's device chain, plus the mixer.

To its right is the Control chooser, which narrows down to the individual controls belonging to whatever you picked in the Device chooser. Across both menus, any parameter whose clip envelope has been edited shows an LED beside its label. To declutter either chooser, pick “Only show adjusted envelopes” from it.

With a Session clip selected in Clip View, a pair of toggles sits underneath the Device and Control choosers: Automation and Modulation. They let you flip between [automating and modulating](https://www.ableton.com/en/live-manual/12/clip-envelopes/#mixer-and-device-clip-envelopes) parameters on devices and the mixer. For Arrangement clips these toggles stay hidden, because Clip View permits only clip envelope modulation there. To bring automation envelopes to Arrangement clips, work instead on the track's [automation lane](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation).

Drawing and editing a clip envelope follows exactly the same procedure used for [automation envelopes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) over in the Arrangement View. To learn how Session View automation is captured, consult [Recording Automation in Session View](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#recording-automation-in-session-view).

Removing a clip envelope — that is, returning it to its default value — is done by right-clicking inside the Clip View's Envelope Editor, or by hitting the CtrlBackspace (Win) / CmdDelete (Mac) shortcut keys, to bring up its context menu, then choosing Clear Envelope.

If you want particular MIDI control messages to reset on their own each time a clip restarts, pick the “MIDI Envelope Auto-Reset” entry from either the Options menu or the Sample Editor's context menu.

We can now turn to a handful of practical applications for clip envelopes.

### 26.2 Audio Clip Envelopes

Clip envelopes carry Live's “elastic“ treatment of audio further still, and together with Live's audio effects they make Live a formidable sound-design instrument. Applied to audio clips, they let you spin countless intriguing versions of a single clip on the fly — ranging from gentle fixes all the way to wholly fresh, unrelated sounds.

### 26.2.1 Clip Envelopes are Non-Destructive

Clip envelopes let you sculpt fresh sounds out of a sample while leaving the file on disk untouched. Since Live works out the envelope modulations as it plays, a single Live Set can hold hundreds of clips that each sound distinct yet all draw on one shared sample.

Naturally, a sound you've just built can be saved out by [rendering](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#exporting-audio-and-video) or through [resampling](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips). Within the Arrangement View, the [Consolidate command](https://www.ableton.com/en/live-manual/12/arrangement-view/#consolidating-clips) lets you generate new samples.

### 26.2.2 Changing Pitch and Tuning per Note

Pull a sample loop out of the browser and drop it into Live, confirm the [Warp switch](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping) is on, then start the clip playing. Pick “Clip” in the Device chooser along with “Transposition” in the Control chooser. From here you're free to shift the pitch transposition of single notes within the sample while it plays back.

The quickest route is to switch on [Draw Mode](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-envelopes) and lay down steps that follow the grid. Turn Draw Mode back off whenever you need to tweak breakpoints and line segments — handy for softening the blocky steps by shifting breakpoints sideways.

The Transposition Envelope with Steps (Top) and Ramps (Bottom).

Keep in mind that your warp settings govern how faithfully Live's time-warping engine follows the contour of the envelope. For snappier tracking, lower the Grain Size value when in Tones or Texture Mode, or set a smaller Granulation Resolution while in Beats Mode.

When fine-tuning the pitch of single notes in the sample, hold the Shift modifier as you draw or reposition breakpoints to gain a finer resolution.

To move the display around, keep the CtrlAlt (Win) / CmdOption (Mac) modifier held while you drag.

The modulation applied to pitch works _additively_: the transposition envelope's output is just summed onto the value of the Transpose control. Whatever the modulation produces is then clamped so it remains within the permitted span (-48..48 semitones here).

### 26.2.3 Muting or Attenuating Notes in a Sample

Choose “Clip” in the Device chooser together with “Gain” in the Control chooser. Whether you lay steps down in Draw Mode or sculpt contours using breakpoints, you can stamp any volume shape you like onto the sample.

Imposing a Volume Envelope on a Sample.

Live reads the volume envelope's output as a relative percentage of wherever the Clip Gain slider currently sits. For that reason the clip envelope's modulation is never able to climb past the absolute volume setting, though it can pull the audible level all the way down to silence.

### 26.2.4 Scrambling Beats

A particularly inventive application of clip envelopes is modulating the sample offset. This kind of modulation is best suited to rhythmic material and is offered only for clips configured to play back in the Beats Warp Mode.

Give sample offset modulation a go using a one-bar drum loop: confirm Beats Mode is selected, then in the Envelopes tab pick “Clip“ from the Device chooser and “Sample Offset“ from the Control chooser. A vertical grid overlay shows up across the Envelope Editor. With the envelope's Draw Mode active, push steps to non-zero values and you'll hear the loop come apart. So what's actually happening?

Picture a tape head reading the audio, with the envelope steering where that head sits. As the envelope's value climbs, the head drifts further from its resting center. A positive envelope value pushes the head toward the “future,“ while a negative one pulls it back into the “past.“ Helpfully, Live measures this modulation in beats instead of centimeters: each vertical grid line stands for a sixteenth note of offset, and the modulation can swing from plus eight sixteenths down to minus eight sixteenths.

When you want to whip up engaging variations on beat loops in a hurry, sample offset modulation is the go-to. We'd steer you away from it for “analytical“ cut-and-splice jobs, though; those go far more smoothly in Live's Arrangement View, where the outcome can be consolidated into new clips without fuss.

Repeating Steps and Slowing Time with the Sample Offset Envelope.

Certain sample offset envelope gestures yield a signature result: a descending “escalator“ shape, say, essentially loops back the step found at the start of the envelope. In the same vein, a gentle downward-sloping ramp drags time out and yields pleasant smearing effects whenever the slope sits just shy of 45 degrees; give it a try at a 1/32 Granulation Resolution.

### 26.2.5 Using Clips as Templates

The more creatively you employ clip envelopes, the more the host clips take on a character all their own, detached from whatever sample they began with. Sooner or later you may ask yourself: how would this clip sound built around some other sample? Finding out is simple — select the clip so it shows in the Clip View, then drag whichever sample you want from the browser, or from the Session or Arrangement View, onto that Clip View. Every clip setting, the envelopes included, stays exactly as it was; the only thing swapped out is the sample.

### 26.3 Mixer and Device Clip Envelopes

You can press clip envelopes into service to _automate_ or _modulate_ mixer and device controls. Because such controls might be driven by both envelope types simultaneously (and on top of that by the Arrangement's [automation envelopes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation), some confusion can creep in. There is, though, one key respect in which modulation envelopes part ways with automation envelopes: an automation envelope fixes the absolute value a control holds at each moment, whereas a modulation envelope can merely nudge that already-set value. That distinction is what lets the two kinds cooperate smoothly even when they act on the same parameter. As a visual cue, automation envelopes are drawn in red and modulation envelopes in blue. On parameters that use knob controls, automation shifts the absolute position (the “needle”), while modulation shows up as the blue segment around the ring.

Suppose you've captured volume automation on an audio clip that steadily fades it out across four bars. Now what becomes of that fade-out once you add a modulation envelope that steadily lifts the mixer volume over those same four bars? Early on, the fade-out turns into a swell, since the modulation envelope keeps pushing the volume up as far as the automation envelope permits. Yet as soon as the falling automated value crosses paths with the rising modulation value, the fade-out kicks in, because automation drives the absolute control value — and with it the working range of the modulation envelope — downward.

Clips in the Session View offer both automation and modulation clip envelopes. Sitting below the envelope choosers, a toggle lets you flip between editing the automation and the modulation clip envelope for whatever parameter you've chosen. Over in the Arrangement, clips carry modulation envelopes alone, with their automation envelopes living on the track's [automation lane](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation).

Toggle Between Editing Automation and Modulation Envelopes.

Within a clip, any parameter carrying an automation envelope is flagged by a red LED in the Control chooser, and likewise a blue LED marks one carrying a modulation envelope. A parameter may show both a red and a blue LED at once, signaling that the clip is automating and modulating it together.

LEDs Indicate Existing Automation and Modulation Envelopes for the Selected Parameter.

### 26.3.1 Modulating Mixer Volumes and Sends

Take note that volume is in fact governed by two separate modulation envelopes: Clip Gain and Track Volume. That second one modulates the mixer's gain stage, so its effect lands on the post-effect signal. To keep things clear, a tiny dot beneath the thumb of the mixer's volume slider marks the genuine, modulated volume setting.

Mixer Volume Under Modulation. That Small Dot Sitting Beneath the Volume Slider Thumb Stands for the Modulated Volume Setting.

When you push the Volume slider up or down, watch the dot trail your motion in a relative manner.

Putting modulation on the track's Send controls is every bit as straightforward. Here too the modulation is a relative percentage: a clip envelope can't drive the send any higher than the Send knob allows, yet it can drop the real send value all the way to minus infinite dB.

A Send Under Modulation. On the Send Knob's Position Ring, the Blue Segment Marks the Modulated Value.

### 26.3.2 Modulating Pan

The Pan modulation envelope acts on the mixer pan stage relatively, with the pan knob's setting deciding how strong the modulation gets. Leave the pan knob centered and clip envelope modulation can swing the whole way from hard left to hard right; turn the knob toward either side and the modulation's range shrinks automatically. Push the pan knob fully to the left, for example, and the pan modulation clip envelope does nothing whatsoever.

### 26.3.3 Modulating Device Controls

Every device sitting on a clip's track shows up in the Device chooser. Modulating a device parameter proceeds much as modulating a mixer control does. While you do so, bear in mind how modulation and automation envelopes interact: a clip envelope, unlike a [device preset](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#using-devices), can't set outright values for a device's controls — it can only _shift_ them relative to whatever they're currently set to.

### 26.4 MIDI Controller Clip Envelopes

No matter whether your MIDI clip was just recorded straight into Live or pulled in from your own files, Live lets you build and revise the clip's MIDI controller data as clip envelopes.

Select “MIDI Ctrl“ in a MIDI clip's Device chooser, then turn to the adjacent Control chooser to home in on one particular MIDI controller. For any controller in the list you can draw fresh clip envelopes using steps or breakpoints. Beyond that, you can revise clip envelope versions of controller data that arrived inside your MIDI files or was laid down as you recorded new clips: controllers that already hold clip envelopes show their names with an LED right beside them in the Control chooser.

Live recognizes nearly all MIDI controller numbers through 119, which you reach using the scroll bar down the right edge of the menu. Bear in mind that whatever devices receive your MIDI controller messages might not honor the standard MIDI control assignments, so “Pitch Bend“ or “Pan,“ to name two, won't always do what their labels suggest.

A MIDI Controller Clip Envelope.

A good number of the methods covered in the upcoming section on detaching a clip envelope from its parent clip carry over nicely to MIDI controller clip envelopes too.

### 26.5 Unlinking Clip Envelopes From Clips

Each clip envelope is capable of holding its own local loop/region settings. Being able to detach an envelope from its clip opens up a wealth of thrilling creative avenues, a selection of which we'll walk through across the remainder of this chapter.

### 26.5.1 Programming a Fade-Out for a Live Set

Begin with an uncomplicated case. Picture yourself building a Live Set where you want an eight-bar fade-out to fire whenever one particular audio clip starts — except the only material on hand is a single one-bar loop.

Employing a Clip Envelope to Build a Fade-Out Across Several Passes of a Loop.

1. Pick either the Clip Gain or the Mixer Track Volume envelope, then _unlink_ it from the sample.
2. The clip envelope's loop braces take on color, signaling that this envelope now carries local loop/region settings of its own. Over in the Envelopes tab the loop/region controls “come to life.“ Flip the envelope's Loop switch and you'll see the Clip tab/panel's Loop switch stays put — the sample goes on looping even as the envelope plays back as a “one-shot.”
3. Enter “8“ in the leftmost box for the envelope's loop length.
4. Pull the envelope view fully out by clicking the Envelope's time ruler and dragging upward.
5. Drop a breakpoint where the region ends and pull it down to the bottom.

Play the clip now and you'll hear that one-bar loop fade away across eight bars.

### 26.5.2 Creating Long Loops from Short Loops

Now push the idea one notch further. Elsewhere in your set you'd like to reuse that very same one-bar loop — it sounds terrific — but hearing it repeat over and over wears thin. What you want is to stretch it into a longer loop somehow.

Pick up from the clip we just rigged to fade out across eight bars. Switch on the Loop switch of the clip volume envelope. Play the clip now and the eight-bar fade-out repeats. You're free to draw or reshape any envelope to lay over the sample loop. None of this is limited to volume, of course — it applies to any other control too; why not a filter sweep every four bars?

Keep in mind that the Envelope Editor lets you carve out as much time as you require, whether by hauling the loop braces past the edge of the view or by typing figures into the numeric region/loop controls.

For every envelope you're free to set whatever loop length you fancy, odd ones like 3.2.1 included. It's easy enough to picture serious intricacy (and bewilderment!) emerging once a single clip holds several envelopes of odd length.

The Sample (Left) and Envelope (Right) Start Marker.

Reining in that intricacy calls for a shared point of reference. The start marker pins down the spot from which sample or envelope playback sets off whenever the clip begins.

Be aware that, like envelope drawing itself, the start/end markers and the loop brace get quantized by the [zoom-adaptive grid](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid).

### 26.5.3 Imposing Rhythm Patterns onto Samples

Up to this point our discussion has centered on laying long envelopes over short loops. There are equally interesting uses that run in the opposite direction. Take a sample holding a song that stretches several minutes long. A clip could play that sample using a one-bar volume envelope loop, where the loop now behaves as a pattern that keeps “punching“ holes through the music — knocking out every third beat, say. You can surely picture other parameters such a pattern might modulate to intriguing effect.

### 26.5.4 Clip Envelopes as LFOs

For anyone drawn to sound synthesis, it can help to regard a clip envelope carrying a local loop as an LFO. That LFO runs locked to the project tempo, though you can equally pick a loop period quirky enough to leave the envelope out of sync. Hide the grid and you're able to set the clip envelope's loop start and end points free of any meter grid.

Between the [Stretch/Skew Envelope handles](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#stretching-and-skewing-envelopes) and the [automation shapes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#inserting-automation-shapes), you have the means to craft inventive LFO contours.

### 26.5.5 Warping Linked Envelopes

While Linked mode is active, clip envelopes react to whatever happens to the clip's Warp Markers. In practice this means dragging a warp marker stretches or compresses the clip envelope to match. On top of that, you can tweak Warp Markers right inside the envelope editor.

Clip Envelopes and Warp Markers Can Be Adjusted Together.
