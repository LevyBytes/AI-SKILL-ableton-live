# Automation And Editing Envelopes

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 25. Automation and Editing Envelopes

As you operate Live’s mixer and devices, there are frequently moments where you'd like the way you move a control to be captured as part of the track itself. We call this _automation_: the path a control traces over the song timeline or a Session clip, and a control whose setting shifts over that span is described as _automated_. Nearly every mixer and device control in Live, the song tempo among them, supports this.

### 25.1 Recording Automation in Arrangement View

There are two routes for capturing automation into the Arrangement View:

1. By adjusting parameters by hand as you lay down fresh material straight into the Arrangement.
2. By capturing a Session View performance [into the Arrangement](https://www.ableton.com/en/live-manual/12/session-view/#recording-sessions-into-the-arrangement), provided the Session clips hold automation.

Throughout Session-to-Arrangement recording, any automation held in Session clips is _always_ committed to the Arrangement, and the same goes for hand-made parameter tweaks on tracks captured from the Session.

As you cut new material directly into the Arrangement, it's the Automation Arm button that decides whether your manual parameter moves get captured.

The Automation Arm Button.

With Automation Arm enabled, every move you make on a control while the Control Bar’s Arrangement Record button is active turns into Arrangement automation. Give it a go by automating a control — say, a mixer volume slider. Once you've recorded, replay the take so you can watch and listen to what that control move did. Notice that a small LED now shows up in the slider thumb, signalling that the control carries automation. Repeat the experiment with track panning and the Track Activator switch; for those, the automation LEDs sit in their upper left corners.

Volume, Pan and the Track Activator Switch Have Been Automated.

### 25.2 Recording Automation in Session View

Session View clips can capture automation too. The procedure goes like this:

Controls for Recording Session Automation.

1. Switch on the Automation Arm button so the session is set up for automation capture.
2. Turn on the Arm button for whichever tracks you intend to record onto. Clip Record buttons then show up in the vacant slots of those armed tracks.
3. Press the Session Record button to kick off automation capture.

You can equally lay automation down into _all_ Session clips currently playing, whether or not their tracks happen to be armed. The route for this is the Session Automation Recording switch found in the Record, Warp & Launch Settings.

The Session Automation Recording Preference.

That lets you, say, overdub Session automation onto an existing MIDI clip while leaving the clip's notes untouched.

Whenever Session View clips get recorded or copied across into Arrangement View, their automation turns into track-based automation.

### 25.2.1 Session Automation Recording Modes

How automation gets captured changes according to the way you manipulate parameters during recording. If you're working with the mouse, the capture halts the instant you release the mouse button — a number of editing programs label this “touch” behavior. Should you instead turn knobs or move faders on a MIDI controller, the capture keeps going for as long as you're moving the controller. After you release it, recording carries on through to the close of the clip’s loop and then “punches out” on its own. Various applications call this “latch” behavior.

### 25.3 Deleting Automation

To wipe every bit of automation data, right-click an automated control so its context menu opens and pick Delete Automation, or use the CtrlBackspace (Win) / CmdDelete (Mac) shortcut keys. With that, the automation LED vanishes and the control holds one fixed value right across the whole Arrangement timeline and within any Session View clips. Particular stretches of automation can also be removed by [editing breakpoint envelopes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation).

### 25.4 Overriding Automation

It's common to want to audition fresh control moves while leaving the automation already sitting in the Arrangement intact. Granted, with [infinite Undo](https://www.ableton.com/en/live-manual/12/editing-midi/#non-destructive-editing) nothing is ever permanent, yet there's a simple way to switch a control’s automation off for the moment so existing data stays safe: alter the value of an automated control when you're not recording, and its automation LED switches off to show that automation has gone inactive. The current hand-set value has, in effect, _overridden_ whatever automation was there.

Whenever any of the automated controls within your Live Set sit in this inactive state, the Control Bar’s Re-Enable Automation button illuminates.

The Re-Enable Automation Button.

That button does two jobs. First, it flags that the controls right now sit in a state that diverges from what's stored in your Session clips or the Arrangement; second, clicking it switches all automation back on, restoring the controls to the automation that was committed “on tape.“

A single parameter can be re-enabled on its own through the Re-Enable Automation entry in that parameter's context menu. Within the Session View, overridden automation comes back simply by relaunching whichever clip holds the automation.

### 25.5 Drawing and Editing Automation

Both within the Arrangement View and inside Session View clips, automation is shown and reshaped as breakpoint envelopes.

The way envelope editing operates in the Arrangement runs as follows:

Automation Envelopes in the Arrangement View.

1. To reveal automation envelopes, turn on Automation Mode either by clicking the toggle button sitting above the track headers or via the A shortcut for that View menu item. Bear in mind that the same toggle button, or pressing A once more, switches Automation Mode back off.
2. A click on any of a track’s mixer or device controls brings that control’s envelope up on the clip track.
3. Within the track’s main automation lane, envelopes render “on top of“ whatever audio waveform or MIDI display is there — handy when you need breakpoints to line up against the track’s audio or MIDI material. Vertically, an envelope plots the control value, while horizontally it plots time. With switches and radio buttons, the value axis becomes “discrete”, which is to say it deals in non-continuous values (on/off, for example).
4. The Device chooser picks either the track mixer, one of that track’s devices, or “None“ to conceal the envelope. It additionally gives you a quick read on which devices carry automation, flagging each with an LED beside its label. For even more clarity, choose “Show Automated Parameters Only“ down at the bottom of the chooser.
5. From whichever device the Device chooser has selected, the Automation Control chooser then picks an individual control. Automated controls are marked by an LED on their labels.
6. The button shifts the envelope down into a dedicated automation lane beneath the clip. From there you can pick a further automation parameter in the choosers to display the two at once. Pressing the button with Alt (Win) / Cmd (Mac) held shifts the chosen envelope — plus every automated envelope — into separate automation lane(s) under the clip. Whenever the Device chooser reads “None“, this button stays hidden.
7. The button conceals the automation lane it belongs to. Keep in mind that tucking a lane out of sight does not switch its envelope off. Click the button with Alt (Win) / Cmd (Mac) held and it deletes the chosen automation lane along with every automation lane that follows it in that track.
8. The toggle shows up once an envelope has been shifted into a lane of its own. With it you can reveal or conceal all the extra automation lanes.

A right-click on an automation lane header brings up a context menu carrying further envelope-viewing choices. That same menu holds commands for swiftly clearing every automation envelope belonging to the track or to any of its devices.

The left arrow key takes you from an automation lane back up to the main track, folding all the automation lanes in the process. Pressing left and right arrow keys on a main track folds and unfolds its automation lanes.

Details on editing automation for Session View clips live in the [Clip Envelopes chapter](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes).

### 25.5.1 Drawing Envelopes

Once Draw Mode is switched on, a click-and-drag lets you “draw“ the shape of an envelope curve.

The Draw Mode Switch.

You can flip Draw Mode on or off through the Draw Mode item in the Options menu, by clicking the Control Bar’s Draw Mode switch, or by pressing B. Holding B down while you edit with the mouse flips Draw Mode just for that moment.

Drawing an Envelope.

Each drawn step spans the width of the grid you can see, and the grid itself can be [modified using a number of handy shortcuts](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid). Keep the Shift modifier pressed as you drag up or down and you can dial in a step's automation value with finer precision.

To draw freehand, switch the grid off with the Snap to Grid item in the Options menu or the Ctrl4 (Win) / Cmd4 (Mac) shortcut. If you'd rather keep the grid visible but draw freehand for a moment, hold Alt (Win) / Cmd (Mac) as you draw.

### 25.5.2 Editing Breakpoints

Once Draw Mode is off, the envelope behaves and appears in another way. Now the line segments, together with the breakpoints joining them, turn into objects you can drag. Click and drag across the envelope’s background and that marks out a selection. Editing breakpoints proceeds like this:

- Click somewhere along a line segment and a fresh breakpoint is born at that spot.
- Double-click any part of the envelope display that isn't sitting on a line segment to spawn a new breakpoint there.
- Click a breakpoint and it's gone.
- So you can edit breakpoints at speed, automation values pop up as you make, hover above, or drag one. Bear in mind that while you hover over or drag a selected line segment, the value shown belongs to whichever breakpoint sits nearest the cursor.
  A Breakpoint’s Automation Value.
- Drag a breakpoint with the mouse to reposition it wherever you like. Should the one you're dragging belong to the present selection, every other breakpoint in that selection moves right along with it. As you drag, a slim black vertical line surfaces so you can gauge your breakpoint's placement against the grid lines.
- Right-click a breakpoint and pick Edit Value from the context menu. From there you type an exact figure into the editable field with your computer keyboard. When several breakpoints are selected, the move applies to them all relatively. In much the same way, right-click a preview breakpoint and pick the Add Value command to spawn fresh breakpoints at a precise value.
- Click just beside (not directly on) a line segment, or hold Shift and click straight onto it, to select that segment. Keeping the left mouse button down, drag the segment to wherever you want it. If the segment you're moving falls inside the present time selection, Live drops breakpoints at the selection’s edges and the whole segment travels as one.
  To Move all Breakpoints Within the Selection, Drag Any One of Them.
- Any breakpoint placed near a grid line latches onto it automatically. To sidestep that snapping, hold the Alt (Win) / Cmd (Mac) modifier as you drag sideways.
- Breakpoints and line segments latch onto the time positions of neighboring breakpoints. To clear a neighboring breakpoint, keep dragging a breakpoint or line segment sideways “over” it.
- As you relocate a line segment or breakpoint, holding Shift while dragging confines the move to just the horizontal or just the vertical axis.
- With the Shift modifier held during a vertical drag, you can tune the value of a breakpoint or line segment at a finer resolution.
- Hold Alt (Win) / Option (Mac) and drag a line segment to bend it into a curve. A double-click with Alt (Win) / Option (Mac) held snaps the segment back to straight.
  A Curved Envelope Segment.

### 25.5.3 Stretching and Skewing Envelopes

The Handles Allow You to Stretch or Skew Envelopes.

Hover the cursor over a time selection and handles surface along its outer edges. By clicking and dragging those handles you can reshape the selected automation in these ways:

- Drag the top and bottom center handles to stretch the automation vertically. As you drag, a rectangle reports how much stretch you're applying. That rectangle latches onto the upper and lower boundaries and onto the points where its corners meet. Hold Shift for fine control over the stretch amount. Push past the boundaries and the envelope gets clipped.
  As a Handle Is Dragged, the Degree of Stretch or Skew Is Shown by a Rectangle.
- Drag the left and right center handles to stretch the automation horizontally. Any breakpoints lying outside the time selection that you drag across get wiped out. Hold Shift as you stretch and those breakpoints shift in proportion to how far the handle travels. Hold the Alt (Win) / Cmd (Mac) modifier during a horizontal drag to sidestep grid snapping.
- Drag any of the corner handles to skew the automation. A rectangle appears during the drag to show how much skew you're adding. It latches onto the upper and lower boundaries and onto where its corners meet. Hold Shift to fine-tune the degree of skew.
- Drag a handle with Alt (Win) / Option (Mac) held and the move is mirrored on the opposite handle, just as though you were dragging the pair at once in opposing directions.

### 25.5.4 Simplifying Envelopes

Should your automation envelope be crowded with breakpoints — which often happens once you've recorded automation — the Simplify Envelope command comes in handy. It works out the smallest number of breakpoints that still captures the selected envelope, strips out any that aren't pulling their weight, and swaps in straight lines or curved segments wherever that fits.

The Simplify Envelope Command Removes Unnecessary Breakpoints.

Mark a time selection over the automation you'd like to tidy, then pick Simplify Envelope from the context menu.

### 25.5.5 Inserting Automation Shapes

Automation Shapes Inserted into an Envelope.

With automation shapes you can rapidly build intricate rhythmic automation patterns, and equally gentler, unhurried gestures such as swells, builds and drops.

A handful of ready-made automation shapes can be dropped onto a time selection. To place one, right-click the time selection and pick a shape out of the context menu.

The Two Rows Contain Different Types of Automation Shapes.

Automation shapes come in two kinds. The upper row offers a set of familiar waveforms: sine, triangle, sawtooth, inverse sawtooth and square. Once placed, each scales horizontally to fit the time selection and vertically to span the automated parameter range. Lacking a time selection, the shape instead scales horizontally to match the current grid size.

The lower row holds two sets of ramps plus an ADSR shape. Their behavior departs a little from the top row's: on insertion they tie into the automation value sitting before or after the selection, which their dotted line points out.

### 25.5.6 Locking Envelopes

As a rule, when you reposition Arrangement View clips, Live carries all of the automation along with each clip. There are times, though, when you'd prefer the envelopes pinned to the song position instead of to the clips — that's exactly the job of the Lock Envelopes switch.

Locking envelopes is also available from the Options menu.

The Lock Envelopes Switch.

### 25.5.7 Edit Menu Commands

As you handle automation data in the Arrangement View, a number of Edit menu commands act in distinct ways according to whether your selection sits in the clip track or in its automation lanes.

When Cut, Copy, Duplicate or Delete is run on an envelope selection confined to one lane, only that envelope is touched. The clip and any other automation falling within that time selection stay as they were. Working across envelopes in several lanes at the same time is possible too.

Should you want your edits to reach both the clip and all the envelopes tied to it, make certain the Lock Envelopes switch is off and direct your edit commands at a selection within the clip track.

It's worth noting that Live lets you copy and paste envelope moves across time and also from one parameter onto a different one. Because those parameters might bear no relation to each other, the outcome can be surprising — though sometimes intriguing.

### 25.5.8 Editing the Tempo Automation

Among Live’s hallmark strengths is its knack for stretching and compressing audio on the fly to chase any tempo or shift in tempo. As far as Live is concerned, the song tempo is simply one more automated control.

To work on the song tempo envelope, expand the Main track within Arrangement View, then set the top envelope chooser to “Mixer“ and the bottom one to “Song Tempo“.

The Tempo Envelope.

While you shape the tempo envelope, you may wish to rescale how the value axis reads — that's what the pair of value boxes beneath the envelope choosers are for: the left one fixes the minimum and the right one the maximum tempo on display, given in BPM.

Keep in mind that these same two controls also govern the [value range of a MIDI controller](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-remote-control) mapped to the tempo.
