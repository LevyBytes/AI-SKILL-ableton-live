# Live Instrument Reference (part 5)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

The Plate Resonator filter feeds the incoming signal through a bank of modal resonators tuned to a rectangular plate’s first 32 modes. Its macro knobs let you reshape the plate’s size, resonance, and dimension ratio. Switching on Filter Scale Awareness keeps the filter’s resonant peaks locked to scale.

The Membrane Resonator filter feeds the incoming signal through a bank of modal resonators tuned to a circular membrane’s first 32 modes. Its macro knobs let you reshape the membrane’s size, resonance, and high frequency damping. Switching on Filter Scale Awareness keeps the filter’s resonant peaks locked to scale.

### 30.8.10 Mix Section

Mix Controls for Each Engine.

Within Meld’s Mix section, every engine carries its own Volume and Pan controls plus a dedicated Tone Filter. Volume governs how loud that engine plays overall, while Pan places it left or right within the stereo image.

Think of Meld’s Tone Filter control as a high-pass and low-pass pair rolled together. Push it into positive territory and an engine’s lows are cut back; pull it negative and the engine’s highs are trimmed instead.

Pressing the Limit button engages Meld’s onboard limiter. Once on, it acts per voice — running only after the two engines are combined and the global Drive amount has taken effect. Use it to rein in Meld’s total output whenever both engines are sounding together.

### 30.8.11 Global Controls

Meld’s Global Parameters.

Shaping the instrument’s broad sound and behavior is the job of Meld’s global controls.

Flip Meld’s Mono/Poly switch to choose between monophonic and polyphonic output.

With Mono selected, you gain access to the Legato switch. Turn Legato on and a fresh note struck over a still-held one borrows that earlier note’s envelope, picking it up wherever it currently sits. Turn Legato off and every fresh note fires its own envelope right from the start.

Choosing Poly reveals a drop-down menu for dialing Meld’s available voice count anywhere from 2 to 12.

The Spread control sets how wide the Spread modulation source reaches inside Meld’s Modulation Matrix. With a voice count chosen in the Stacked Voices control, Spread introduces an offset from one stacked voice to the next. With Stacked Voices set to Off, it instead spreads a range of values across each note of a sustained chord. Keep in mind that Spread does nothing unless it is routed to a modulation target in the Modulation Matrix.

Use the Stacked Voices drop-down menu to choose how many stacked voices a single note spawns. Because stacked voices clone both engines per note — filters, modulation, and mixer settings included — they can place a heavy CPU load on your system.

How much saturation hits Meld’s output is governed by the Mixer Drive control. Drive operates per voice, kicking in after mixer settings yet ahead of the limiter.

Meld’s output level is set by the Volume control.

Click the Use Current Scale button and Meld will track Live’s Scale Mode. With it engaged, Meld’s oscillators conform to Live’s active scale, so every transposition — the Pitch Quant modulation target in the Modulation Matrix among them — happens in scale degrees instead of semitones.

### 30.9 Operator

The Operator Instrument.

Operator is a deep, versatile synthesizer that marries “frequency modulation“ (FM) to traditional subtractive and additive techniques. Four multi-waveform oscillators sit at its core, each able to modulate the others’ frequencies and so wring richly intricate timbres out of relatively few building blocks. Rounding out the instrument are a filter section, an LFO and global controls, plus dedicated envelopes for the oscillators, filter, LFO and pitch.

### 30.9.1 General Overview

Operator’s layout breaks into two zones: a central display flanked on both sides by the shell. The shell gathers the headline parameters into one view and splits into eight sections — four oscillator sections down the left, while the right-hand column descends through the LFO, then the filter section, next the pitch section, and finally the global parameters. Touch any shell parameter and the central display jumps automatically to that section’s details. While building a patch, for instance, the shell lets you reach every oscillator’s level and frequency at a glance, after which each oscillator’s display hands you its envelope, waveform and remaining parameters.

A triangular button at Operator’s top left folds the instrument away — handy whenever the display details aren’t needed.

Operator Folded.

Every Operator oscillator may send its signal straight out or route it into another oscillator as a modulator. To wire them together, Operator supplies eleven preset algorithms. You pick one by clicking a structure icon in the global display, which surfaces once the shell’s lower-right (global) section is active. Within an algorithm icon, signal travels from the top oscillator down to the bottom. Like any other parameter, the algorithm selector accepts MIDI controller mappings, automation, or live modulation.

