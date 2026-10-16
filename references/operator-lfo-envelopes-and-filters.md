# Operator LFO Envelopes And Filters

Open when you need guidance on Operator LFO Envelopes And Filters in Ableton Live.

Context: [Operator](meld-and-operator-routes.md#309-operator).

<a id="source-3093-lfo-section"></a>
### 30.9.3 LFO Section

Operator’s LFO Display and Shell Parameters.

It’s fair to treat Operator’s LFO as a fifth oscillator of sorts. Running at audio rates, it modulates the frequency of the remaining oscillators. The Dest. A buttons in the LFO’s display let you arm or disarm that modulation per oscillator (and for the filter too), while the Dest. A slider sets how hard the LFO hits those destinations. Should you not need it, the LFO can be shut off outright.

A second destination opens up through the Dest. B chooser, letting the LFO drive one more parameter, with the Dest. B slider controlling how strong that modulation is.

For waveforms, the LFO presents the usual LFO shapes plus sample and hold (S&H) and noise. Sample and hold grabs random values at the LFO’s rate, stepping randomly in a way that suits classic retro-futuristic sci-fi sounds. The noise waveform amounts to nothing more than band-pass filtered noise.

Tip: FM synthesis is great for cooking up percussion, and pairing the LFO with its noise waveform is the secret behind convincing hi-hats and snares.

The LFO’s frequency comes from the LFO Rate control in the shell together with the low/high/sync position of the neighboring LFO Range chooser. That frequency can lock to note pitch, stay fixed, or land anywhere between, as dictated by the Rate < Key parameter in the LFO’s display. Enable the R (Retrigger) button and the LFO returns to the same phase point with every note; disable R and it free-runs.

Overall LFO strength is governed by the LFO Amount control in the shell, which scales the Dest. A and B amounts alike and can itself bend to note velocity through the display’s Amt < Vel control. On top of that, the LFO’s own envelope shapes its intensity.

<a id="source-3094-envelopes"></a>
### 30.9.4 Envelopes

Operator’s Oscillator B Envelope.

Operator carries seven envelopes in all: one per oscillator, plus a filter envelope, a pitch envelope and one for the LFO. Every envelope sports a set of special looping modes, and on top of that the filter and pitch envelopes let you adjust their slopes.

Six parameters define each oscillator’s volume envelope: three rates paired with three levels. A rate measures how long the journey from one level to the next takes. Take a stereotypical pad: it opens at the initial level “-inf dB“ (i.e., silence), climbs at an attack rate to its peak, eases down to the sustain level at a decay rate, and at last — once Note Off arrives — falls back to “-inf dB“ at the release rate. Operator’s display sketches out the real shape of whichever envelope you’re viewing and lets you reshape the curve directly by grabbing a breakpoint and dragging. A clicked breakpoint stays selected afterward, so you can nudge it with the keyboard’s cursor keys whenever that’s easier.

The Envelope Display’s context menu lets you copy an envelope shape from one Operator oscillator and paste it onto another.

As noted above, the filter and pitch envelopes carry adjustable slopes too. Click the diamonds sitting between breakpoints to bend the slope of each envelope segment. A positive slope makes the envelope race ahead at first and then ease off; a negative slope holds it flat for a while before it accelerates toward the end. Set the slope to zero and the segment runs linearly, advancing at one constant rate the whole way.

FM synthesis can yield breathtaking, never-ending, shape-shifting sounds, and looping envelopes are the trick behind them. Flip Loop Mode on down in the display’s lower-left corner. When an Operator envelope set to Loop Mode hits sustain level while the note is still held, it fires again, and the Loop Time parameter sets how fast that cycle runs. Bear in mind that Loop Mode envelopes can recycle extremely quickly, opening the door to effects you’d rarely associate with an ordinary envelope generator.

Loop Mode suits textures and experimental tones, but Operator throws in Beat and Sync Modes for an easy route to rhythmic material. Choose Beat Mode and the envelope restarts after the beat interval picked from the Repeat chooser. Here the repeat interval is measured in fractions of song time, yet notes themselves go unquantized — play one slightly off the grid and it repeats flawlessly while staying off the grid. Sync Mode behaves differently: its first repeat snaps to the nearest 16th note, which in turn locks every later repeat to the song tempo. Remember that Sync Mode is only active while the song plays; otherwise it falls back to Beat Mode behavior.

So it won’t click audibly by jumping back to its initial level, a looped envelope picks up from its current level and climbs at the set attack rate toward peak.

There’s also a mode named Trigger, perfect for percussive material. With it engaged, Note Off is disregarded, so how long you hold a key makes no difference to the sound’s duration.

Every Operator envelope’s rates can be scaled together by the Time control in the shell’s global section. Note that the beat-time figures used in Beat and Sync Modes sit outside the reach of that global Time parameter. Note pitch can further bend envelope rates through the Time < Key parameter in the global section’s display, and a single envelope’s rate can also respond to velocity via the Time < Vel parameter. Combine these with the loop feature and you can conjure exceedingly intricate results…

Arm or disarm the pitch envelope per oscillator and for the LFO with the Destination A-D and LFO buttons in its display. The Dest. A slider sets how strongly that envelope modulates those destinations, and the switch in the shell’s pitch section can shut the envelope off entirely.

Just like the LFO, the pitch envelope can reach a second parameter chosen through the Dest. B chooser, with the modulation strength set by the Amt. B slider together with the main Pitch Env value.

Both the pitch and filter envelopes include one more parameter, End, which sets the level the envelope heads toward once the key is let go; the release time governs how fast that final segment travels.

Tip: Aim a looping pitch envelope solely at the LFO and it effectively becomes a second LFO modulating the first one’s rate. And because the LFO’s own envelope can loop as well, it can act as a third LFO driving the intensity of the first!

<a id="source-3095-filter-section"></a>
### 30.9.5 Filter Section

Operator’s Filter Display and Shell Parameters.

Operator’s filters earn their keep by reshaping the harmonically dense timbres the oscillators throw off. And because those oscillators also hand you the staple waveforms of analog synths, rolling a subtractive synthesizer out of them is a breeze.

The lineup of filter types in Operator spans low-pass, high-pass, band-pass, notch, and the distinctive Morph filter. Any of them can flip between 12 and 24 dB slopes and tap a range of analog-modeled circuit behaviors — crafted together with Cytomic — that recreate the hardware filters of certain vintage analog synthesizers.

The Clean circuit option is a polished, CPU-thrifty design identical to the filtering in [EQ Eight](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#eq-eight), and it covers every filter type.

The OSR circuit option is a state-variable design whose resonance is reined in by a distinctive hard-clipping diode. Drawn from a fairly uncommon British monosynth, it works with all filter types.

The MS2 circuit option leans on a Sallen-Key topology with soft clipping to cap resonance. Based on a celebrated semi-modular Japanese monosynth, it serves the low-pass and high-pass filters.

The SMP circuit is a bespoke design tied to no specific hardware. Blending traits of the MS2 and PRD circuits, it is on hand for the low-pass and high-pass filters.

The PRD circuit follows a ladder design with no built-in resonance ceiling. Modeled after a vintage dual-oscillator monosynth out of the United States, it’s offered for the low-pass and high-pass filters.

Front and center among the filter parameters sit the familiar synth controls Frequency and Resonance. Frequency picks the spot in the harmonic spectrum where the filter acts, and Resonance lifts the frequencies clustered around it.

Run the low-pass, high-pass, or band-pass filter through any circuit other than Clean and an extra Drive control appears, ready to pour gain or distortion into the signal just before it reaches the filter.

A Morph control unique to the Morph filter glides the filter type smoothly from low-pass into band-pass, on to high-pass, through notch, and back round to low-pass.

The Morph slider’s context menu carries dedicated entries that snap the Morph control straight to a low-pass, band-pass, high-pass, or notch position.

Within the filter section’s display, the Envelope and Filter buttons flip the view between the filter envelope and the filter’s frequency response. You can set filter cutoff frequency and resonance from the shell or by dragging the response curve right in the display. Several sources can additionally modulate filter frequency:

- Note velocity, through the filter display’s Freq < Vel control.
- Note pitch, through the filter display’s Freq < Key control.
- Filter envelope, through the filter display’s Envelope control.
- LFO, either by switching on the Dest. A “FIL“ button in the LFO’s display or by pointing Dest. B at Filter Freq.

Right-click the Frequency knob and the context menu offers “Play by Key.“ Choosing it sets the filter up for ideal key tracking in one move, pushing Freq < Key to 100% and parking the cutoff at 466 Hz.

You can also send the filter’s output into a waveshaper, picking its curve from the Shaper chooser. The Shaper Drive (Shp. Drive) slider raises or lowers the level feeding that waveshaper, and the Dry/Wet control balances the untouched signal against the processed one. Drop it to 0% and the shaper along with its drive parameters drops out of the path.
