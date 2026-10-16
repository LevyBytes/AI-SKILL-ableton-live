# Auto Filter Circuits Global And Sidechain

Open when you need guidance on Auto Filter Circuits Global And Sidechain in Ableton Live.

Context: [Auto Filter](amp-filter-and-pan-routes.md#282-auto-filter).

<a id="source-2825-filter-drive-and-circuits"></a>
### 28.2.5 Filter Drive and Circuits

Filter Drive and Circuit Controls.

The Drive control lets you push extra input drive into the signal ahead of the filter. This comes in handy for introducing distortion to the signal. At 0.0% the sound stays untouched, growing steadily more distorted and saturated as the Drive setting climbs.

Auto Filter’s filter circuit types capture the personality of assorted analog filter designs. With the Filter Circuit chooser, pick a type from these: SVF, DFM, MS2, and PRD. Note that the filter circuits matter only alongside the Low-pass, High-pass, Band-pass, Notch, and Morph filters.

The SVF circuit option behaves as a clean filter, yet it can also bring in distortion when Drive sits above zero.

DFM routes more of its own distortion back through itself, giving a wide span of tones reaching from gentle filter sweeps to warm drive.

The MS2 circuit relies on a Sallen-Key design plus soft clipping to keep resonance in check. It is modeled on the filters found in a renowned semi-modular Japanese monosynth.

PRD draws on a ladder design and applies no deliberate resonance limiting. It is modeled on the filters found in a legacy dual-oscillator monosynth from the United States.

<a id="source-2826-global-controls"></a>
### 28.2.6 Global Controls

Global Controls in Auto Filter.

The Clip toggle lets you apply soft clipping to whatever the effect outputs. This can help rein in any peaks that arise from high resonance settings. The LED beside the toggle blinks any time the signal clips.

The Output slider fixes how loud the processed signal is at the device’s output. It lets you offset jumps in loudness, which proves handy when you run high Drive settings.

Dry/Wet sets the mix between the processed and unprocessed signals.

<a id="source-2827-sidechain-parameters"></a>
### 28.2.7 Sidechain Parameters

Out of the box, Auto Filter draws on its own input source to drive the envelope follower. You can, however, configure the device to follow an external sidechain signal in its place. Reach the external sidechain parameters by clicking the Sidechain Section toggle at the device’s upper left corner.

Auto Filter’s Sidechain Parameters.

Flip on the External toggle to switch on the external sidechain. With it enabled, the External Source chooser lets you name the signal’s source. The External Tapping Point chooser additionally lets you decide whether the signal arrives Pre FX, Post FX, or Post Mixer.

The Mix slider lets you blend the external and internal sidechain signals together as the trigger for the envelope follower. At 100% the envelope follower follows the external sidechain source alone. At 0% only the internal sidechain comes into play.

The SC Gain control lets you set the level arriving from the external sidechain. Note that the sidechain audio merely triggers the envelope follower, so raising the gain does not raise the source signal’s volume.

To audition the sidechain signal, switch on the Sidechain Listen toggle. This overrides Auto Filter’s output and plays the sidechain input straight to your ears, which helps while you adjust sidechain parameters.

The Sidechain Listen Toggle.

The sidechain carries its own dedicated frequency-selective filter, switched on via the SC Filter toggle. Once active, Auto Filter responds solely to the frequency range fixed by the sidechain filter controls.

The Sidechain Filter Frequency control fixes the cutoff frequency of the sidechain filter. With the Type chooser, pick a filter from these: low-shelf, peak, high-shelf, low-pass, band-pass, and high-pass.

The low-shelf filter raises or lowers frequencies beneath the cutoff frequency, leaving those above largely untouched. Rather than rolling off endlessly the way a low-pass does, the response settles onto a steady gain fixed with the Shelf Gain slider. Positive settings lift the signal, while negative settings cut it.

The peak filter raises or lowers frequencies surrounding the cutoff frequency, with frequencies above and below that band increasingly less affected. The Peak Gain slider fixes the degree of boost or cut.

The high-shelf filter raises or lowers frequencies above the cutoff frequency, leaving frequencies beneath the cutoff largely untouched. As with the low-shelf filter, the response settles onto a steady gain fixed with the Shelf Gain slider rather than rolling off without end.

The low-pass filter cuts back frequencies above the cutoff. High-pass lets through frequencies sitting above the cutoff frequency while cutting back the lower ones. Notch cuts back a slim band of frequencies while leaving nearby frequencies mostly untouched. The Sidechain Filter Q slider lets you fix the filter’s bandwidth.
