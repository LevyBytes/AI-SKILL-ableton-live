# Device View And Device Chains

Open when you need guidance on Device View And Device Chains in Ableton Live.

Context: [Working with Instruments and Effects](working-with-instruments-and-effects.md#23-working-with-instruments-and-effects).

<a id="source-231-device-view"></a>
### 23.1 Device View

The Device View is the place where you add, examine, and edit the devices belonging to whichever track is selected. Double-clicking a track’s title bar opens its devices in the Device View, which sits along the bottom edge of Live’s window.

The Device View.

Out of the box, only one of the Device View or the Clip View is shown at any given moment, based on whether the focus is on a device or a clip. To adjust device parameters and work on notes or samples at the same time, you can place the Clip View on top of the Device View.

Stacked Clip and Device View.

To open both views together, use the toggles beside the Clip and Device View Selectors located in the lower-right corner of Live’s window.

The Clip and Device View Selectors.

The keyboard shortcuts Ctrl+Alt+3 (Win) / Cmd+Option+3 (Mac) toggle the Clip View, while Ctrl+Alt+4 (Win) / Cmd+Option+4 (Mac) toggle the Device View.

To free up room in the Device View, fold a device by double-clicking its title bar or by picking Fold from the title bar’s context menu.

Devices Can Be Folded.

<a id="source-232-using-devices"></a>
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
