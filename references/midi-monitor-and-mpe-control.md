# MIDI Monitor And MPE Control

Open when you need guidance on MIDI Monitor And MPE Control in Ableton Live.

Context: [Max for Live MIDI Effects](max-for-live-devices.md#323-max-for-live-midi-effects).

<a id="source-3233-midi-monitor"></a>
### 32.3.3 MIDI Monitor

The MIDI Monitor Effect.

MIDI Monitor serves as a utility MIDI device for showing incoming MIDI together with MPE data.

You can inspect MIDI data through either the Note display or the Flow diagram.

Within the Note display, arriving MIDI notes appear on a keyboard layout together with their root note and any associated chords (when chords are played). The velocity of each note appears as well.

The Flow diagram builds an ongoing stream listing arriving MIDI notes and data, including messages like pitch bend and aftertouch, as the notes are performed. Use the Freeze toggle to halt or resume the display, and the Clear button wipes everything from it.

The Flow Diagram.

You inspect MPE data inside the MPE display. Arriving note, velocity, slide, pressure and per-note pitch data flow through as an ongoing stream while notes are performed.

The MPE Display.

<a id="source-3234-mpe-control"></a>
### 32.3.4 MPE Control

The MPE Control Effect.

MPE Control is a Max for Live MIDI effect for reshaping and transforming arriving MPE (MIDI Polyphonic Expression) signals, providing separate, tailored adjustments for every MPE data source. You normally pair it with a second device so you can refine how the MPE data influences mapped parameters. On top of that, MPE Control can turn MPE signals into global MIDI, which lets you drive non-MPE enabled instruments from an MPE controller.

Before digging into how the MPE Control effect reshapes arriving MPE data, it helps to consider what separates MPE from ordinary MIDI messages. With MPE, MIDI Control Change (or MIDI CC) messages travel on a per-note basis, so each note can be articulated on its own. Lacking MPE, the same messages travel globally, so every note responds to whatever MIDI CC is in play. To read more about MPE, see the [Editing MPE](https://www.ableton.com/en/live-manual/12/editing-mpe/#editing-mpe) chapter.

MPE already opens up far more musical expression than plain MIDI data, yet MPE Control lets you sculpt those MPE signals even further through curves, which makes still more expressive performances possible. Imagine you have the Expression Control device in use and routed its Slide MIDI input onto the Filter Freq knob inside Operator. Every bit of arriving MPE slide data then drives the filter frequency. From there MPE Control can refine that signal so that only the very highest slide values push toward a high cutoff frequency.

Inside MPE Control, arriving MPE signals get reshaped through two kinds of curves, both of which support smoothing for even rise and fall behavior. Three signal sources exist: Press (pressure), Slide, and also NotePB (per-note pitch bend), with each one adjustable on its own.

Whichever MPE source you select has its curve drawn in the front of the display, putting that curve and its associated controls within reach for editing. Out of the box every MPE source is switched on, yet you can turn each one off on its own by clicking the toggle beside its name.

Every MPE source offers two curve-setting choices at the lower left of the display: linear or S-shaped. A linear curve carries two breakpoints, whereas an S-shaped curve carries three.

Pick the linear setting and you can shape the curve through two methods. Either turn the Curve control knob or drag the curve straight inside the display. Beyond reshaping the curve, you can also set its floor and ceiling through the Min and Max sliders, or by hauling the breakpoints sitting at each end of the curve.

A single curve comes from the linear setting, producing a smooth ramp for whichever modulation source you chose, either "compressing" the data so staying in the lower value range is easier, or "expanding" it so reaching higher values takes less input.

Pick the S-shaped curve and a third breakpoint appears at the center of the curve's line, splitting the curve into two separate segments. Because that breakpoint moves freely, you have full say over where the two segments cross over, opening the door to far more extreme curves. By default the two segments stay linked. Flip the Curve Link button to detach the segments from one another, after which each can be compressed or expanded on its own through the two separate Curve dials.

Keep in mind that the breakpoint dividing the two segments can be moved either by clicking and dragging it directly, or through the X-Y controls along the bottom of the display. Those X-Y controls come alive only while the S-shaped curve is in use.

Click the triangular button at the lower right of the visualization to reveal the advanced settings panel.

MPE Control's Expanded View.

Each of the three modulation sources carries a Smooth toggle that turns on smoothing for whichever source is currently selected. You can dial in separate Rise and Fall values per curve through the matching controls, and further controls appear depending on which source you happen to be editing.
