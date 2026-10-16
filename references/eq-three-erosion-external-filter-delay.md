# EQ Three Erosion External Filter Delay

Open when you need guidance on EQ Three Erosion External Filter Delay in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2816-eq-three"></a>
### 28.16 EQ Three

The EQ Three Effect.

Anyone who has worked with a decent DJ mixer will recognize this: an EQ that lets you independently set the level of the low, mid and high frequencies.

The gain controls let you set each band anywhere from -infinite dB up to +6 dB. That makes it possible to fully strip out, say, the bass drum or bassline of a track while keeping the rest of the frequencies intact.

You can also switch each band on or off via the On/Off buttons sitting beneath the gain controls. Those buttons come in especially handy when mapped to computer keys.

EQ Three offers a visual cue for whether a signal is present in each frequency band through three LEDs. Even with a band switched off, you can still spot whether anything is happening in it. The LEDs’ internal threshold is fixed at -24 dB.

Two crossover controls, FreqLo and FreqHi, set the frequency span of each band. With FreqLo at 500 Hz and FreqHi at 2000 Hz, the low band spans 0 Hz to 500 Hz, the mid band spans 500 Hz to 2000 Hz, and the high band runs from 2000 Hz on up to whatever ceiling your soundcard or sample rate allows.

The 24 dB/48 dB switch is a particularly significant control. It governs how steeply the filters cut the signal at the crossover frequency. Choosing the higher setting gives more aggressive filtering but demands more CPU.

Note: The filters inside this device are voiced to act less like a clean digital filter and more like a robust, capable analog filter cascade. In particular, the 48 dB Mode doesn’t reach a perfectly linear transfer quality, so a touch of coloration enters the input signal even with every control parked at 0.00 dB. That’s normal for a filter of this sort and forms part of what gives EQ Three its distinctive sound. Should you require more linear behavior, opt for 24 dB Mode or turn to the EQ Eight.

<a id="source-2817-erosion"></a>
### 28.17 Erosion

The Erosion Effect.

Erosion applies digital degradation to the input signal by modulating a brief delay with a mix of a sine wave and filtered noise. The outcome can range from noisy artifacts all the way to distortions reminiscent of downsampling.

During playback the input signal’s frequency spectrum appears in the display, accompanied by a visual depiction of the modulation. That display doubles as an X-Y controller you can use to set the Freq and Amount controls. Drag horizontally along the X-axis to alter the sine wave frequency and the noise filter’s center frequency. Drag vertically along the Y-axis to govern the modulation amount. Holding Alt (Win) / Option (Mac) instead lets you set the filter width of the noise modulation on the Y-axis. Note that the filter width does nothing when only sinusoidal modulation is in use.

Noise Blend sets how the sinusoidal and noise modulation carriers get mixed. At 0%, the input signal is modulated by a sine wave alone, whereas at 100%, only noise does the modulating. The sine wave and noise icons under the display shift in brightness as you change the blend, signaling which modulation carrier dominates. Within the display, the sinusoidal modulation appears as a solid vertical line while the noise modulation appears as horizontal dotted lines.

The Filter Width control sets the bandwidth of the noise filter. Smaller values yield a tighter frequency range, whereas larger values stretch it over a broader slice of the spectrum. Note that with Noise Blend at 0%, the Filter Width control is grayed out, since it does nothing to the sinusoidal modulation.

The Stereo Width control lets you shift the modulation source from mono (0.0%) toward stereo (100%). Larger values introduce a gentle stereo widening to the modulation.

Any Sets built before 12.4 containing Erosion will open the older form of the device, which now goes by Erosion Legacy.

<a id="source-2818-external-audio-effect"></a>
### 28.18 External Audio Effect

The External Audio Effect.

The External Audio Effect stands somewhat apart from Live’s other effect devices. Rather than processing audio on its own, it lets you bring _external_ (hardware) effects processors into a track’s device chain.

The Audio To chooser picks which outputs on your computer’s audio hardware feed your external device, while the Audio From chooser picks which inputs carry the processed signal back into Live. Just as with the track inputs and outputs, which inputs and outputs are available hinges on the Audio Settings, reachable through the ”Configure…” option at the foot of each chooser.

Each chooser has a Peak level indicator below it that reports the highest audio level reached. Click the indicators to clear them.

The Gain knobs beside the choosers govern the levels leaving and re-entering Live. Set these carefully to keep from clipping, both inside your external hardware and as the audio returns to your computer.

The balance between the processed and dry signals is set by the Dry/Wet control. Take it to 100 percent whenever you use the External Audio Effect on a return track.

The Invert button reverses the phase of the processed signal as it comes back into Live.

Because hardware effects add latency that Live has no way to detect on its own, you can offset any delays by hand using the Hardware Latency slider. The button beside that slider lets you express your latency compensation amount in either milliseconds or samples. When your external device links to Live through a digital connection, set your latency in samples, which guarantees the sample count you enter stays put even after a sample rate change. When your external device links to Live through an analog connection, set your latency in milliseconds, which guarantees the time amount you enter stays put after a sample rate change. Keep in mind that working in samples affords finer control, so even with analog devices you might choose to ”fine tune” your latency in samples to reach the lowest achievable latency. Just remember to flip back to milliseconds before you change your sample rate.

Note: Should the [Delay Compensation](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#device-delay-compensation) option sit unchecked within the Options menu, then the Hardware Latency slider becomes unavailable.

For step-by-step guidance on dialing in accurate latency compensation for your hardware, please consult the [Driver Error Compensation FAQ article](https://help.ableton.com/hc/en-us/articles/115000234830-Driver-Error-Compensation-FAQ) in the Knowledge Base.

<a id="source-2819-filter-delay"></a>
### 28.19 Filter Delay

The Filter Delay Effect.
