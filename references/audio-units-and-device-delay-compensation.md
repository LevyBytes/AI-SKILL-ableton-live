# Audio Units And Device Delay Compensation

Open when you need guidance on Audio Units And Device Delay Compensation in Ableton Live.

Context: [Working with Instruments and Effects](working-with-instruments-and-effects.md#23-working-with-instruments-and-effects).

<a id="source-235-audio-units-plug-ins"></a>
### 23.5 Audio Units Plug-Ins

You'll find Audio Units plug-ins on macOS only. For the most part they behave just like VST plug-ins.

An Audio Units Plug-In.

When you first open Live, Audio Units plug-ins are absent from the browser. To enable your Audio Units as a plug-in source, click the Activate button in the browser's Plug-Ins label, or head to the Plug-Ins Settings via Ctrl+, (Win) / Cmd+, (Mac). The Plug-In Sources section lives there. Switching on the Use Audio Units option enables Audio Units plug-ins so they show up in Live's browser.

Bear in mind you can switch this option off again later if you decide against using Audio Units.

Activating Audio Units Plug-Ins.

Audio Units plug-ins occasionally include a feature for picking among several device modes. You could, for instance, select among different quality levels for how a reverb is rendered. The choosers for these device modes are reachable only via the native plug-in panel, opened through the Show/Hide Plug-In Window button.

Opening an Audio Units Plug-In Window.

Audio Units carry presets that behave exactly like those of the Live effects. That said, certain AU presets are read-only and therefore can't be dragged elsewhere in the browser.

Audio Units presets carry an .au preset extension and reside in the directory below, organized by their manufacturer's name:

(Home)/Library/Audio/Presets/(Manufacturer Name)/(Plug-in Name)

<a id="source-236-device-delay-compensation"></a>
### 23.6 Device Delay Compensation

On its own, Live accounts for the delays introduced by Live and plug-in instruments and effects, the ones on return tracks included. Such delays come from the time a device needs to take in an input signal and produce its result. By keeping Live's tracks aligned, the compensation algorithm cuts the lag between what the player does and what they hear.

Device delay compensation runs by default and usually needs no tweaking at all. If you want to switch latency compensation on (or off) yourself, use the Delay Compensation option found in the Options menu.

With Delay Compensation switched on, the Options menu offers the Reduced Latency When Monitoring option. It turns latency compensation on or off for any track that has input monitoring engaged. Switched on, input-monitored tracks reach the smallest latency achievable, yet they can drift out of sync with certain other tracks in your Set, like Return tracks, which remain delay compensated. Switched off, every track lines up, though input-monitored tracks may carry more latency.

Bear in mind that tempo-synced effects and other devices drawing timing from Live's internal clock can drift out of sync when they sit in a device chain downstream of devices that introduce delay.

Abnormally large individual [track delays](https://www.ableton.com/en/live-manual/12/mixing/#track-delays) or latencies reported by plug-ins can make the software feel noticeably sluggish. Should you hit latency trouble while recording and playing instruments back, you could try disabling device delay compensation, although that's generally discouraged. Tweaking the individual track delays may help in such situations too, but note that the Track Delay controls go dark once device delay compensation is switched off.

Bear in mind that, depending on how many tracks and devices are running, device delay compensation can raise the CPU load.
