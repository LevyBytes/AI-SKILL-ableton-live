# Meld Mixing And Global Controls

Open when you need guidance on Meld Mixing And Global Controls in Ableton Live.

Context: [Meld](impulse-and-meld-routes.md#308-meld).

<a id="source-30810-mix-section"></a>
### 30.8.10 Mix Section

Mix Controls for Each Engine.

Within Meld’s Mix section, every engine carries its own Volume and Pan controls plus a dedicated Tone Filter. Volume governs how loud that engine plays overall, while Pan places it left or right within the stereo image.

Think of Meld’s Tone Filter control as a high-pass and low-pass pair rolled together. Push it into positive territory and an engine’s lows are cut back; pull it negative and the engine’s highs are trimmed instead.

Pressing the Limit button engages Meld’s onboard limiter. Once on, it acts per voice — running only after the two engines are combined and the global Drive amount has taken effect. Use it to rein in Meld’s total output whenever both engines are sounding together.

<a id="source-30811-global-controls"></a>
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
