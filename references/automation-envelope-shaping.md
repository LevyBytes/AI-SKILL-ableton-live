# Automation Envelope Shaping

Open when you need guidance on Automation Envelope Shaping in Ableton Live.

Context: [Drawing and Editing Automation](automation-and-editing-envelopes.md#255-drawing-and-editing-automation).

<a id="source-2551-drawing-envelopes"></a>
### 25.5.1 Drawing Envelopes

Once Draw Mode is switched on, a click-and-drag lets you “draw“ the shape of an envelope curve.

The Draw Mode Switch.

You can flip Draw Mode on or off through the Draw Mode item in the Options menu, by clicking the Control Bar’s Draw Mode switch, or by pressing B. Holding B down while you edit with the mouse flips Draw Mode just for that moment.

Drawing an Envelope.

Each drawn step spans the width of the grid you can see, and the grid itself can be [modified using a number of handy shortcuts](https://www.ableton.com/en/live-manual/12/arrangement-view/#using-the-editing-grid). Keep the Shift modifier pressed as you drag up or down and you can dial in a step's automation value with finer precision.

To draw freehand, switch the grid off with the Snap to Grid item in the Options menu or the Ctrl+4 (Win) / Cmd+4 (Mac) shortcut. If you'd rather keep the grid visible but draw freehand for a moment, hold Alt (Win) / Cmd (Mac) as you draw.

<a id="source-2552-editing-breakpoints"></a>
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

<a id="source-2553-stretching-and-skewing-envelopes"></a>
### 25.5.3 Stretching and Skewing Envelopes

The Handles Allow You to Stretch or Skew Envelopes.

Hover the cursor over a time selection and handles surface along its outer edges. By clicking and dragging those handles you can reshape the selected automation in these ways:

- Drag the top and bottom center handles to stretch the automation vertically. As you drag, a rectangle reports how much stretch you're applying. That rectangle latches onto the upper and lower boundaries and onto the points where its corners meet. Hold Shift for fine control over the stretch amount. Push past the boundaries and the envelope gets clipped.
  As a Handle Is Dragged, the Degree of Stretch or Skew Is Shown by a Rectangle.
- Drag the left and right center handles to stretch the automation horizontally. Any breakpoints lying outside the time selection that you drag across get wiped out. Hold Shift as you stretch and those breakpoints shift in proportion to how far the handle travels. Hold the Alt (Win) / Cmd (Mac) modifier during a horizontal drag to sidestep grid snapping.
- Drag any of the corner handles to skew the automation. A rectangle appears during the drag to show how much skew you're adding. It latches onto the upper and lower boundaries and onto where its corners meet. Hold Shift to fine-tune the degree of skew.
- Drag a handle with Alt (Win) / Option (Mac) held and the move is mirrored on the opposite handle, just as though you were dragging the pair at once in opposing directions.

<a id="source-2554-simplifying-envelopes"></a>
### 25.5.4 Simplifying Envelopes

Should your automation envelope be crowded with breakpoints — which often happens once you've recorded automation — the Simplify Envelope command comes in handy. It works out the smallest number of breakpoints that still captures the selected envelope, strips out any that aren't pulling their weight, and swaps in straight lines or curved segments wherever that fits.

The Simplify Envelope Command Removes Unnecessary Breakpoints.

Mark a time selection over the automation you'd like to tidy, then pick Simplify Envelope from the context menu.

<a id="source-2555-inserting-automation-shapes"></a>
### 25.5.5 Inserting Automation Shapes

Automation Shapes Inserted into an Envelope.

With automation shapes you can rapidly build intricate rhythmic automation patterns, and equally gentler, unhurried gestures such as swells, builds and drops.

A handful of ready-made automation shapes can be dropped onto a time selection. To place one, right-click the time selection and pick a shape out of the context menu.

The Two Rows Contain Different Types of Automation Shapes.

Automation shapes come in two kinds. The upper row offers a set of familiar waveforms: sine, triangle, sawtooth, inverse sawtooth and square. Once placed, each scales horizontally to fit the time selection and vertically to span the automated parameter range. Lacking a time selection, the shape instead scales horizontally to match the current grid size.

The lower row holds two sets of ramps plus an ADSR shape. Their behavior departs a little from the top row's: on insertion they tie into the automation value sitting before or after the selection, which their dotted line points out.

<a id="source-2556-locking-envelopes"></a>
### 25.5.6 Locking Envelopes

As a rule, when you reposition Arrangement View clips, Live carries all of the automation along with each clip. There are times, though, when you'd prefer the envelopes pinned to the song position instead of to the clips — that's exactly the job of the Lock Envelopes switch.

Locking envelopes is also available from the Options menu.

The Lock Envelopes Switch.
