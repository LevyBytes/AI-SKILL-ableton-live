# Multiband Dynamics Theory And Band Controls

Open when you need guidance on Multiband Dynamics Theory And Band Controls in Ableton Live.

Context: [Multiband Dynamics](reverb-limiter-looper-multiband-routes.md#2826-multiband-dynamics).

<a id="source-28261-dynamics-processing-theory"></a>
### 28.26.1 Dynamics Processing Theory

Getting the most out of the Multiband Dynamics device is easier once you grasp the four distinct ways dynamics can be shaped.

“Compression” usually refers to pulling down the level of any signal that climbs past a threshold. That’s exactly what Live’s [Compressor](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#compressor) does, and the more precise name for it is _downward compression_, since it pushes the loud parts down and so narrows the dynamic range. Yet you can shrink the dynamic range the other way too, by lifting the level of signals that sit _below_ a threshold. That far rarer variety goes by the name _upward compression_. The diagram makes it clear that whichever flavor you reach for, the result is a signal with a tighter dynamic range than you started with.

Downward and Upward Compression.

Expansion is compression’s mirror image. A standard expander drops the level of signals falling beneath a threshold. Live’s [Gate](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#gate) operates this way, and is more properly termed _downward expansion_, because it pushes the quiet bits down and thereby widens the dynamic range. You can also stretch the dynamic range by boosting signals that rise _above_ a threshold. Mirroring upward compression, this approach is called _upward expansion_ and shows up far less often. The diagram illustrates that either kind of expansion leaves you with a wider dynamic range.

Downward and Upward Expansion.

In short:

- Downward compression (common): make loud signals quieter
- Upward compression (uncommon): make quiet signals louder
- Downward expansion (common): make quiet signals quieter
- Upward expansion (uncommon): make loud signals louder

Every one of these processing types is on offer in the Multiband Dynamics device. Since it splits the incoming audio into three frequency bands and gives each band an upper plus a lower threshold, one instance of Multiband Dynamics can run six kinds of dynamics processing all at the same time.

<a id="source-28262-interface-and-controls"></a>
### 28.26.2 Interface and Controls

Toggling the high and low bands on or off is done with the High and Low buttons. Switch both off and the device collapses to a single-band effect, where only the Mid controls touch the signal. Sitting under the High and Low buttons, the frequency sliders move the crossovers that mark out each band’s range. Say the low frequency reads 500 Hz and the high frequency reads 2000 Hz: the low band then spans 0 Hz to 500 Hz, the mid band 500 Hz to 2000 Hz, and the high band runs from 2000 Hz on up to whatever ceiling your soundcard or sample rate allows.

<a id="source-live-audio-effect-reference-part-7"></a>

Every band is equipped with both an activator and a solo button. When the activator button is switched off for a particular band, that band's gain controls along with its compression/expansion are skipped. Putting one band into solo silences all the rest. Ahead of dynamics processing, the Input knobs raise or lower each band's level, whereas the Output knobs sitting to the right of the display set the band levels once processing has occurred.

The display area lets you both watch your dynamics processing in action and tune the compression and expansion behavior that applies. Within each band, large bars stand in for the output level, whereas small bars stand in for the input level prior to processing. When nothing is being processed, the input meters sit flush with the top edge of the output meters. Along the lower edge of the display, the scale is marked in dB. While you tweak a band's gain or dynamics processing, the display lets you observe how its output shifts relative to its input.

When you drag your mouse across the display, the pointer turns into a bracket whenever it crosses the edges of the blocks at either the left or right side. Those blocks stand for the signal levels falling under the Below threshold and rising over the Above threshold, in that order. Pulling left or right at the edges of these blocks changes the threshold level. Keeping Ctrl (Win) / Cmd (Mac) held during a threshold drag applies the same threshold across every band. Keep Alt (Win) / Option (Mac) held to tune the Above and Below thresholds together for one band. Keeping Shift held while you drag left or right lets you set a single band's threshold with greater precision.

When you hover the pointer over the central part of the block, it becomes an up-down arrow. Drag it up or down to raise or lower the loudness of the signal that falls inside the chosen volume range. Keeping Ctrl (Win) / Cmd (Mac) held while you drag up or down sets that same block's volume on every band. Keep Alt (Win) / Option (Mac) held to tune the Above and Below volumes together for one band. Keeping Shift held while dragging up or down lets you tune a single band's volume with greater precision. A double-click inside the region returns the volume to its default value.

Speaking technically, dropping the volume in the block sitting above the Above threshold yields downward compression, whereas lifting it yields upward expansion. In the same way, dropping the volume in the block sitting below the Below threshold yields downward expansion, whereas lifting it yields upward compression. Across every one of these cases, what you are changing is the compressor or expander ratio.

You can likewise tweak the thresholds and ratios for all bands through the column placed to the right of the display. Per band, the ”T,” ”B” and ”A” buttons in the lower-right corner of the display area cycle the readout through three sets: Time, holding attack plus release; Below, holding threshold plus ratio; and Above, again holding threshold plus ratio.

When dealing with the Above thresholds, Attack determines the time required to hit full compression or expansion after a signal climbs past the threshold, whereas Release determines the time the device needs to come back to normal once the signal sinks beneath the threshold.

When dealing with the Below thresholds, Attack determines the time required to hit full compression or expansion after a signal sinks beneath the threshold, whereas Release determines the time the device needs to come back to normal once the signal climbs past the threshold.

When Soft Knee is switched on, compression or expansion sets in slowly as the signal nears the threshold.

How rapidly Multiband Dynamics tracks level changes is likewise shaped by the RMS/Peak switch. When Peak is chosen, the device responds to brief peaks inside a signal. Choosing RMS mode makes it less reactive to extremely brief peaks and holds off processing until the incoming level has stayed past the threshold for a somewhat longer stretch.

Overall output gain for the device is governed by the global Output knob.

The Time control rescales the lengths of every one of the Attack and Release controls. With this, you can keep the same proportional envelope timing while speeding them all up or slowing them all down together.

Across all bands, the Amount knob controls how strong the applied compression or expansion is. When set to 0%, every compressor/expander runs at an effective ratio of 1, so it leaves the signal untouched.
