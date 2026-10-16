# Plug In Windows And Parameter Configuration

Open when you need guidance on Plug In Windows And Parameter Configuration in Ableton Live.

Context: [Plug-Ins in the Device View](device-presets-and-plug-in-routes.md#2331-plug-ins-in-the-device-view).

<a id="source-23311-showing-plug-in-panels-in-separate-windows"></a>
#### 23.3.1.1 Showing Plug-In Panels in Separate Windows

The Show/Hide Plug-In Window Button.

Clicking the Show/Hide Plug-In Window button brings up a floating window displaying the native VST or Audio Units plug-in panel. Adjusting a parameter in that floating window produces the same result as adjusting it in the Live panel, and the reverse holds too.

A handful of Plug-Ins Settings matter when you deal with plug-in windows:

- When the _Auto-Open Plug-In Windows_ option is turned on, it guarantees that a plug-in window pops open by itself as soon as you load the plug-in onto a track from the browser.
- Switching on the _Multiple Plug-In Windows_ option in the Plug-In Settings lets you have as many plug-in windows visible simultaneously as you want. Even when it's off, holding the Ctrl (Win) / Cmd (Mac) modifier as you open a new plug-in window stops the earlier window(s) from shutting.
- The _Auto-Hide Plug-In Windows_ option lets you restrict Live to showing just the plug-in windows that belong to whichever track is selected at the moment.

To toggle the visibility of open plug-in windows, use the Show/Hide Plug-In Windows command in the View menu or the Ctrl+Alt+P (Win) / Cmd+Option+P (Mac) shortcut. Bear in mind that the shortcut takes effect only when the plug-in windows were opened by hand first, or when the Auto-Open Plug-In Windows option is switched on in Live's Settings. The title bar of an open plug-in window displays the name of the track the plug-in sits on.

<a id="source-23312-plug-in-configure-mode"></a>
#### 23.3.1.2 Plug-In Configure Mode

The Configure Button.

With Configure Mode, you can tailor Live's panel so it presents only the plug-in parameters you actually need to reach. Here's how:

- Press the "Configure" button in the device's header to switch on Configure Mode.
- Add a parameter to Live's panel by clicking it in the plug-in window. With certain plug-ins, you might have to change the parameter's value for this to register. Also, some plug-ins won't "publish" every parameter to Live, and any such parameter can't be brought into Live's panel.

Once Configure Mode is active, you can rearrange or relocate the parameters in Live's panel by dragging and dropping them elsewhere. Pressing the Delete key removes a parameter. Should you attempt to remove a parameter that already carries automation data, clip envelopes, or MIDI, key or Macro mappings, Live issues a warning first.

Each plug-in instance in your Set keeps its own assigned parameters, and they travel with the Set when saved. To preserve a layout built around a specific group of parameters, [create a Rack](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks) that holds the configured plug-in. You can then store Racks in your User Library and pull them into other Sets. Saving a given parameter configuration as a [default preset](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#default-presets) is another option.

Some plug-ins lack their own windows and present their parameters exclusively in Live's panel. With these, deleting parameters in Configure Mode isn't possible, though you can still relocate and rearrange them.

Plug-in parameters can also reach Live's panel through several routes that don't involve Configure Mode:

- Moving a parameter in the plug-in's floating window spawns temporary entries for it across the clip envelope and automation choosers and the choosers of the panel's X-Y field. Those entries vanish as soon as you touch a different parameter. To keep one (and thereby add it to Live's panel), either edit that parameter's automation or clip envelope, choose another parameter from the automation or clip envelope choosers, or pick the temporary parameter inside one of the X-Y field's choosers.
- Altering a parameter in a plug-in's floating window during recording captures automation data on its own. Once you stop recording, the automated parameters get appended automatically to Live's panels for whichever plug-ins were touched.
- While you're in MIDI, key or Macro mapping mode, moving any parameter in the plug-in's window adds it to Live's panel. That fresh panel entry is selected for you straight away, so you can map it on the spot.

After a plug-in sits on a track and you've (optionally) arranged its parameters in Live's panel, it behaves exactly like any Live device:

- Every parameter in Live's panel can receive mapped MIDI controller messages.
- You're free to drag or copy the device to other spots in the device chain or onto different tracks, within the constraints that govern audio effects and instruments.
- Its continuous parameters can be automated or modulated through clip envelopes.
- Where a plug-in offers multiple I/O, you can route it as a source or target in a track's routing setup. The [Routing and I/O](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) chapter covers this.
- You can attach custom info text to the plug-in.
