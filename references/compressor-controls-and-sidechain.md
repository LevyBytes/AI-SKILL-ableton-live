# Compressor Controls And Sidechain

Open when you need guidance on Compressor Controls And Sidechain in Ableton Live.

Context: [Live Audio Effect Reference](amp-filter-and-pan-routes.md#28-live-audio-effect-reference).

<a id="source-289-compressor"></a>
### 28.9 Compressor

The Compressor Effect.

<a id="source-live-audio-effect-reference-part-3"></a>

Whenever a signal climbs past a threshold you choose, a compressor pulls its gain back down. Because the loudest peaks get tamed, additional headroom appears, which lets you raise the level of the whole track. The result is a higher average loudness, and the ear tends to perceive that as a fuller, more forceful sound compared to material left uncompressed.

The Threshold and the compression Ratio rank as the two settings that matter most on any compressor.

Where compression kicks in is governed by the Threshold slider. Anything louder than that point gets pulled down by a degree that the Ratio parameter controls, since Ratio fixes the relationship between input and output. Take a compression ratio of 3 as an example: a 3 dB rise on an input that sits above the threshold yields only a 1 dB rise at the output. Likewise, a 6 dB input rise above the threshold produces just 2 dB more at the output. Set the ratio to 1 and you get no compression at all, whatever the threshold happens to be.

At any instant, the orange Gain Reduction meter reports the current amount of gain being pulled down. Heavier reduction makes the processing more obvious; pushing past roughly 6 dB of gain reduction may hit the loudness you wanted, yet it noticeably reshapes the tone and can wreck the dynamic structure. Once that damage is done, no later stage of production will bring it back. Bear that in mind in particular if you place a compressor, limiter, or loudness-maximizing device on the Main track. Restraint usually pays off in those situations.

Since compression trims the loud parts and frees up headroom, the Output (Out) control lets you push the peaks back up to the top of the available headroom. Output level is displayed on the Output meter. Switch on the Makeup button and Live will adjust the output level for you whenever you change the threshold or ratio.

The blend of processed and unprocessed audio is set by Dry/Wet. Set it to 100% and you hear only the compressed signal; pull it to 0% and the device essentially does nothing.

How smoothly or sharply compression sets in as the signal nears the threshold is shaped by the Knee control. At 0 dB, nothing below the threshold is touched and anything reaching or passing it is compressed in full. Paired with steep ratios, this so-called ”hard knee” response can come across as harsh. Raise the knee toward ”soft” values and compression eases in progressively as the signal approaches the threshold. Picture a 10 dB knee combined with a -20 dB threshold: gentle compression starts around -30 dB and ramps up so that, by -10 dB, the signal is being fully compressed.

Using the switches tucked into the lower corners of the display, you can flip Compressor’s display among several modes:

- The _Collapsed_ view exposes nothing but the core controls.
  Compressor’s Collapsed View.
- The _Transfer Curve_ plots input level across the horizontal axis and output level up the vertical one. It comes in handy for dialing in the Knee parameter, which appears as two dotted lines flanking the threshold.
  Compressor’s Transfer Curve.
- The _Activity_ view draws the incoming signal’s level in light gray. Here the GR and Output switches let you swap between displaying gain reduction in orange and showing the output level in a darker shade of gray. Such views help you picture how the signal evolves moment to moment.
  Compression Activity Display, Showing Input and Output.

By setting how quickly Compressor responds to shifts in the input level, the Attack and Release controls govern its timing behavior, which makes them critical parameters.

Once a signal passes the threshold, Attack governs the time needed to reach full compression, whereas Release governs how long the compressor takes to ease back to its resting state after the signal drops under the threshold. Switch on Auto Release and the release time recalibrates on its own according to the audio coming in.

Giving the attack a modest value (10-50 ms) lets peaks slip through untouched, which preserves dynamics by emphasizing the leading edge of each sound. Should those peaks trigger overloads, shortening the attack can help, though very brief settings drain the ”life” out of the audio and can introduce a faint “buzziness” from distortion. Brief release values can bring on ”pumping” while the compressor wavers over whether or not to clamp down; usually treated as a flaw, this is nonetheless something some engineers deliberately apply to full drum kits for odd ”sucking” textures. Dialing attack and release in carefully really matters when you are compressing rhythmic material. New to compressors? Loop a drum part and experiment for a while with Attack, Release, Threshold and Gain. The process can be a lot of fun!

A compressor has nothing to act on until the input signal actually arrives. Because it also has to impose an attack/release envelope, its response inevitably lands slightly behind the beat. The digital fix is straightforward: hold the incoming signal back by a tiny margin. Compressor provides three Lookahead settings to do this: zero ms, one ms and ten ms. Depending on which you pick, the outcome can sound noticeably different.

Three core operating modes are available on Compressor. Choose Peak and Compressor responds to brief spikes inside a signal. Being sharper and more exact, this mode suits limiting jobs where you must guarantee nothing whatsoever exceeds the threshold you set. Pick RMS and Compressor grows less reactive to fleeting peaks, clamping down only after the level has stayed over the threshold for a marginally longer stretch. Since RMS tracks loudness more like the human ear does, it is generally felt to be more musical. With Expand mode you dial in the expansion ratio between input and output. As an illustration, a 1 to 2 ratio means each 1 dB the input sits above the threshold turns into a 2 dB rise at the output. Set it to 1 to 1 and no expansion takes place. To read more about the different categories of dynamics processing, refer to the [Multiband Dynamics](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#multiband-dynamics) section.

Beyond those modes, Compressor lets you pick between two envelope-follower shapes, giving you extra say over how the device gauges and tracks signal levels. Under linear (Lin) mode, the Attack and Release values alone dictate how fast compression responds. Switch to logarithmic (Log) mode and heavily compressed peaks recover faster than gently compressed passages. The upshot can be smoother, less obtrusive compression than Lin offers. Keep in mind that the Lin/Log switch stays hidden while Compressor is collapsed.

<a id="source-2891-sidechain-parameters"></a>
### 28.9.1 Sidechain Parameters

The Compressor Device With Sidechain Section.

In the usual case, the audio being compressed and the source that triggers the compressor are one and the same. Through _sidechaining_, though, you can drive compression on one signal from the level of a different signal or even a particular frequency component. Reach the Sidechain parameters by expanding the Compressor window via the button on its title bar.

Two halves make up the sidechain parameters. The external controls sit on the left side. Switch that part on with the Sidechain button and you can pick any of Live’s [internal routing points](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#internal-routing-points) from the choosers underneath. The chosen source then becomes what triggers the compressor, in place of the audio currently being compressed.

Level of the external sidechain’s input is handled by the Gain knob, and the Dry/Wet knob lets you blend the sidechain with the original signal as the compressor’s trigger. Push Dry/Wet to 100% and only the sidechain source drives the compressor. Drop it to 0% and the sidechain is essentially out of the picture. Bear in mind that turning up the gain does _not_ make the source signal louder in the mix. That sidechain audio merely triggers the compressor; it is never heard on its own.

Keep in mind that automatic Makeup cannot be used together with an external sidechain.

The sidechain EQ controls occupy the right portion of the external section. Switch this part on and the compressor responds to a chosen band of frequencies rather than the whole signal. Those frequencies may live within the compressed signal itself, or — when you pair the EQ with an external sidechain — within the audio of a different track.

Sitting between the external and EQ sections, the headphones button lets you monitor the sidechain input alone while muting the compressor’s output. Because that sidechain audio never reaches the output and only serves to trigger the compressor, this brief monitoring mode makes it far simpler to dial in sidechain parameters and hear exactly what is driving the compressor.

<a id="source-2892-compressor-tips"></a>
### 28.9.2 Compressor Tips

What follows are a few pointers for getting the most out of Compressor, with special attention to the sidechain features.
