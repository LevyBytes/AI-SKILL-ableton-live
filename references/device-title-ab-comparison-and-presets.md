# Device Title A/B Comparison And Presets

Open when you need guidance on Device Title A/B Comparison And Presets in Ableton Live.

Context: [Using Devices](working-with-instruments-and-effects.md#232-using-devices).

<a id="source-2321-device-title-bar"></a>
### 23.2.1 Device Title Bar

A device’s title bar gives you controls to switch the device on or off, [save](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#saving-presets) and [hot-swap](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#hot-swapping-presets) presets, [create default presets](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#default-presets), and bring up the device’s context menu.

Some title bar controls show up only on particular devices, for instance [the scale awareness toggle](https://www.ableton.com/en/live-manual/12/live-concepts/#scale-awareness) on devices able to track a clip’s scale, and the Learn toggle on [the Chord device](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#chord).

To switch devices on or off, use their Activator toggles.

Device Activator Toggles.

Switching a device off behaves like deleting it for the moment: the signal passes through untouched, and no CPU cycles go to the device. As a rule, a Live device costs nothing in CPU until it is switched on. For further reading, see the [Managing the CPU Load section](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#managing-the-cpu-load). The Freeze Track command covered there comes in particularly handy with CPU-heavy devices.

Certain devices offer views you can open up above the Device View. Examples include the Gain Stage and Modulation Matrix sections found within [Roar](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#roar), along with the Frequency Display belonging to [EQ Eight](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#eq-eight).

Devices that offer this sort of view carry an arrow toggle just to the right of the Activator toggle. That toggle reveals or hides the view.

The Expanded View Toggle for Roar.Roar’s Expanded View.

Certain views can be opened inside the device itself as well, such as the LFO and Envelope Follower sections in [Phaser-Flanger](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#phaser-flanger). A triangle icon on the device title bar marks this kind of view.

The Expanded View Toggle for Phaser-Flanger.Phaser-Flanger’s Expanded View.

Every device offers a context menu holding standard editing actions like Cut, Copy, and Rename. Certain entries belong to just one device, like the Mono Sidechain option found in [Auto Filter](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#auto-filter).

Context Menu Options for Auto Filter.

To open the context menu, right-click a device’s title bar or click the Show Options toggle.

The Show Options Toggle.

<a id="source-2322-device-ab-comparison"></a>
### 23.2.2 Device A/B Comparison

Each of Live’s built-in devices carries two device states, A and B, and each can hold its own set of parameter values. This gives you a way to store and contrast the edits you make while building or refining presets. You might park a version of a preset you’d rather not lose in one device state and keep tinkering in the other.

A Device Can Store Two Sets of Parameter Values.

Comparing parameter settings across the two device states is handy for tasks such as EQing and compression, where small tweaks can be clearly audible. You can audition tiny parameter changes to hear their effect on the sound, or weigh your edits against the default values.

The first time a device loads, both A and B share its default parameter values. As soon as you change a parameter, B holds onto the original values while your edits land only in A.

To send the current parameter values from the A device state over to B, pick the _Compare: Copy A to B_ command, which you’ll find in the Edit menu, in the device’s own context menu, or under its Show Options toggle.

You Can Copy the Parameter Values from One Device State to Another.

To move from the A device state to B, use the _Compare: Switch to B_ command or press the P key. While the B device state is active, a “(B)” shows up beside the device’s name in the title bar.

The B Device State.

Since the Compare commands work in either device state, you decide how parameter values get stored in A and B. One state could hold the defaults as a baseline, or you could turn both into entirely different-sounding presets. Be aware that these commands don’t apply to Racks, Max for Live devices, or plug-ins.

Because A and B are separate device states, [any parameter automation](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#drawing-and-editing-automation) you draw in one isn’t carried over to the other. In practice, automation you create in the A device state turns off when you move to B, and it won’t come back on by itself when you return to A.

Automation Is Disabled When Switching Between Device States.

To switch any disabled parameter automation back on, run the _Re-Enable Automation_ command from the parameter’s context menu while the device state you intend to use is active.

Re-Enable Automation Using the Context Menu Command.

You can issue this command from either device state. Remember that, because automation belongs to A and B separately, it gets turned off again every time you move between the two states.

When a device is copied or duplicated, only the parameter values of the active device state come along. As an example, copying a device while A is active produces a new device whose A and B both take the original’s A device state values, even when the original’s B device state holds different ones.

Copying (Right) Carries Over Only the Active Device State’s Parameter Values (Left).

In the same way, saving a preset to your User Library applies the active device state’s parameter values to both A and B.

Note that device states can be reached through [the Live API with Max for Live](https://docs.cycling74.com/apiref/lom/device/).

<a id="source-2323-live-device-presets"></a>
### 23.2.3 Live Device Presets

Live devices can save and recall their parameter settings as _presets_. In the browser’s content pane, every device shows up as a folder you can open to see the presets inside.

Presets in the Browser.

That folder stands for the device’s default preset, which is either the factory settings as shipped or [default settings](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#default-presets) you saved yourself. The presets sitting inside the folder carry custom settings. Presets ship as part of the Core Library and Packs. You can additionally [create and save your own presets](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#saving-presets).

The computer keyboard lets you browse and load presets in a hurry:

- Move up and down with the up and down arrow keys.
- Collapse and expand device folders with the left and right arrow keys.
- Hit Enter to drop a preset onto a selected track.

You can also load a preset onto a selected track by double-clicking it in the browser, or by dragging it from the browser onto a track’s title bar or device chain.

While loading presets through the browser is the usual recommendation, you can also drag [Live-specific device file types](https://help.ableton.com/hc/en-us/articles/209769625) (such as .adg, .adv, and .amxd) right into a Live Set from the Explorer (Win) / Finder (Mac).

To swap a track’s preset for another, drag a different preset out of the browser and drop it on top of the current preset in the track’s device chain.
