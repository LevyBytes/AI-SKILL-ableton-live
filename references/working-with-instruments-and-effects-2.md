# Working With Instruments And Effects (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

- Rebuild the Defaults folder inside the Project folder, along with whatever subfolders you want.
- Set the relevant device parameters, track settings, and so on, based on the kinds of Project-specific defaults you intend to use.
- Store the device or track in the matching folder under your Project-specific Defaults folder.

From then on, loading a Set belonging to this Project will pull any default presets you stored in these Project folders rather than the ones in the User Library. Keep in mind that the context menu commands for saving defaults route them to your primary User Library, which means they can't create Project-specific defaults.

### 23.3 Using Plug-Ins

You can broaden the set of devices available in Live by adding _plug-ins_. The VST plug-in format from Steinberg Media is supported, along with the Audio Units (AU) plug-in format (macOS only), namely:

- VST2
- VST3
- Audio Units 2
- Audio Units 3 (Live 11.2 and later)

Using VST and Audio Units plug-ins closely resembles using Live's own devices. Instruments in VST and AU formats are restricted to Live MIDI tracks, and just like Live instruments they accept MIDI and produce audio output. Plug-in audio effects may sit only in audio tracks or downstream of instruments. For more, refer back to the earlier [Using the Live Devices](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#using-devices) section.

If you want Live to bypass plug-in scanning at startup, keep the Alt (Win) / Option (Mac) modifier held down as the program opens, until the splash screen disappears. That trick is useful when diagnosing crashes, letting you check whether a plug-in is at fault.

Plug-Ins in the Browser.

You browse and bring in Audio Units and VST plug-ins through the Plug-Ins label of the browser. Instruments appear with a keyboard icon there, which sets them apart from plug-in effects.

Be aware that the browser exposes plug-in presets for Audio Units plug-ins only. At times, Audio Units factory presets surface in the browser solely after the device has been added to a track and its Hot-Swap button switched on.

