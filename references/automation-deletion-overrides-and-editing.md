# Automation Deletion Overrides And Editing

Open when you need guidance on Automation Deletion Overrides And Editing in Ableton Live.

Context: [Automation and Editing Envelopes](automation-and-editing-envelopes.md#25-automation-and-editing-envelopes).

<a id="source-253-deleting-automation"></a>
### 25.3 Deleting Automation

To wipe every bit of automation data, right-click an automated control so its context menu opens and pick Delete Automation, or use the Ctrl+Backspace (Win) / Cmd+Delete (Mac) shortcut keys. With that, the automation LED vanishes and the control holds one fixed value right across the whole Arrangement timeline and within any Session View clips. Particular stretches of automation can also be removed by [editing breakpoint envelopes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation).

<a id="source-254-overriding-automation"></a>
### 25.4 Overriding Automation

It's common to want to audition fresh control moves while leaving the automation already sitting in the Arrangement intact. Granted, with [infinite Undo](https://www.ableton.com/en/live-manual/12/editing-midi/#non-destructive-editing) nothing is ever permanent, yet there's a simple way to switch a control’s automation off for the moment so existing data stays safe: alter the value of an automated control when you're not recording, and its automation LED switches off to show that automation has gone inactive. The current hand-set value has, in effect, _overridden_ whatever automation was there.

Whenever any of the automated controls within your Live Set sit in this inactive state, the Control Bar’s Re-Enable Automation button illuminates.

The Re-Enable Automation Button.

That button does two jobs. First, it flags that the controls right now sit in a state that diverges from what's stored in your Session clips or the Arrangement; second, clicking it switches all automation back on, restoring the controls to the automation that was committed “on tape.“

A single parameter can be re-enabled on its own through the Re-Enable Automation entry in that parameter's context menu. Within the Session View, overridden automation comes back simply by relaunching whichever clip holds the automation.

<a id="source-255-drawing-and-editing-automation"></a>
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
