# External Instrument And Impulse

Open when you need guidance on External Instrument And Impulse in Ableton Live.

Context: [Live Instrument Reference](analog-and-collision-routes.md#30-live-instrument-reference).

<a id="source-306-external-instrument"></a>
### 30.6 External Instrument

The External Instrument.

The External Instrument device is not actually an instrument; it is a routing helper that makes it simple to fold external (hardware) synthesizers and multitimbral plug-ins into your projects. It dispatches MIDI outward and brings audio back.

The two MIDI To choosers pick the destination where the device sends its MIDI data. The upper chooser picks either a physical [MIDI port](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#midi-port-inputs-and-outputs) or a multitimbral plug-in. Pick a MIDI port (for an external synthesizer) and the lower chooser then offers MIDI channel numbers.

Should a different track in your Set hold a multitimbral plug-in, you can pick that track from the upper chooser. Here the lower chooser lets you target a particular MIDI channel inside the plug-in.

The Audio From chooser supplies choices for bringing audio back from the hardware synth or plug-in device. When routing to a hardware synth, use this chooser to pick the ports on your audio interface wired to your synth's output. Which choices appear hinges on what is configured in the Audio Settings.

When routing to a multitimbral plug-in sitting on another track in your Live Set, the Audio From chooser presents the plug-in's auxiliary outputs. Bear in mind the main outputs come through on the track that holds the instrument.

The Gain knob sets the level of audio arriving back from the sound source. Set this level with care so that clipping is avoided.

Because external devices may add latency that Live cannot detect on its own, you can offset any delays by hand using the Hardware Latency slider. The button beside this slider lets you express your latency compensation either in milliseconds or in samples. When your external device links to Live over a digital connection, you should configure latency in samples, so that the sample count you enter holds even as you change the sample rate. When your external device links to Live over an analog connection, you should configure latency in milliseconds, so that the time you enter holds as you change the sample rate. Bear in mind that working in samples affords finer control, so even with analog devices you might choose to “fine tune“ latency in samples to reach the lowest latency achievable. If you do, remember to switch back to milliseconds ahead of changing your sample rate. Live compensates automatically for any latency that its own internal devices add, so the slider is disabled whenever the External Instrument Device routes internally.

Note: Should you leave the [Delay Compensation](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#device-delay-compensation) option unticked within the Options menu, then the Hardware Latency slider becomes unavailable.

For fuller details on routing setups involving the External Instrument device, consult the [Routing and I/O](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#routing-and-io) chapter.

<a id="source-307-impulse"></a>
### 30.7 Impulse

The Impulse Instrument.

Impulse is a drum sampler offering sophisticated modulation features. The eight drum samples placed in Impulse's sample slots can be time-stretched, filtered, and shaped by envelope, saturation, pan, and volume components, almost all of which respond to random and velocity-driven modulation.
