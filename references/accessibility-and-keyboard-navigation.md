# Accessibility And Keyboard Navigation

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 40. Accessibility and Keyboard Navigation

Across macOS and Windows alike, Live 12 introduces fresh accessibility capabilities. These cover screen readers along with other assistive tools that rely on each operating system's own accessibility communication protocols. The release also brings a high-contrast choice for the new themes, more efficient [keyboard navigation](https://www.ableton.com/en/live-manual/12/live-keyboard-shortcuts/#general-keyboard-navigation-and-workflow), plus a Settings menu with tidier organization.

The bulk of Live’s views, controls, and devices function with screen readers, yet a handful of device elements remain un-optimized for them — for instance, the Modulation Matrix in Wavetable together with certain deeper parameters in Operator. A number of further Live and external features lack screen reader support at present, among them:

- Browser tagging and filters
- MPE editing in Clip View
- Max for Live
- Some third-party plug-ins

If you have frequently asked questions regarding the accessibility support in Live, consult the [Accessibility in Ableton Live FAQ](https://help.ableton.com/hc/en-us/articles/11762577169948) within the Knowledge Base.

### 40.1 Menu and Keyboard Navigation Settings

You can locate a range of accessibility and keyboard navigation choices within Live’s Settings, plus inside the Options and Navigate menus.

Alongside the enhanced keyboard navigation, a variety of [keyboard shortcuts](https://www.ableton.com/en/live-manual/12/live-keyboard-shortcuts/#live-keyboard-shortcuts) exist for frequent actions and commands.

### 40.1.1 Using Tab for Navigation

Once the _Use Tab Key to Move Focus_ option has been turned on through the Navigate menu or by way of Live’s Display & Input Settings, you can rely on the Tab key for navigation in these manners:

- Tab moves to the next control.
- ShiftTab moves to the previous control.

You may also employ the Tab key to step among controls within the Session and Arrangement mixers through the shortcuts below:

- CtrlTab (Win) / OptionTab (Mac) carries you onward to the following control within that same row.
- CtrlShiftTab (Win) / OptionShiftTab (Mac) carries you back to the preceding control within that same row.

With Use Tab Key to Move Focus disabled, a press of the Tab key toggles between Session and Arrangement View, the way it did in earlier Live releases.

Beyond moving focus with Tab, you also have access to these navigation choices:

- _Wrap Tab Navigation_ - With this turned on, once you reach the final control in an area, pressing Tab loops focus back to the very first control rather than halting. Should the first control be the active one, a press of ShiftTab carries focus to the last control. Turn this on through the Navigate menu or via the Display & Input Settings.
- _Move Clips with Arrow Keys_ - Active by default, this lets the left and right arrow keys shift selected clips and/or the time selection inside Arrangement View. Disable the behavior in the Display & Input Settings whenever you prefer. With it off, the left arrow key shrinks the time selection down to its start point, whereas the right arrow key shrinks it down to its end point.

### 40.1.2 Settings Menu

Open Live’s Settings with the shortcut Ctrl, (Win) / Cmd, (Mac).

You can move between options within the Settings tabs by means of the Tab and ShiftTab keys. Whether the [Use Tab Key to Move Focus](https://www.ableton.com/en/live-manual/12/accessibility-and-keyboard-navigation/#using-tab-for-navigation) option is on or off, these shortcuts still function.

While a command holds focus in one of the Settings tabs, the up and down arrow keys let you flip a toggle's state, tweak a value, or step through the choices offered for that command. The Enter key likewise lets you alternate between toggle states.

Move among the various tabs in the Settings Page Chooser with CtrlTab (Win) / OptionTab (Mac) and CtrlShiftTab (Win) / OptionShiftTab (Mac), or with the up and down arrow keys whenever the chooser holds focus. Should keyboard focus rest on the first control of any Settings tab, the ShiftTab shortcut sends focus back to the Settings Page Chooser.

Shut the Settings window by pressing the Esc key.

Keep in mind that selecting a different preferred UI language in the Display & Input Settings requires a restart of Live before the change applies.

### 40.1.3 Options Menu

Additional accessibility settings live in Live’s Options menu, where you'll find an Accessibility sub-menu. Reach that sub-menu from the keyboard with AltO (Win) / VOM then O with VoiceOver (Mac).

Within the sub-menu sit a handful of items that switch on particular screen reader announcements, namely Speak Menu Commands, then Speak Minimum and Maximum Slider Values, plus Speak Time in Seconds.

### 40.1.4 Speak Help Text

The majority of controls and regions in Live carry descriptive text, which you reach through the [Info View](https://www.ableton.com/en/live-manual/12/first-steps/#info-view). Under Windows, switch on screen reader announcements for those descriptions by turning on the Speak Help Text option inside your chosen screen reader. Under macOS, achieve the same result by enabling help text within the VoiceOver Utility’s verbosity settings. You may additionally reach this option by hand with a press of VOShiftH.

### 40.2 Audio Setup

To set up your audio in Live, launch the Settings menu via the shortcut Ctrl, (Win) / Cmd, (Mac), and then steer to the Audio page with the arrow keys.

Tab lets you cycle through the options on the Audio page so you can begin setting up your audio device.

How audio is set up differs across macOS and Windows. Under macOS, you can route Live’s input and output to any CoreAudio device, and pick alternative drivers from the Driver Type drop-down menu when required. Under Windows, choose whichever driver you favor — ASIO4ALL, say — and handle attached devices through the driver’s own program.

### 40.3 Connecting MIDI Devices

Connected MIDI devices are picked up by Live on their own, and plenty of them call for no extra setup.

Certain MIDI controllers ship with control surface scripts that ease their integration into Live’s workflows. Bear in mind that screen reader coverage for control surfaces differs from one third-party manufacturer to the next, so a given controller might not be optimized for screen readers.

On the Link, Tempo & MIDI page, the MIDI section provides six Control Surface drop-down menus through which you choose control surfaces by means of the purpose-built [keyboard navigation options](https://www.ableton.com/en/live-manual/12/accessibility-and-keyboard-navigation/#settings-menu). For each control surface you pick, you may also set the input and output port settings.

For a deeper look at configuring MIDI in Live, head to the [MIDI and Key Remote Control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control) chapter.

### 40.4 Navigating in Live

Most of Live’s menus, views, and controls are reachable from the computer keyboard. Keep in mind that to use any of the Tab-based shortcuts covered in this section, the [Use Tab Key to Move Focus](https://www.ableton.com/en/live-manual/12/accessibility-and-keyboard-navigation/#using-tab-for-navigation) option found in the Navigate menu or Display & Input Settings has to be switched on.

### 40.4.1 Navigate Menu

The Navigate menu gives you a way into every one of Live’s main views plus the other navigation options. The bulk of the menu’s entries carry matching keyboard shortcuts as well. Open the Navigate menu with AltN (Win) / VOM then N with VoiceOver (Mac).

#### 40.4.1.1 Control Bar - Alt0 (Win) / Option0 (Mac)

Made up of assorted project settings, transport controls, mouse and keyboard tools, and status views, the Control Bar arranges its controls into accessible groupings; with Speak Help Text turned on, you can step among them via Tab and ShiftTab to hear about each option.

The control you last had focused is retained by the Control Bar, and focus lands back on it whenever you return to the Control Bar from a different view.

#### 40.4.1.2 Session View - Alt1 (Win) / Option1 (Mac)

Live’s non-linear take on making music is the [Session View](https://www.ableton.com/en/live-manual/12/session-view/#session-view). This view breaks down into four primary sections:

_Track Title Bars_ appear for every track in your Set. Step among the track title bars with the left and right arrow keys. A right-click on a track title bar brings up the context menu, home to handy track-related commands together with their matching keyboard shortcuts.

_Clip Slots_ fall into groups by track (running vertically, top to bottom) and by scene (running horizontally, left to right). An audio track's slots can hold audio clips, while a MIDI track's slots can hold MIDI clips. With focus on a clip slot of a MIDI track, drop in an empty MIDI clip with CtrlShiftM (Win) /CmdShiftM (Mac). Fire off a selected clip by hitting Enter. Should Live’s transport be playing, the clip starts up according to the present value in the Control Bar’s quantization menu. Be aware that, although clip slots show up in return tracks too, those slots can neither hold nor launch clips.

_Scenes_ let you set off neighboring clips across different tracks together by way of the Main track scene numbers, which you step through with the up and down arrow keys. Fire scenes with the Enter key.

For each track, the _Mixer_ holds [routing](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) along with [mixer options](https://www.ableton.com/en/live-manual/12/mixing/#mixing). Decide which mixer elements appear through the Mixer Controls sub-menu under the View menu, or via the drop-down menu beside the Mixer view control down in the lower right corner of Live’s window. Such elements cover input/output assignment along with send levels, volume controls plus track options, and also crossfader controls together with performance impact monitoring. By default, the final three stay hidden.

The arrow keys let you move among track title bars, clip slots, and scenes.

Hop from tracks/slots over to the mixer using Tab and ShiftTab. The same Tab and ShiftTab pair also moves you among a track’s mixer controls.

To shift focus onto the matching control on another track, reach for the Navigate menu's _Next Neighbor_ and _Previous Neighbor_ commands, or else these shortcuts: CtrlTab (Win) / OptionTab (Mac) and CtrlShiftTab (Win) / OptionShiftTab (Mac).

The Esc key shifts focus away from the element currently focused in a track and onto that track’s title bar.

#### 40.4.1.3 Arrangement View - Alt2 (Win) / Option2 (Mac)

Serving as a timeline-style view, the [Arrangement View](https://www.ableton.com/en/live-manual/12/arrangement-view/#arrangement-view) is where you lay out audio, MIDI, and automation within Live.

Several distinct approaches exist for getting around the Arrangement View:

_Navigating through Tracks_

- Shift among tracks by means of the up and down arrow keys.
- Shift among track mixers with CtrlTab (Win) / OptionTab (Mac), and work through a track’s mixer controls with Tab and ShiftTab.

_Navigating through the Timeline_

- Step ahead or back in time in line with the present grid settings, using the left and right arrow keys.
- Make the Arrangement View’s grid settings coarser or finer by means of the + and - keys.
- Jump to the prior/following clip edge or locator within a content lane via Ctrl (Win) / Option (Mac) plus the left and right arrow keys.

_Using Locators_

- Create a locator by first steering to the spot you want on the timeline with the arrow keys. After that, press Tab to put focus on the Set Locator button, and then press Enter.
- Step among locators by means of Tab and ShiftTab.
- Remove a locator by steering to it and then pressing the Delete key.

_Handling Content_ - Pick content on the timeline by holding Shift and then working the arrow keys. - Shift selected content via the left and right arrow keys. - Cut selected content via CtrlX (Win) / CmdX (Mac). - Copy selected content via CtrlC (Win) / CmdC (Mac). - Paste selected content via CtrlV (Win) / CmdV (Mac). - Duplicate selected content via CtrlD (Win) / CmdD (Mac). - Remove selected content via the Delete key.

_Adjusting Clip Edges_

- Stretch or trim a clip by bringing the insert marker over to the clip’s edge, then pressing Enter and working the left and right arrow keys to set the length. A second press of Enter locks in the changes, while Esc backs out.

_Exporting Audio_

- Pick a region on the timeline and press the shortcut CtrlR (Win) / CmdR (Mac) to bring up the audio export dialog. The Main track is rendered by default.

Note: At present, the editing of audio clip fades cannot be done through a screen reader.

#### 40.4.1.4 Clip View - Alt3 (Win) / Option3 (Mac)

Clip properties get defined and tweaked in the [Clip View](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view). Open Clip View by double-clicking any clip in the Arrangement or Session View, or with the shortcut CtrlAlt3 (Win) / CmdOption3 (Mac).

Two principal regions make up Clip View: the _clip panels_ and an _editor_.

A range of options for tweaking note properties sits in the clip panels. Reach the panels from another view with the shortcut AltShiftP (Win) / OptionShiftP (Mac).

A selection of editors caters to audio waveforms, MIDI notes, clip envelopes, and MPE data. The first time a clip opens in Clip View, audio clips show the _Sample Editor_ whereas MIDI clips show the _MIDI Note Editor_. Bring focus onto the active editor from another view with the shortcut Alt3 (Win) / Option3 (Mac).

Getting around Clip View can be done in these ways:

_Working with the MIDI Note Editor_

- Turn on _MIDI Note Editor Preview_ under the Options menu so the notes sound as you add, select, or shift them in the editor.
- Drop the insert marker at any point in the MIDI Note Editor, then hold Shift and work the left and right arrow keys to pick out time.
- Pick any MIDI notes that fall inside a time selection with the Enter key.
- Bring the insert marker to the prior or following note boundary via Ctrl (Win) / Option (Mac) plus the left and right arrow keys.

_Navigating through MIDI Notes_

- Skip to the prior or following note by holding Ctrl with the up/down arrow keys (Win), or Option with those same arrow keys (Mac).
- Skip to the prior or following note at the same pitch by holding Ctrl with the left/right arrow keys (Win), or Option with those same arrow keys (Mac).
- Tack on the Shift modifier to the shortcuts above to widen the note selection.

_Editing MIDI Notes_

- Transpose the selected notes with the up and down arrow keys.
- Transpose the selected notes in octave steps with Shift and the up and down arrow keys.
- Trim or stretch the selected notes per the present grid settings with Shift and the left and right arrow keys.
- Slide the selected notes through time per the present grid settings with the left and right arrow keys.
- Tweak the velocity of the selected notes with Ctrl (Win) / Cmd (Mac) and the up and down arrow keys.
- Tweak the probability of the selected notes with CtrlAlt (Win) / CmdOption (Mac) and the up and down arrow keys.

_Working with Audio Clips_

- Shift the insert marker with Ctrl (Win) / Option (Mac) plus the left and right arrow keys.
- Hold the Shift modifier to begin a time selection, then press the left or right arrow key to widen or narrow it.
- Reposition a selected Warp Marker with the left and right arrow keys.
- Drop in and select a Warp Marker at the present position with CtrlI (Win) / CmdI (Mac).
- Drop in a transient at the present position with CtrlShiftI (Win) / CmdShiftI (Mac).

Note: MPE editing is not currently supported for use with screen readers.

#### 40.4.1.5 Device View - Alt4 (Win) / Option4 (Mac)

The chain of devices placed on a track shows up in the [Device View](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects). A MIDI track can hold MIDI effects, instruments, and audio effects, while audio tracks, group tracks, return tracks, and the Main track can hold audio effects.

To screen readers, every device placed on a track is presented as a group. Step among the devices with the left and right arrow keys.

You can cut, copy, paste, duplicate, or delete devices by means of the keyboard shortcuts listed here:

- Cut: CtrlX (Win) / CmdX (Mac)
- Copy: CtrlC (Win) / CmdC (Mac)
- Paste: CtrlV (Win) / CmdV (Mac)
- Duplicate: CtrlD (Win) / CmdD (Mac)
- Delete: Delete

Work through the controls of a selected device with Tab and ShiftTab.

Note: Although the majority of Live's devices provide basic accessibility support, the more involved ones are not yet optimized for screen readers.

#### 40.4.1.6 Browser - Alt5 (Win) / Option5 (Mac)

Your library of instruments, devices, and files lives in the [browser](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#working-with-the-browser). Four primary sections split it up: the _search bar_, _filters_, _sidebar_, and _content pane_.

From any spot in Live, the shortcut CtrlF (Win) / CmdF (Mac) sends focus to the search bar. Doing so also picks the All label in the browser’s sidebar on its own, the label that takes in every bit of browser content. Whatever the search turns up appears in the content pane.

The Tab key flips you among the browser's different areas. With the search bar focused, a Tab press carries focus first onto the Show/Hide Filter View toggle, next onto the Filter View menu, and at last onto the sidebar. With the sidebar focused, pressing Tab carries focus onto the filters (when shown) or onto the content pane. The down arrow key likewise carries focus from the search bar over to the content pane.

A variety of labels for the different browser items fill the sidebar — among them the bundled Core Library content, Live Packs, Collections, and beyond. Step among labels with the up and down arrow keys. Picking a label shows its contents in the content pane. Cross between the sidebar and content pane with the left and right arrow keys.

Driven by the chosen browser label, the content pane lays out a list of devices and files. Multi-select content with Shift and the up and down arrow keys. Open a selected folder with the right arrow key, and close the folder with the left arrow key.

A handful of browser items — clips and instrument presets among them — carry an [audio preview](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#previewing-files). To catch the preview as you browse, switch on the Browser File Preview entry under the Options menu. Even with previewing turned off, you can still trigger the preview by pressing the right arrow key while a browser item is selected.

Note: As of yet, screen readers cannot be used together with filtering and tagging.

#### 40.4.1.7 Groove Pool - Alt6 (Win) / Option6 (Mac)

You can reshape the timing and “feel“ of clips by applying _grooves_. A broad assortment of grooves ships with Live, and you can bring them into a Set through the [Groove Pool](https://www.ableton.com/en/live-manual/12/using-grooves/#using-grooves).

Step among groove parameters with Tab and ShiftTab, and lean on the up and down arrow keys to set parameter values.

#### 40.4.1.8 Learn View - Alt7 (Win) / Option7 (Mac)

Inside the Learn View sits an assortment of lessons — brief tutorials that walk through various facets of Live.

### 40.5 Editing Automation and Modulation Envelopes

The computer keyboard lets you add, edit, and remove breakpoints within automation and modulation envelopes. As you make changes, screen readers report back on each action.

The actions covered below work in [automation lanes](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) for tracks within the Arrangement View, and equally in the [Envelope Editor](https://www.ableton.com/en/live-manual/12/clip-envelopes/#the-clip-envelope-editor) for clips.

### 40.5.1 Navigating Between Breakpoints

Get around automation and modulation envelopes by means of the insert marker, which marks where you currently are on the grid. Shift the insert marker with the left and right arrow keys. As you travel across the envelope, the automation or modulation value at your current spot is shown.

The Automation Value is Shown at the Insert Marker Location.

Make a breakpoint at the insert marker’s spot by pressing Enter. From there, press Enter once more to lock it in, or nudge the breakpoint with the left and right arrow keys before pressing Enter so it lands somewhere else.

Hit Alt (Win) / Option (Mac) together with the left or right arrow key to skip to the prior or following breakpoint.

As you step through breakpoints, whichever breakpoint holds focus appears in a color distinct from the main envelope. That same color shows up when you hover the mouse over breakpoints.

A Focused Breakpoint.

### 40.5.2 Selecting and Editing Breakpoints

Pick an existing breakpoint at the insert marker’s spot by pressing the Enter key.

As an alternative, hold Alt (Win) / Option (Mac) and click a breakpoint to bring the insert marker to its spot and select it.

Select the following or prior breakpoint with Tab and ShiftTab.

A pulsing animation marks selected breakpoints to signal that they are presently selected and open to editing.

A Breakpoint Pulses When Selected.

Should you shift a selected breakpoint and then undo that action with CtrlZ (Win) / CmdZ (Mac), the breakpoint you just moved momentarily takes on the same color seen when a breakpoint is focused or hovered over. That makes it simpler to spot which one was touched — particularly while editing breakpoints stacked in vertical alignment.

A Previously Moved Breakpoint Temporarily Uses a Different Color.

To alter the automation or modulation value of a selected breakpoint, key in a number or work the up and down arrow keys to set the value. Press Enter to lock in the change and drop the selection on the breakpoint. Or else, press Esc to back out of the change and drop the selection.

Clear a selected breakpoint with the Delete key.

### 40.5.3 Switching Between Automation Envelopes in Arrangement View

Step through every automation envelope belonging to the devices on a track by pressing Alt (Win) / Option (Mac) along with the up and down arrow keys.

Step through all of a device's parameters — those with automation envelopes and those without — by pressing ShiftAlt (Win) / ShiftOption (Mac) along with the up and down arrow keys.
