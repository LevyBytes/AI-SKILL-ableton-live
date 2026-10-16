# Plug In Formats And Setup

Open when you need guidance on Plug In Formats And Setup in Ableton Live.

Context: [Working with Instruments and Effects](working-with-instruments-and-effects.md#23-working-with-instruments-and-effects).

<a id="source-233-using-plug-ins"></a>
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
