# Using Push 1 (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

The Melodic Sequencer + 32 Notes layout merges live performance with step entry in one view. Because it exposes several octaves alongside the steps on a single page, this arrangement works nicely for discovering the chords and harmonies you intend to program. It also handles extended phrases comfortably.

### 34.7.1 32 Notes

Use the lower portion of the pad grid to perform notes live and to mark which ones go into the step sequencer. Every pad maps to one of the pitches offered by whichever scale is active. Tap a pad and it becomes selected and sounds. A pad that is selected appears in a brightened shade of the track’s color.

If you want to mark a pad without sounding it, keep the Select button held down as you tap that pad.

What the pad colors mean is as follows:

- Blue — marks the root note of the scale.
- Blue-Green — marks a pad that is selected.
- Green — marks a pad that is sounding right now.
- White — a note belonging to the scale that is not the root.

Tapping the Octave Up or Down button moves the band of notes you can reach. If you keep the Shift key held while you drag the touch strip, the band moves by whole octaves. Holding Shift as you tap the Octave buttons instead nudges the band by a single scale step. While you change it, the display flashes the range that is currently reachable.

Just like the 64 Notes layout, you can retune the notes shown in the lower half of the pad grid through the [Scale menu](https://www.ableton.com/en/live-manual/12/using-push-1/#playing-in-other-keys).

### 34.7.2 Sequencer

When you tap a step in the upper portion of the pad grid, every note you have selected is written into that step. A step that holds notes shows up in a blue color.

Keep a step held to see which notes it holds; those notes appear across the lower portion of the pad grid in a blue-green color. Tap any one of these selected notes to clear it out of the step.

Hold several steps at once and the selected notes are written into all of them. With Duplicate held, tap a step to grab the notes it contains, then tap a different step to drop them into a fresh spot in the step sequencer. Be aware that this does not clear out whatever notes already sit in the target page; instead the copied notes are layered over them. If you want them gone first, hold Delete and tap that page’s loop length pad.

Within the step sequencer, here is what the pad colors signify:

- Blue — a step holding a note.
- Green — a step that is sounding right now.
- White — a step that is selected.
- Dull Yellow — a step that holds a note whose note is muted.
- Gray — an empty pad.
- Light Red — when triplets are picked as the step size, the rightmost two columns of pads stay dark. Those pads do nothing in that case; only the leading six pads of each step row remain usable.

If you leave the sequencer at its default 16th note resolution, you get two pages of steps on hand simultaneously, which adds up to two bars. To set the loop length and reach further step sequencing pages, use the [loop length pads](https://www.ableton.com/en/live-manual/12/using-push-1/#adjusting-the-loop-length). You can briefly summon the loop length pads into the fifth row by keeping the Note button held.

It is also possible to pin the loop length pads so they stay put. For that, hold Shift and tap the Note button. Keep in mind that Push 1 stores this locked-or-unlocked condition per track. Tapping the Note button once more releases the loop length pads.

To copy a whole sequencer page, hold Duplicate, tap the loop length pad belonging to the source page, then tap the loop length pad of the page you want it copied to. Be aware that this does not clear out whatever notes already sit in the target page; instead the copied notes are layered over them. If you want them gone first, hold Delete and tap that page’s loop length pad.

### 34.8 Navigating in Note Mode

Having made a handful of tracks already, you are free to keep adding others. Often, though, you will want to jump among the tracks that already exist so you can keep developing musical ideas on those instruments and devices. That is exactly what the Arrow Keys are for.

Arrow Keys.

Use the Left/Right Arrows to step from track to track. Keep in mind that picking a MIDI track on Push 1 arms it for you on its own, letting you play it at once. Over in Live, the track Arm buttons turn pink to signal that selection is what armed them.

Pink Track Arm Button.

What the Up/Down Arrows actually do hinges on the Workflow mode, which you configure under Push 1’s [User Preferences](https://www.ableton.com/en/live-manual/12/using-push-1/#setting-user-preferences). Either way, the Up/Down Arrows shift you by exactly one scene. Under Scene Workflow, the scene you land on is launched. Under Clip Workflow, only the clip on the chosen track fires; clips on other tracks stay untouched.

Moving with the Up/Down Arrows while in Note Mode kicks off playback at once, and the clip you trigger picks up the play position from whichever clip had been running on that track previously. This matches what you would get if the clips were configured for [Legato Mode](https://www.ableton.com/en/live-manual/12/launching-clips/#legato-mode) inside Live.

### 34.9 Controlling Live’s Instruments and Effects

Tap the Device button to switch Push 1 into Device Mode, where Push 1’s encoders are handed control over the parameters inside Live’s devices.

Device Button.

While Device Mode is active, you pick devices on the track you have chosen using the Selection Control buttons, and the State Control buttons switch that device on or off. Whichever device is chosen carries an arrow beside it in the display.

Device Mode Settings.

With the In and Out buttons you can reach further devices and parameters that are not surfaced straight away.

In and Out Buttons.

Reach the following through these buttons:

- Further banks of parameters (for effects carrying more than a single bank).
- Further device chains inside Racks that hold more than a single chain.

### 34.10 Mixing with Push 1

If you want the encoders to drive volumes, pans, or sends across as many as eight tracks at once, tap the matching button on Push 1. Keep Shift held as you turn the encoders to get fine-tune resolution.

Volume and Pan & Send Buttons.

While Volume Mode is active, the encoders set track volume.

Tapping the Pan & Send button over and over steps through pans plus whatever number of sends exist in your Live Set.

Tap Push 1’s Track button to switch on Track Mode.

Track Button.

Under Track Mode, the encoders handle volume, pan, and the first six sends belonging to the chosen track. Use the Selection Control buttons to decide which track Track Mode acts on.

Selecting Tracks in Track Mode.

Tap the Master button to pick the Main track.

Keep a Group Track’s Selection Control button held to fold or unfold that track.

Bear in mind that with [Split Stereo Pan Mode](https://www.ableton.com/en/live-manual/12/mixing/#the-live-mixer) turned on during Pan & Send Mode, the display still reports the present pan value yet the pan dial is switched off. Under Track Mode, the display presents either the pan control or the stereo pan sliders, according to which pan mode is in force.

### 34.11 Recording Automation

Any adjustments you make to device and mixer parameters can be captured into your clips as automation, letting the sound evolve as the clip runs. Tap Push 1’s Automation button to begin recording automation.

Automation Button.

Doing so flips Live’s Session Automation Arm button, so the moves you make on Push 1’s encoders are written into the clip. Once you have finished recording parameter moves, tap the Automation button once more to switch it back off. Should you want to erase what you recorded for one parameter, keep the Delete button held and touch the encoder that goes with it. When no automation exists yet for a parameter, holding Delete and touching its encoder instead returns that parameter to its default value.

A parameter that carries automation appears with a rectangle beside its name in the display. Parameters you have overridden — by tweaking them by hand while not recording — display their value enclosed in brackets.

Automated and/or Overridden Parameters are Indicated in the Display.

If you want to switch every manually overridden automation back on, keep Shift held and tap the Automation button.

### 34.12 Step Sequencing Automation

Within either the drum or the melodic step sequencer, you are able to automate parameters for whichever step is chosen.

Which parameters you get varies with the display mode you happen to be in at the moment, as the sections that follow describe.

### 34.12.1 Note-Specific Parameters

No matter which sequencing layout you use while in Clip Mode, the note settings of every step are yours to change. Just keep a step held to reach those settings. At that point the display swaps its controls over to that step’s note settings.

Hold a Step to Adjust Note and Automation Parameters.

From there you turn the matching encoders so as to:

- Nudge notes earlier or later in time. The figure stands for the percentage by which the note sits away from the grid line before it. A negative figure means the note lands ahead of the grid line.
- Set the coarse Length for the chosen notes.
- Refine that length tweak for the chosen notes
- Alter the Velocity of the chosen notes.

These note-specific parameters can be set across several steps together as well. For that, keep every pad you wish to change held down, then work the encoders. The display then reports the spread of values across the chosen steps.

With Multiple Steps Selected, the Display Shows the Range of Parameter Values.

You can likewise lay down notes carrying the Nudge, Length, and Velocity values you want by holding an empty step and then working any of these encoders.

While dealing with drums, you can set nudge, length, and velocity for _every_ note that a given pad triggers: hold the Select button down, tap the pad, and then turn the encoders.

Holding Select While Pressing a Drum Pad Lets You Tweak Every Note that Pad Plays.

Within either the drum or melodic step sequencer, a step can be copied — together with all of its note-specific parameters — and dropped onto a different step. For that, hold Duplicate and tap the step you want to grab. Next tap the target step and let go of Duplicate.

### 34.12.2 Per-Step Automation

While you are in Device Mode or Volume Mode, hold one step or several to make and edit device or mixer automation that affects just the held step or steps. As you hold a step and turn an encoder, that parameter’s automation value is changed only for the slice of time that step stands for. Keep in mind that per-step automation works on any step, even one that holds no notes.

### 34.13 Controlling Live’s Session View

Tap Push 1’s Session button to move from Note Mode over to Session Mode. Holding the Session button down flips into Session Mode only for as long as you hold it. Let the button go and you drop back to Note Mode. In the same way, holding Note down during Session Mode flips momentarily into Note Mode.

Session Button.

Under Session Mode, the 8x8 pad grid now fires clips while the Scene/Grid Buttons fire scenes. Tapping a pad launches the clip sitting in the matching spot of Live’s Session View. When the track is chosen, tapping the button captures a fresh clip.

The pads glow in assorted colors to keep you informed:

- Whatever color a non-playing clip has in your Live Set shows up on its pad.
- Clips that are playing throb from green to white.
- Clips that are recording throb from red to white.

To halt all sound on a track, switch on Stop Mode and tap that track’s State Control button.

Stopping Clip Playback.

To halt every clip, keep Shift held and then tap Stop.

Push 1 reports back what the software is doing, but, just as importantly, the software mirrors what the hardware is up to. Live marks the clip slots that Push 1’s pad grid is steering at the moment with a colored border.

Together the directional arrows and the Shift button widen the reach of the eight-by-eight grid.

- Tapping Up or Down shifts you a single scene up or down. Keep Shift held as you hit Up or Down to jump eight scenes at a time. The Octave Up and Down buttons likewise move you eight scenes per press.
- The Left and Right arrow keys shift you a single track left or right. Keep Shift held as you hit Left or Right to jump eight tracks at a time.

### 34.13.1 Session Overview

With Push 1’s Session Overview you can move around big Live Sets fast and never glance at your computer screen. Keep the Shift button held and the pad grid pulls back to show a bird’s-eye view of your Session View. Inside the Session Overview, a single pad stands for an eight-scene-by-eight-track block of clips, which yields a grid of 64 scenes by 64 tracks. Tap a pad to zero in on that part of the Session View. As an example, holding Shift and then tapping the pad at row three, column one focuses you on scenes 17-24 and tracks 1-8. On top of that, with Shift held each scene launch button stands for a block of 64 scenes, where your Set has them.

Inside the Session Overview, the colors are coded slightly differently:

- Amber: points to the block of clips currently chosen, the one the software wraps in the colored border.
- Green: clips are sounding somewhere in that block of clips (though it need not be the block that is chosen).
- Red: nothing is sounding anywhere in that range.
- No color: that range holds no tracks or scenes at all.

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

### 34.15 Push 1 Control Reference

What every section and control does is laid out underneath.

#### 34.15.0.1 Focus/Navigation Section

Focus/Navigation Section.

Note Mode — Once picked, the Pad Section retools its behavior to suit the kind of track that is chosen at the moment:

- MIDI track containing an instrument — the pads sound notes. Tapping Note again and again flips back and forth between real-time playing and melodic step sequencing.
- MIDI track containing a Drum Rack — the Pad Section splits up; the lower-left 16 pads sound the Drum Rack, the lower-right 16 pads set the clip’s loop length, and the top four rows run the step sequencer. Tap Note once more to flip into 64-pad mode, which lets you play drums over the full 8x8 pad grid.

Session Mode — Once picked, the Pad Section shifts to firing clips in Live’s Session View.

Shift — Keep Shift held as you tap other buttons to reach extra functionality.

Arrow Keys — Travel across your Live Set (under Session Mode) and from track to track or scene/clip to scene/clip (under Note Mode).

Select — Under Session Mode, hold Select and tap a clip to choose that clip without firing it. The clip’s name also turns up in the display. Under Note Mode, hold Select and tap a Drum Rack pad to choose its notes without sounding the pad.

#### 34.15.0.2 Add Section

Add Section.

These buttons drop fresh devices or tracks into your Live Set.

Add Effect — Brings up Browse Mode so a fresh device lands to the right of whichever device is chosen. Hold Shift as you tap Add Effect to place the fresh device to the left of the chosen device instead. For a MIDI Effect, first pick the instrument on a track. Then hold Shift as you tap Add Effect.

Add Track — Spawns a fresh MIDI track to the right of whichever track is chosen. Keep Add Track held to pick another kind of track to drop in, namely Audio, MIDI, or Return. Should you tap the Add Track button while a track inside a Group Track is chosen, any fresh tracks go into that Group Track.

#### 34.15.0.3 Note Section

Note Section.

These buttons shape the way notes get played on Push 1.

Scales — With Note Mode on and an instrument track chosen, tapping this button lets you pick which scale the pads will play. Bear in mind this button does nothing while a Drum Rack track is chosen or while you are in Session Mode.

- Fixed Y/N: With Fixed Mode on, the pad grid’s notes hold their positions even as you switch keys; the bottom-left pad plays C every time, apart from keys lacking a C, where the bottom-left pad plays whichever note in the key sits closest. With Fixed off, the pad grid’s notes slide so the bottom-left pad forever plays the root of the chosen key.
- In Key/Chromatic: With In Key picked, the pad grid is in effect “folded” so that only the key’s notes show up. Under Chromatic Mode, the pad grid carries every note. Notes belonging to the key are lit, whereas notes outside the key stay unlit.
- Scale selection: Pick the base scale using the up/down buttons over on the lefthand side.

User — Every bit of Push 1’s built-in functionality can be switched off through User Mode. This lets Push 1 be reprogrammed to drive other functions in Live or in different software. Keep the User button held to open a range of configuration options. Push 1’s relative encoders run best under “Relative (2’s Comp.)” mode. To make sure that mode is picked, rotate the encoder slowly leftward as you map.

Repeat — With Repeat on, keeping a pad held retriggers the note. The Scene/Grid buttons set the rhythmic value of that repeated note.

Accent — With Accent on, every arriving note — whether step sequenced or played live — sounds at full velocity. Keep Accent held to switch it on only briefly.

Octave Up/Down — With an instrument track chosen, these buttons move the pads an octave up or down. With a Drum Rack chosen, these buttons move the Drum Rack’s pad overview up or down by 16 pads. Under Session Mode, these buttons move Session View control up or down by eight scenes. These buttons stay unlit when no further octaves exist.

#### 34.15.0.4 State Control Section

State Control Section.

While you deal with tracks, the eight leftmost buttons will stop clips, or mute, or solo the matching track, according to which of the three rightmost buttons you tap (Stop, Mute, or Solo). While you deal with devices in place of tracks, those eight leftmost buttons switch devices on and off. These buttons take on extra functionality under other modes, scale selection being one example.

To halt every clip, keep Shift held and then tap Stop.

#### 34.15.0.5 Selection Control Section

Selection Control Section.

These buttons operate alongside the Display/Encoder Section buttons and decide which parameters the encoders can edit and the display can show. The In and Out buttons get you into devices nested in Racks or into further parameter banks on devices carrying more than eight parameters. Under Browse Mode, the In and Out buttons slide the display rightward or leftward, letting you dig through deeper layers of subfolders or take in a greater count of presets on the display.

#### 34.15.0.6 Display/Encoder Section

Display/Encoder Section.

The half-dozen buttons sitting to the display’s right set the encoders’ editing mode. Across every mode, the ninth encoder governs the volume of the Main track, or the Pre-Cue volume while Shift is held. Keeping Shift held as you turn any of the first eight encoders lets you fine-tune whatever parameter that encoder is steering at the moment. Bear in mind you can flip briefly to another editing mode by keeping the matching button held. Let the button go and you drop back to the prior mode.

Volume Mode.

Under Volume Mode, the encoders govern the volume of the eight chosen tracks.

Pan & Send Mode.

Under Pan & Send Mode, a single press governs pans. Each press after that steps through the sends.

Track Mode.

Under Track Mode, the encoders govern volume, pan, and the first six sends of the chosen track. Decide which clip track to govern through the eight Selection Control buttons. Tap the Master button to pick the Main track.

Under Clip Mode, the encoders govern assorted parameters for the chosen clip. Which parameters appear hinges on the kind of clip chosen:

Clip Mode With a MIDI Clip Selected.

- Loop Start (or Clip Start if Loop is off)
- Position
- Loop Length (or Clip End if Loop is off)
- Loop On/Off
  Clip Mode With an Audio Clip Selected.
- Loop Start (or Clip Start if Loop is off)
- Position
- Loop Length (or Clip End if Loop is off)
- Loop On/Off
- Warp Mode
- Detune
- Transpose
- Gain
  Device — The encoders govern the parameters of the chosen device.Browse — The encoders move through the devices and presets on offer.

#### 34.15.0.7 Tempo Section

Tempo Section.

Tap Tempo — Press it once per beat and the Live Set’s tempo tracks your tapping. With the “Start Playback with Tap Tempo” button turned on under Live’s Record, Warp & Launch Settings, your tapping can also serve as a count-in: in a 4/4 signature, four taps are needed before song playback kicks off at the tapped tempo.

Metronome — Switches Live’s metronome on or off.

The left encoder nudges Live’s tempo by one BPM per step. Keeping Shift held while you turn it instead nudges the tempo by .1 BPM per step.

The right encoder dials in how much swing is applied during Quantizing, Record Quantizing, or whenever Repeat is tapped.

#### 34.15.0.8 Edit Section

Edit Section.
