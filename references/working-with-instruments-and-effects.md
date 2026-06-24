# Working With Instruments And Effects (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 23. Working with Instruments and Effects

Any track in Live is capable of holding several devices, and those devices fall into one of three categories:

- _MIDI effects_ operate on MIDI data and are restricted to MIDI tracks.
- _Audio effects_ operate on audio data and may sit in audio tracks, return tracks, and the Main track. You can also drop them into MIDI tracks, provided they come after an instrument.
- _Instruments_ take in MIDI and produce audio; they belong in MIDI tracks.

For details on any specific device and the way it works, turn to the [Live Audio Effect Reference](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#live-audio-effect-reference), [Live MIDI Effect Reference](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#live-midi-effect-reference), or [Live Instrument Reference](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#live-instrument-reference) chapters.

If you want to build and reuse your own combinations of instruments and effects, see the [Instrument, Drum and Effect Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks) chapter.

You can read more about the kinds of tracks in Live in the [Routing and I/O](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) chapter, which also covers how return tracks let one device's effect be shared across multiple tracks.

To control devices interactively, map their parameters to [MIDI or key remote control](https://www.ableton.com/en/live-manual/12/midi-and-key-remote-control/#midi-and-key-remote-control).

### 23.1 Device View

The Device View is the place where you add, examine, and edit the devices belonging to whichever track is selected. Double-clicking a track’s title bar opens its devices in the Device View, which sits along the bottom edge of Live’s window.

The Device View.

Out of the box, only one of the Device View or the Clip View is shown at any given moment, based on whether the focus is on a device or a clip. To adjust device parameters and work on notes or samples at the same time, you can place the Clip View on top of the Device View.

Stacked Clip and Device View.

To open both views together, use the toggles beside the Clip and Device View Selectors located in the lower-right corner of Live’s window.

The Clip and Device View Selectors.

The keyboard shortcuts CtrlAlt3 (Win) / CmdOption3 (Mac) toggle the Clip View, while CtrlAlt4 (Win) / CmdOption4 (Mac) toggle the Device View.

To free up room in the Device View, fold a device by double-clicking its title bar or by picking Fold from the title bar’s context menu.

Devices Can Be Folded.

### 23.2 Using Devices

You will find Live’s devices in the [browser](https://www.ableton.com/en/live-manual/12/working-with-the-browser/#working-with-the-browser). Along the browser’s sidebar are categories for the built-in devices, [Max for Live devices](https://www.ableton.com/en/live-manual/12/max-for-live-devices/#max-for-live-devices), and [third-party plug-ins](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#using-plug-ins).

Device Labels in the Browser Sidebar.

The quickest method for adding a device to a track is to double-click it in the browser; doing so drops it onto the selected track, or spins up a fresh track when none is selected. As another option, click inside a track to choose it as the target, then highlight a device or preset in the browser and hit Enter to load it onto that track.

Devices can also be dragged onto tracks or drop areas within the Session and Arrangement Views, or straight into the Device View. When you drag a sample into the Device View of a MIDI track, Live spins up a Simpler instrument with that sample already loaded.

To route an external input into a track in Live, you have to switch on the track’s _Arm_ button in the mixer; that is what lets you hear the incoming signal pass through the devices in the track’s device chain when the default Auto monitoring setting is in use. For MIDI tracks, arming usually happens on its own once you add an instrument.

MIDI and Audio Track Arm Buttons.

That, for instance, is how you’d run live instruments through a track’s effects, or drive a track’s instrument from a MIDI keyboard. From here it’s a short step to [recording new clips](https://www.ableton.com/en/live-manual/12/recording-new-clips/#recording-new-clips) you can keep using in a Set. Should you prefer different monitoring behavior, consult the [Monitoring section](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#monitoring) for how to set these options.

You can put one more device on the track by dragging it over or by double-clicking its name to tack it onto the end of the device chain. Within a device chain, signals always flow from left to right.

Audio effects may be dropped anywhere along an audio track’s device chain, but bear in mind that the sequence of effects shapes the final sound. The same applies to the device chain on a MIDI track.

When you place an instrument into a MIDI track’s device chain, note that everything after it (to its right) carries _audio signals_, which only audio effects can use. Everything before it (to its left) carries _MIDI signals_, which only MIDI effects can use. So a single MIDI track’s device chain can contain all three device types at once: MIDI effects first, an instrument next, and audio effects last.

A MIDI Track’s Device Chain Can Contain All Three Device Types.

To delete a device from the chain, click its title bar and hit your keyboard’s Backspace or Delete key, or choose Delete from the Edit menu. To reorder devices, grab a device by its title bar and drop it beside any other device in the Device View. You can relocate devices to different tracks altogether by dragging them out of the Device View and into the Session or Arrangement Views.

Edit menu actions like cut, copy, paste, and duplicate also work on devices. A pasted device lands ahead of whichever device is currently selected. To paste at the tail of a device chain, click the empty area past the last device, or press the right arrow key to shift the selection there. As a rule, you can add, rearrange, and delete devices without breaking the audio stream.

Each device in a Live track carries input and output level meters. They make it easy to spot a misbehaving device in the chain: a weak or missing signal shows up on the meters, after which you can tweak the relevant device settings, deactivate the device, or take it out.

The Level Meters Between Devices in a Chain.

Keep in mind that clipping never happens between devices, since the headroom there is essentially limitless. Clipping only happens when too hot a signal reaches a _physical output_ or gets written to a sample file.

Now that you’ve covered working with devices in Live, you may want to explore [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes), which let you automate or modulate single device parameters clip by clip.

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

### 23.2.4 Hot-Swapping Presets

_Hot-Swap mode_ offers a fast route to swapping out a track’s preset. While it’s on, the track’s preset is tied to the browser, letting you preview and load other presets. Kick off hot-swapping by pressing Q or clicking the _Hot-Swap Presets_ button on the device’s title bar.

The Hot-Swap Presets Button.

Pressing Q to turn on Hot-Swap mode makes the track’s currently selected preset available for swapping. When no preset is selected, the swap falls on the instrument for a MIDI track, or on the earliest audio effect for an audio track.

After Hot-Swap mode turns on, the preset gets highlighted in the browser and its device folder opens. You can trade it for another preset in that same folder, or move to a different folder to bring in a preset for a different device. Only presets sharing a device type can be hot-swapped; you can’t, for example, trade an audio effect for a MIDI effect.

Browse and Replace Presets in Hot-Swap Mode.

Step through the presets with the up and down arrow keys. Press Enter to load whichever preset is highlighted, or double-click the one you want. To fall back on a device’s default settings, pick the device’s parent folder and load that rather than any of its presets.

Note that presets can load automatically in Hot-Swap mode if you add the -EnableHotSwapOnSelection entry to the [Options.txt](https://help.ableton.com/hc/en-us/articles/6003224107292) file. With it on, the current preset gets swapped the instant you select a new one in the browser.

After you’ve finished swapping presets, leave Hot-Swap mode through any of these actions:

- Press the Q key.
- Press the Esc key.
- In the Hot-Swap bar sitting atop the browser’s content pane, click the X button.
- Click the X button in the device’s title bar.
- Navigate from the browser to a different view.

#### 23.2.4.1 Hot-Swapping Samples

Beyond trading whole presets, you can also swap the loaded samples in [Drum Rack pads](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#pad-view), [Drum Sampler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#drum-sampler), [Impulse](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#impulse), [Sampler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sampler), and [Simpler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#simpler).

To do this, click the _Hot-Swap Sample_ button, which shows up in these spots:

- Drum Rack pads — At the bottom right of each pad.
- Drum Sampler — At the bottom right of the Waveform Display.
- Impulse — At the bottom right of each sample slot.
- Sampler — In the Zone Editor’s upper-left area once it has been expanded.
- Simpler — At the bottom right of the Sample Display.

Note that the button shows up only while you hover over the matching area (Sampler being the exception, where it stays visible). In Drum Sampler, for instance, hovering over the Waveform Display brings up the button.

The Hot-Swap Sample Button for Drum Sampler.

Clicking it opens the browser to the folder holding that sample. From there you can switch the loaded sample for a different one in the same folder, or grab a sample out of another folder. Press Enter to load a highlighted sample, or double-click the one you want.

The Loaded Sample in a Device Can Be Swapped in the Browser.

Once you’re finished swapping samples, leave Hot-Swap mode by:

- Clicking the Hot-Swap Sample button in the device.
- Clicking the X button on the Hot-Swap bar found above the content pane of the browser.
- Pressing the Esc key.
- Pressing the Q key.
- Navigating from the browser to a different view.

### 23.2.5 Saving Presets

In the browser’s _User Library_, you’re free to build and store as many of your own presets as you like.

The Save Preset Button.

Hit the Save Preset button to keep a device’s current settings (custom info text included) as a brand-new preset. Live then takes you to the browser, where pressing Enter accepts Live’s proposed name or you can enter your own. Press the Esc key to back out of saving. You can also drop presets into particular folders in the browser’s Places section (for example, your Current Project folder) by dragging from the device’s title bar into whichever browser spot you choose.

For a thorough rundown of what the browser can do, see the [Managing Files and Sets](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#managing-files-and-sets) chapter. To learn about keeping presets tied to a specific project, see the [Projects and Presets](https://www.ableton.com/en/live-manual/12/managing-files-and-sets/#projects-and-presets) section.

### 23.2.6 Default Presets

Whenever you store presets in the _Defaults_ folders inside your User Library, they take the place of the standard device settings when loading. The Defaults folders additionally let you:

- Tailor Live’s behavior toward various user actions, like dropping samples, slicing, and converting audio to MIDI.
- Make freshly created MIDI and audio tracks open with specific devices already loaded and their parameters set the way you want.
- Open VST and Audio Units plug-ins with a chosen set of parameters already laid out in Live’s panel.
  The Default Presets folders in the User Library.

To store a Live device’s current settings as a default preset, bring up the context menu on the device’s header and choose “Save as Default Preset.“ It applies to every one of Live’s instruments, MIDI effects, and audio effects (the various [Racks](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks) included). When a default preset already exists for that device, Live prompts you before replacing it.

To build a default configuration preset for a VST or Audio Unit plug-in:

- Load the chosen plug-in onto a track.
- Within the plug-in’s [Configure Mode](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#plug-in-configure-mode), arrange the set of parameters you want.
- Bring up the context menu on the track header and choose “Save as Default Configuration.”

When both the VST and Audio Units builds of a given plug-in are installed, you can make a separate default configuration preset for each one. Note that a plug-in’s default preset doesn’t store the _settings_ of the configured parameters; what gets saved is only how the parameters are arranged in Live’s panel.

To build default presets for MIDI and audio tracks:

- Place whatever device(s) you want as the default onto a track (or none at all, if your default track should be empty).
- Set the device parameters however you prefer.
- Bring up the context menu on the track header and choose “Save as Default Audio/MIDI Track.”

To set how Live responds when you drag a sample to a Drum Rack or to the Device View of a MIDI track:

- Make an empty Simpler or Sampler.
- Set the parameters however you prefer.
- Drag the adjusted device onto the “On Drum Rack“ or “On Device View“ folder inside the Defaults/Dropping Samples folders of your User Library. You can also store Drum Rack pad defaults through a context menu option on a Drum Rack’s pad.

To change how Live responds when slicing an audio file:

- Make an empty Drum Rack.
- Put an empty Simpler or Sampler into the Drum Rack so there’s a single chain.
- Add whatever extra MIDI or Audio Effects you want to this chain.
- Set the parameters on any of the devices.
- Map [Macro Controls](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#using-the-macro-controls) to any of the controls in the chain’s devices.
- Drag the whole Drum Rack onto the Defaults/Slicing folder of your User Library.

You’re free to make several slicing presets and pick among them using the Slicing Preset chooser in the slicing dialog.

To build default presets for [converting Drums, Harmony, or Melody to MIDI](https://www.ableton.com/en/live-manual/12/converting-audio-to-midi/#convert-harmony-to-new-midi-track):

- Make a MIDI track holding the instrument you want as the default for a given conversion type. Note that a default preset for converting drums has to include a Drum Rack.
- Add whatever extra MIDI or Audio Effects you want to the track.
- Set the parameters on any of the devices.
- When you’re using more than one device, bundle them into a Rack.
- Drag the whole Rack onto the matching folder in Defaults/Audio to MIDI of your User Library.

Beyond these application-wide default presets, you can also make default presets that apply to a single Project only. That comes in handy when, say, you rely on tailored device or track setups for one particular Set and want to spin off variations of the Set that still have these presets, all without disturbing the broader default presets you use elsewhere. To build Project-specific default presets:
