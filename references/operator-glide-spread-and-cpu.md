# Operator Glide Spread And CPU

Open when you need guidance on Operator Glide Spread And CPU in Ableton Live.

Context: [Operator](meld-and-operator-routes.md#309-operator).

<a id="source-3097-glide-and-spread"></a>
### 30.9.7 Glide and Spread

Operator’s Pitch Display and Shell Parameters.

A polyphonic glide capability is built into Operator. With it switched on, a fresh note begins at the pitch of whatever note preceded it and then glides smoothly toward its own intended pitch. The Glide Time control inside the pitch display switches Glide on or off and sets its behaviour.

There is also a distinctive Spread parameter in Operator, which manufactures a lush stereo chorus by allotting two voices to each note and steering one toward the left while the other goes to the right. Detuning separates these two voices, and the Spread control in the shell's pitch section governs how much detuning is applied.

Whether spread takes effect on any given note is decided by where the Spread parameter sits at the moment of the Note On event. For unusual results, you might, say, build a passage in which Spread stays at 0 for most of the time and is engaged only on certain notes. Those notes alone will sound in stereo, whereas the rest stay mono. Bear in mind that Spread draws heavily on the CPU.

A global Transpose knob is likewise housed in the pitch section.

<a id="source-3098-strategies-for-saving-cpu-power"></a>
### 30.9.8 Strategies for Saving CPU Power

To conserve CPU power, switch off whatever functions you have no use for, or trim the voice count. In particular, deactivating the filter or the LFO whenever they add nothing to the timbre will reclaim CPU power.

To economize on CPU resources, you'll typically also want to bring the voice count down to roughly 6 to 12, and apply the Spread feature sparingly. Switching off the Interpolation and Antialias modes within the global display likewise frees up CPU resources.

Keep in mind that silencing the oscillators does nothing to lower CPU power.

<a id="source-3099-finally"></a>
### 30.9.9 Finally…

Operator grew out of a deep fascination with FM synthesis paired with affection and devotion toward the vintage hardware FM synthesizers — among them the Yamaha SY77, the Yamaha TX81Z and the NED Synclavier II. The first musical investigations of FM synthesis came from composer and computer-music pioneer John Chowning during the mid-1960s. By 1973, he together with Stanford University struck up a partnership with Yamaha, which gave rise to the DX7, among the best-selling commercial musical instruments ever made.

Working from a synthesis idea that you can now investigate firsthand simply by experimenting with Operator in Live, John Chowning brought to life some truly astonishing and gorgeous musical works.

We wish you loads of fun with it!

<a id="source-30910-the-complete-parameter-list"></a>
### 30.9.10 The Complete Parameter List

What every Operator parameter does gets covered in the sections that follow. Bear in mind, too, that within Live itself you can read descriptions of controls (Operator's among them) straight from the application — just hover the mouse above a control and study the wording that shows up in the Info View. The list below organizes parameters into groups according to where they sit inside Operator.
