# Push 1 User Preferences

Open when you need guidance on Push 1 User Preferences in Ableton Live.

Context: [Using Push 1](push-one-setup-and-playing-routes.md#34-using-push-1).

<a id="source-3414-setting-user-preferences"></a>
### 34.14 Setting User Preferences

Keep the User button held to tune how responsive Push 1’s velocity is, along with aftertouch and further settings.

User ButtonUser Settings

Pad Threshold fixes the gentlest playing force that still fires notes. Raising the setting demands more force. Be aware that with lower settings, notes can fire by accident and pads may “stick” on.

Velocity Curve governs how the pads react to differing amounts of force, spanning from Linear — a one-to-one tie between striking force and note velocity — through assorted logarithmic curves. Bigger Log values hand you wider dynamic range while playing softly. Gentler playing styles can gain from bigger Log values. The diagram underneath illustrates the assorted velocity curves, plotting striking force along the horizontal axis and note velocity along the vertical axis.

Diagram of Push 1’s Velocity Curves.

The Workflow option settles how Push 1 reacts when you tap the Duplicate, New, or Up/Down arrow buttons. The mode you pick comes down to the way you prefer to arrange your musical ideas. Under Scene Workflow — the default — musical ideas are arranged and traversed by scene. Under Clip Workflow, you deal only with whichever clip is chosen at the moment.

Under Scene Workflow:

- Duplicate makes a fresh scene holding every clip that is playing right now, then smoothly carries on playing them. It matches the [Capture and Insert Scene command](https://www.ableton.com/en/live-manual/12/session-view/#editing-scenes) found in Live’s Create menu.
- New behaves just like Duplicate, save that it does _not_ copy whichever clip is chosen. In its place, an empty clip slot is readied so you can begin a new idea on the current track.
- The Up/Down Arrows step a single scene up or down. The clips in the new scene start playing smoothly.

Under Clip Workflow:

- Duplicate puts a copy of the chosen clip into the next clip slot, while clips already playing on other tracks keep running. Hold Shift as you tap Duplicate to instead build a fresh scene holding every clip that is playing right now.
- New readies an empty clip slot on the track that is chosen. Clips on other tracks stay untouched.
- the Up/Down Arrows step a single scene up or down. The chosen track’s clip in the new scene starts playing smoothly. Clips on other tracks stay untouched.

Aftertouch Threshold fixes the smallest arriving aftertouch value (from 0-127) that Push pays attention to. Anything coming in beneath this level is dropped, while anything coming in above it is stretched across the whole aftertouch range. As an example, suppose the Aftertouch Threshold sits at 120; playing with an aftertouch reading of 119 produces no result. Yet incoming values from 120 through 127 are stretched to yield an output from 0 to 127, like so:

120 -> 0
121 -> 18
122 -> 36
123 -> 54
124 -> 72
125 -> 90
126 -> 108
127 -> 127

<a id="source-3415-push-1-control-reference"></a>
### 34.15 Push 1 Control Reference

What every section and control does is laid out underneath.