_Note_: On your first Live launch, the Plug-Ins label stays empty because you have to "activate" your plug-in sources beforehand. This activation step informs Live about which plug-ins you intend to use and the locations where they live on your machine. Details about activating (and deactivating) plug-in sources appear further along in this chapter, under the [VST Plug-In folder](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#the-vst-plug-in-folder) and [Audio Units Plug-Ins](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#audio-units-plug-ins) sections.

_Note for “Intel® Mac“ users_: VST or AU plug-ins built for the PowerPC platform won't run natively on Intel® Mac machines. Live accepts only plug-ins of the Universal or Intel® type.

Should you add or remove a plug-in with the program already open, Live won't register those changes in the browser before your next launch. To pick them up mid-session, click the _Rescan_ button in the Plug-Ins Settings, which makes freshly installed devices show up in the browser right away.

A rescan is also worthwhile when you suspect that your plug-in database has become corrupted somehow. If you hold the Alt (Win) / Option (Mac) modifier as you click Rescan, Live discards the entire plug-in database and performs a fresh scan from scratch.

### 23.3.1 Plug-Ins in the Device View

VST Plug-Ins in the Device View.

After you drag a plug-in out of the browser onto a track, it appears in the Device View. When a plug-in exposes up to 64 adjustable parameters, a Live panel shows every one of them as horizontal sliders. Anything with more than 64 parameters opens to a blank panel, which you then set up to display whichever parameters you need to reach. You can also have the plug-in's native interface [opened in a separate window](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#showing-plug-in-panels-in-separate-windows).

The Plug-In Unfold Button.

Toggling the button on the plug-in's title bar lets you show or conceal the plug-in's parameters.

Because the X-Y control field drives two plug-in parameters simultaneously, it works particularly well for live performance. Pick any pair of plug-in parameters for the Live panel X-Y field through the drop-down menus situated right below it.

#### 23.3.1.1 Showing Plug-In Panels in Separate Windows

The Show/Hide Plug-In Window Button.

Clicking the Show/Hide Plug-In Window button brings up a floating window displaying the native VST or Audio Units plug-in panel. Adjusting a parameter in that floating window produces the same result as adjusting it in the Live panel, and the reverse holds too.

A handful of Plug-Ins Settings matter when you deal with plug-in windows:

- When the _Auto-Open Plug-In Windows_ option is turned on, it guarantees that a plug-in window pops open by itself as soon as you load the plug-in onto a track from the browser.
- Switching on the _Multiple Plug-In Windows_ option in the Plug-In Settings lets you have as many plug-in windows visible simultaneously as you want. Even when it's off, holding the Ctrl (Win) / Cmd (Mac) modifier as you open a new plug-in window stops the earlier window(s) from shutting.
- The _Auto-Hide Plug-In Windows_ option lets you restrict Live to showing just the plug-in windows that belong to whichever track is selected at the moment.

To toggle the visibility of open plug-in windows, use the Show/Hide Plug-In Windows command in the View menu or the CtrlAltP (Win) / CmdOptionP (Mac) shortcut. Bear in mind that the shortcut takes effect only when the plug-in windows were opened by hand first, or when the Auto-Open Plug-In Windows option is switched on in Live's Settings. The title bar of an open plug-in window displays the name of the track the plug-in sits on.

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

### 23.3.2 Sidechain Parameters

In the usual case, the audio being processed and the input that triggers the plug-in device are one and the same. Sidechaining, though, lets you process one signal according to the level of a separate signal. On plug-in devices with sidechaining support, the sidechain parameters sit along the left edge of the device.

Plug-In Sidechain Parameters.

Through the choosers you can pick any of Live's internal routing points, making the chosen source the device's trigger in place of the signal actually undergoing processing.

The Gain knob sets the level feeding in from the external sidechain, and the Mix knob lets you blend the sidechain with the original signal to form the trigger. Set Mix to 100% and the sidechain source alone triggers the device; at 0% the sidechain is essentially disabled. Keep in mind that raising the gain doesn't make the source signal louder in the mix. That sidechain audio serves purely as a trigger for the device and is never heard.

With the Mute button you can monitor only what the plug-in device puts out, leaving the sidechain source's input out.

### 23.4 VST Plug-Ins

### 23.4.1 The VST Plug-In Folder

On your initial Live launch, your VST plug-in sources have to be activated before you can work with VST plug-ins. Your platform may also require you to point Live at the VST plug-in folder that holds the devices you intend to use. To configure your VST sources, click the Activate button within the browser's Plug-Ins panel, or bring up the Plug-Ins Settings via Ctrl, (Win) / Cmd, (Mac). The Plug-In Sources section is located there.

The VST Plug-In Sources for Windows.

On Windows, do the following:

1. Point Live at your VST plug-ins through the VST Plug-In Custom Folder entry: click the _Browse_ button, which opens a folder-search dialog where you locate and choose the right folder.
2. After you've chosen a VST Custom Folder and Live finishes scanning it, the path appears. On Windows, keep in mind that Live might have located a path in the registry, sparing you the browsing step.
3. Confirm that the Use VST Plug-In Custom Folder option reads “On,“ which keeps your chosen folder an active VST plug-in source in Live. If you'd rather not use your VST plug-ins in Live, switch the Use VST Plug-In Custom Folder option off.
   The VST Plug-In Sources for macOS.

To configure your VST plug-ins on macOS, do this:

1. Typically your VST plug-ins land in this folder within your home and local directories: /Library/Audio/Plug-Ins/VST. The Use VST plug-ins in System Folders option toggles Live's use of them on or off.
2. You might keep a separate folder for your VST plug-ins (say, the ones reserved for Live). VST plug-ins in that folder can be used alongside the System folder ones or in their place. To point Live at this folder, click the Browse button beside the VST Plug-In Custom Folder entry, opening a folder-search dialog where you locate and choose the right folder.
3. Keep in mind that the Use VST Plug-In Custom folder option lets you switch off the VST plug-ins in this folder.

After your Plug-Ins Settings are configured, the browser shows every plug-in it locates within the chosen VST plug-in folder(s) plus any sub-folders.

You can likewise use VST plug-ins kept in other folders on your machine. To do that, make a macOS or Windows _alias_ of the folder containing the extra VST plug-ins, then drop that alias into the VST Plug-In Custom folder (or, on macOS, the VST Plug-In System folder) chosen in Live's Plug-Ins Settings. An alias may reference a separate partition or drive on your computer. Live scans the designated VST plug-in folder along with any alias folders inside it.

A handful of VST plug-ins are flawed or simply don't work with Live, and during scanning they can crash the program. On your next Live launch, a dialog tells you which plug-in triggered the trouble. Based on what Live determines about it, you may be offered a choice between running another scan or disabling the troublesome plug-in. Pick rescan and have them crash the program again, and Live disables them on its own; they then stay out of the browser and won't be rescanned until you reinstall them.

### 23.4.2 VST Presets and Banks

Each VST plug-in instance “owns“ a _bank of presets_. The intent of a preset is to hold a single full set of values for the plug-in's controls.

Pick a preset out of the plug-in's bank using the chooser beneath the title bar. Each bank holds a fixed count of presets. At any moment you operate “in“ the preset currently chosen, meaning every edit you make to the plug-in's controls folds into that selected preset.

The VST Plug-In Preset Chooser.

Keep in mind that VST presets aren't the same as Live device presets: a Live device's presets are common to all of its instances and Live Sets, whereas VST presets “belong“ to that one particular instance of the VST plug-in.

Rename the active preset by selecting the VST's Device Title Bar and running the Rename Plug-In Preset command from the Edit menu. Then enter a fresh preset name and press Enter to confirm.

Renaming a VST Plug-In Preset.

You can load VST presets and banks in from files. A VST's Load Preset or Bank button opens a standard file-open dialog where you track down the file you want.

On the Left, the VST Load Preset or Bank Button; on the Right, the Save Preset or Bank Button.

_Windows only_: In the Windows dialog, use the File Type filter to indicate whether you're after VST Presets (VST Program Files) or VST Banks (VST Bank Files).

To write the chosen preset out to a file, click the VST Save Preset or Bank button for a standard file-save dialog; in the Format menu (Mac), or alternatively the File Type menu (Windows), pick “VST Preset,“ then choose a folder and a name. Writing out the whole bank as a file works the same way, except you select “VST Bank“ as the file type/format.

### 23.5 Audio Units Plug-Ins

You'll find Audio Units plug-ins on macOS only. For the most part they behave just like VST plug-ins.

An Audio Units Plug-In.

When you first open Live, Audio Units plug-ins are absent from the browser. To enable your Audio Units as a plug-in source, click the Activate button in the browser's Plug-Ins label, or head to the Plug-Ins Settings via Ctrl, (Win) / Cmd, (Mac). The Plug-In Sources section lives there. Switching on the Use Audio Units option enables Audio Units plug-ins so they show up in Live's browser.

Bear in mind you can switch this option off again later if you decide against using Audio Units.

Activating Audio Units Plug-Ins.

Audio Units plug-ins occasionally include a feature for picking among several device modes. You could, for instance, select among different quality levels for how a reverb is rendered. The choosers for these device modes are reachable only via the native plug-in panel, opened through the Show/Hide Plug-In Window button.

Opening an Audio Units Plug-In Window.

Audio Units carry presets that behave exactly like those of the Live effects. That said, certain AU presets are read-only and therefore can't be dragged elsewhere in the browser.

Audio Units presets carry an .au preset extension and reside in the directory below, organized by their manufacturer's name:

(Home)/Library/Audio/Presets/(Manufacturer Name)/(Plug-in Name)

### 23.6 Device Delay Compensation

On its own, Live accounts for the delays introduced by Live and plug-in instruments and effects, the ones on return tracks included. Such delays come from the time a device needs to take in an input signal and produce its result. By keeping Live's tracks aligned, the compensation algorithm cuts the lag between what the player does and what they hear.

Device delay compensation runs by default and usually needs no tweaking at all. If you want to switch latency compensation on (or off) yourself, use the Delay Compensation option found in the Options menu.

With Delay Compensation switched on, the Options menu offers the Reduced Latency When Monitoring option. It turns latency compensation on or off for any track that has input monitoring engaged. Switched on, input-monitored tracks reach the smallest latency achievable, yet they can drift out of sync with certain other tracks in your Set, like Return tracks, which remain delay compensated. Switched off, every track lines up, though input-monitored tracks may carry more latency.

Bear in mind that tempo-synced effects and other devices drawing timing from Live's internal clock can drift out of sync when they sit in a device chain downstream of devices that introduce delay.

Abnormally large individual [track delays](https://www.ableton.com/en/live-manual/12/mixing/#track-delays) or latencies reported by plug-ins can make the software feel noticeably sluggish. Should you hit latency trouble while recording and playing instruments back, you could try disabling device delay compensation, although that's generally discouraged. Tweaking the individual track delays may help in such situations too, but note that the Track Delay controls go dark once device delay compensation is switched off.

Bear in mind that, depending on how many tracks and devices are running, device delay compensation can raise the CPU load.
