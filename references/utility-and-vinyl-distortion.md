# Utility And Vinyl Distortion

Open when you need guidance on Utility And Vinyl Distortion in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-2840-utility"></a>
### 28.40 Utility

The Utility Effect.

Utility handles a number of genuinely handy chores, particularly when paired with other devices.

It carries two independent Phase controls, one per input channel (Left and Right). True to their labels, each one flips the phase of its channel.

Selective handling of a sample’s left and right channels comes from the Channel Mode chooser. Pick Left, for instance, and the right channel is dropped while the left channel feeds both outputs. That helps a great deal when a stereo file holds distinct content on each channel and you only want one of them.

How wide the wet signal spreads is set by the Width control. At 0% you get a mono signal, while figures past 100% push the stereo image wider.

Picking Mid/Side Mode from the Width control’s context menu lets you flip between the Width and Mid/Side controls. Across 0 to 100M, the Mid/Side control behaves as a smooth mono-to-stereo dial. Pushing it to 100M collapses the audio to mono. Settings from 0 up to 100S play up a signal’s stereo or “out of phase” content. At 100S you hear the side signal alone, with the left and right channels sitting 180 degrees out of phase from each other.

Bear in mind that picking either Left or Right in the Channel Mode chooser leaves the Width and Mid/Side controls inactive and grayed out.

Switching on the Mono control folds the stereo input down to mono.

The Bass Mono switch collapses the input’s low frequencies to mono, which keeps low end from coloring oddly when it plays back in mono. The Bass Mono Frequency slider sets that crossover point anywhere from 50-500 Hz.

Turning on Bass Mono Audition leaves only the low frequencies audible, which helps when you dial in the Bass Mono Frequency.

Level of the incoming signal is shaped by the Gain control, spanning -infinite dB to +35 dB. It is handy for automating volume fades on a track while leaving that track’s Volume control open for mix work. Nudging the Gain parameter between -18 and +35 dB with the up and down arrow keys moves it in 1 dB steps; from -18 dB down toward -inf dB, though, the value ramps with a smooth acceleration.

The Balance control places the signal anywhere across the stereo field.

Engaging the Mute button just quiets the arriving signal. A track’s active/mute controls always sit at the very tail of its signal chain. Yet because Utility can go anywhere in a chain, its mute can choke the feed into a delay line or reverb without shutting down those devices’ output tails.

The DC switch strips away DC offsets and ultra-low frequencies sitting well beneath what we can hear. It only changes the sound when a signal actually carries those frequencies and gets hit, after Utility, by nonlinear processing such as compressors or waveshapers.

<a id="source-2841-vinyl-distortion"></a>
### 28.41 Vinyl Distortion

The Vinyl Distortion Effect.

Vinyl Distortion recreates several of the characteristic distortions that crop up while a vinyl record plays back. They stem from the geometric interplay of the stylus and the cut groove. A crackle generator is built in as well, layering noisy artifacts on top.

Even harmonic distortion gets added to the input by the Tracing Model section. Set how much with the Drive knob, or click and drag up and down inside the Tracing Model X-Y display. To shift the distortion’s frequency or ”color,” drag sideways in the X-Y display, or double-click the Freq field and key in a number. Holding Alt (Win) / Option (Mac) while you drag vertically in the X-Y display alters the frequency band’s Q (bandwidth).

Odd harmonics get added to the input by the Pinch Effect section. Such distortions usually land 180 degrees out of phase, which fattens the stereo image. Its controls mirror the Tracing Model’s, yet it puts out a noticeably different tone.

The Drive control raises or lowers the total distortion coming from both the Tracing Model and Pinch.

Two distortion modes are on offer: Soft and Hard. Soft Mode evokes the tone of a dub plate, whereas Hard Mode leans nearer to a typical vinyl pressing.

Whether the Pinch distortion runs in stereo or mono rides on the stereo/mono switch. Leave it on stereo for a lifelike take on vinyl distortion.

The Crackle section seeds the signal with noise, its thickness governed by the Density control. The Volume control dials how much gain hits that noise.
