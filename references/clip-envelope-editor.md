# Clip Envelope Editor

Open when you need guidance on Clip Envelope Editor in Ableton Live.

Context: [Clip Envelopes](clip-envelopes.md#26-clip-envelopes).

<a id="source-261-the-clip-envelope-editor"></a>
### 26.1 The Clip Envelope Editor

Begin editing clip envelopes by opening the Clip View's Envelopes tab — click its tab header (the one bearing the icon) within the Clip View. Inside the Envelopes tab sit two choosers that let you pick which envelope to display and modify.

The Clip View's Envelopes Tab for a Session Clip.

On the left sits the Device chooser, used to pick a broad family of controls to operate on. What appears in the Device chooser shifts according to the clip's type:

- For an audio clip you'll see “Clip” (the sample controls belonging to that clip), each effect along the track's device chain, plus the mixer.
- For a MIDI clip the listing covers “MIDI Ctrl“ (its MIDI controller data), each device along the track's device chain, plus the mixer.

To its right is the Control chooser, which narrows down to the individual controls belonging to whatever you picked in the Device chooser. Across both menus, any parameter whose clip envelope has been edited shows an LED beside its label. To declutter either chooser, pick “Only show adjusted envelopes” from it.

With a Session clip selected in Clip View, a pair of toggles sits underneath the Device and Control choosers: Automation and Modulation. They let you flip between [automating and modulating](https://www.ableton.com/en/live-manual/12/clip-envelopes/#mixer-and-device-clip-envelopes) parameters on devices and the mixer. For Arrangement clips these toggles stay hidden, because Clip View permits only clip envelope modulation there. To bring automation envelopes to Arrangement clips, work instead on the track's [automation lane](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation).

Drawing and editing a clip envelope follows exactly the same procedure used for [automation envelopes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) over in the Arrangement View. To learn how Session View automation is captured, consult [Recording Automation in Session View](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#recording-automation-in-session-view).

Removing a clip envelope — that is, returning it to its default value — is done by right-clicking inside the Clip View's Envelope Editor, or by hitting the Ctrl+Backspace (Win) / Cmd+Delete (Mac) shortcut keys, to bring up its context menu, then choosing Clear Envelope.

If you want particular MIDI control messages to reset on their own each time a clip restarts, pick the “MIDI Envelope Auto-Reset” entry from either the Options menu or the Sample Editor's context menu.

We can now turn to a handful of practical applications for clip envelopes.

<a id="source-262-audio-clip-envelopes"></a>
### 26.2 Audio Clip Envelopes

Clip envelopes carry Live's “elastic“ treatment of audio further still, and together with Live's audio effects they make Live a formidable sound-design instrument. Applied to audio clips, they let you spin countless intriguing versions of a single clip on the fly — ranging from gentle fixes all the way to wholly fresh, unrelated sounds.