Operator’s Algorithms.

Classic FM synthesis usually starts from clean sine waves and builds richer spectra through modulation. To make sound design easier and to widen the palette, though, we equipped Operator with a range of additional waveforms, two flavors of noise among them. A partial editor even lets you sketch waveforms of your own. An LFO, a pitch envelope and a filter section finish off the instrument. Bear in mind that plenty of “classic“ FM synths produce wonderful results with no filter whatsoever, so we’d suggest poking around in filter-free FM first and only reaching for the filter afterward if you need it.

Anyone keen to go deep into sound design will find Operator endlessly absorbing! And if you’d like to take the universe apart and put it back together, try driving Operator’s controls from [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#clip-envelopes) or [track automation](https://www.ableton.com/en/live-manual/12/automation-and-editing-envelopes/#automation-and-editing-envelopes).

### 30.9.2 Oscillator Section

Oscillator A’s Display and Shell Parameters.

#### 30.9.2.1 Built-in Waveforms

Each oscillator ships with a stock set of fundamental waveform types — sine, sawtooth, square, triangle and noise — picked from the Wave chooser inside the individual oscillator displays. Leading the list is a pure, mathematical sine wave, the go-to starting point for a great many FM timbres. We threw in “Sine 4 Bit“ and “Sine 8 Bit“ as well, delivering the retro flavor that C64 fans cherish, alongside the “Saw D“ and “Square D“ digital waveforms that excel at digital bass sounds. The square, triangle and sawtooth options are resynthesized stand-ins for their ideal counterparts. Whatever number rides along in the displayed name (say, “Square 6“) tells you how many harmonics drive that resynthesis. Smaller counts come across as mellower and are far less prone to aliasing up in the high register. Two noise waveforms round things out: “Noise Looped,“ which is a looped chunk of noise, and “Noise White,“ which you should reach for when you want genuinely random noise.

#### 30.9.2.2 User Waveforms

Picking the “User“ entry in the Wave chooser lets you build waveforms from scratch by drawing the amplitudes of the oscillator’s harmonics. Equally, you can grab one of the stock waveforms and reshape it the very same way. A compact display beside the Wave chooser tracks your waveform live as you work.

Hover the mouse across the Oscillator display area and the cursor becomes a pencil. Drawing there pushes the harmonic amplitudes up or down. While you’re shaping them, the Status Bar reports both which harmonic you’re editing and its current amplitude. Hold Shift as you drag to lock the motion horizontally, which lets you tweak a single harmonic’s amplitude on its own.

Switches off to the right of the display let you toggle between editing the first 16, 32 or 64 harmonics. To reach beyond those, the drawn partials can be echoed upward with a tapering fade governed by the Repeat chooser. A low Repeat figure yields a brighter tone, whereas a higher one rolls off more top end and leaves the fundamental more pronounced. Switch Repeat off and any partials past the 16th, 32nd or 64th harmonic are simply cut.

Right-clicking the harmonics display brings up a context menu for restricting edits to just the even or just the odd harmonics; “All“ is the default. That same menu carries a Normalize toggle. Switch it on and the oscillator holds a steady overall output level as you keep adding harmonics; switch it off and each new harmonic piles on more level. Watch out — with Normalize off the volume can climb to extremes.

A context-menu option lets you save your waveform in .ams format into the Samples/Waveforms folder within your User Library. To bring Ams files back into Operator, drag them out of the browser and onto one of the oscillator’s display areas. Those Ams files load into Simpler or Sampler just as readily.

Right-click via the Osc Preview’s context menu to copy and paste either stock or user waveforms from one oscillator to another.

#### 30.9.2.3 More Oscillator Parameters

Dial an oscillator’s frequency from the shell using its Coarse and Fine controls. Ordinarily an oscillator’s frequency tracks the notes you play, yet certain sounds call for pinning one or more oscillators to set frequencies instead. Engage the Fixed option on any individual oscillator to do exactly that. The payoff is a sound whose timbre shifts across the keyboard while its tuning holds steady — Fixed Mode is handy, say, for building live drum sounds. It can also reach down to frequencies as low as 0.1 Hz. Keep in mind that with Fixed Mode on, the oscillator’s frequency is steered from the shell through the Frequency (Freq) and Multiplier (Multi) controls.

Each oscillator also carries a dedicated Osc < Vel control in Operator, letting velocity reshape frequency. That comes in especially handy with sequenced parts, where you can fine-tune every note’s velocity. Riding alongside it is the Q (Quantize) button: switch it on and frequency steps only in whole numbers, exactly as though you were turning the Coarse control by hand. Leave quantize off and frequency glides without snapping, producing detuned or inharmonic results (which might be precisely the effect you’re after…).

An oscillator’s amplitude rests on two things: its Level setting in the shell and its envelope, which appears and can be edited whenever the Envelope display is showing. Those envelopes also respond to note velocity and note pitch through the Vel and Key parameters found in the Envelope section of each oscillator’s display.

Set each oscillator’s phase with the Phase control in its display. Enable the R (Retrigger) button and the waveform snaps back to the same phase position on every note; disable R and the oscillator simply free-runs.

As noted earlier, oscillators can modulate one another once you arrange them with the global display’s algorithms. Where one oscillator modulates a second, the outcome hinges on two factors: how loud the modulating oscillator is and the frequency ratio linking the pair. And any oscillator that nothing else is modulating can feed back on itself through the Feedback parameter in its display.

#### 30.9.2.4 Aliasing

Aliasing distortion turns up across every kind of digital synthesis, stemming from the limited sample rate and precision inherent to digital systems, and it shows itself mainly up high. FM synthesis is a particularly fertile breeding ground for it, since rich stacks of high harmonics come so easily. By the same token, busier oscillator waveforms like “Saw 32,“ prove more aliasing-prone than clean sine waves. The thing cuts both ways: a touch of aliasing can be just the seasoning a cool sound needs, yet too much renders the timbre unplayable, because pitch perception collapses once high notes fold back to arbitrary frequencies. Operator holds aliasing in check with a high-quality Antialias mode, switched on by default for fresh patches but available to disable in the global section. The global section’s Tone parameter offers another handle on aliasing; it can behave somewhat like a low-pass filter, though that varies with the sound and isn’t reliably predictable. To get acquainted with how aliasing sounds, crank Tone all the way up and strike a handful of very high notes — you’ll probably hear certain notes diverge wildly from the rest. Then bring Tone back down: the artifact eases off, but the tone loses some of its brightness too.

### 30.9.3 LFO Section

Operator’s LFO Display and Shell Parameters.

It’s fair to treat Operator’s LFO as a fifth oscillator of sorts. Running at audio rates, it modulates the frequency of the remaining oscillators. The Dest. A buttons in the LFO’s display let you arm or disarm that modulation per oscillator (and for the filter too), while the Dest. A slider sets how hard the LFO hits those destinations. Should you not need it, the LFO can be shut off outright.

A second destination opens up through the Dest. B chooser, letting the LFO drive one more parameter, with the Dest. B slider controlling how strong that modulation is.

For waveforms, the LFO presents the usual LFO shapes plus sample and hold (S&H) and noise. Sample and hold grabs random values at the LFO’s rate, stepping randomly in a way that suits classic retro-futuristic sci-fi sounds. The noise waveform amounts to nothing more than band-pass filtered noise.

Tip: FM synthesis is great for cooking up percussion, and pairing the LFO with its noise waveform is the secret behind convincing hi-hats and snares.

The LFO’s frequency comes from the LFO Rate control in the shell together with the low/high/sync position of the neighboring LFO Range chooser. That frequency can lock to note pitch, stay fixed, or land anywhere between, as dictated by the Rate < Key parameter in the LFO’s display. Enable the R (Retrigger) button and the LFO returns to the same phase point with every note; disable R and it free-runs.

Overall LFO strength is governed by the LFO Amount control in the shell, which scales the Dest. A and B amounts alike and can itself bend to note velocity through the display’s Amt < Vel control. On top of that, the LFO’s own envelope shapes its intensity.

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

### 30.9.6 Global Controls

Operator’s Global Display and Shell Parameters.

Housed in the global section are the parameters that steer Operator’s overall behavior. On top of that, the global display area lays out a full complement of modulation routing controls.
