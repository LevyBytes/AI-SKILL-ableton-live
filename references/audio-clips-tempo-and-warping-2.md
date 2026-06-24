# Audio Clips Tempo And Warping (part 2)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Use the _Preserve_ control to hold onto divisions within the sample — the markers that separate one chunk of audio from the next. For percussion that you intend to warp, the _Transients_ option gives the truest outcome, since it reads where the audio’s transients fall and warps according to those positions. Should you instead want fixed beat divisions kept no matter where transients happen to sit, pick any of the grid-division settings. Pairing wide grid divisions with pitch transposition can yield some pleasingly odd rhythmic textures.

Use the _Transient Loop Mode_ selector to define how the audio’s transients behave when looped:

_Loop Off_ — Every slice of audio bounded by transients runs through once and then halts. Whatever gap is left over until the following transient stays silent.

_Loop Forward_ — Every slice bounded by transients runs to completion, after which playback leaps back to a zero-crossing roughly at the slice’s midpoint and keeps cycling there until the following transient arrives.

_Loop Back-and-Forth_ — Every slice bounded by transients runs to completion, then playback rewinds as far as a zero-crossing near the slice’s center before advancing once more toward the slice’s end. That oscillation repeats up until the following transient. Paired with preserved transients, this setting frequently produces a clean, polished tone — particularly at reduced tempos.

The _Transient Envelope_ control governs how the level fades from one slice of audio to the next. A value of 100 applies no fade at all, whereas 0 stretches the fades out so each slice dies away almost immediately. Raising the envelope time tends to iron out clicks where slices meet, and dropping it lets you fashion rhythmic gating textures.

### 9.3.2 Tones Mode

Reach for Tones mode when you need to time-stretch material with a clearly defined pitch — think vocal lines, single-note instruments, and bass parts.

_Grain Size_ gives you a coarse handle on the typical length of the grains in play. How big the grains actually end up depends on how sharply the audio’s pitch shifts. When the material moves between well-defined pitches, smaller grains tend to serve you best. Bigger grains can stave off stray noise, though they sometimes introduce audible artifacts of their own.

### 9.3.3 Texture Mode

Texture mode suits material lacking an obvious tune or pitch center — polyphonic orchestral passages, ambient pads, noise beds, or sustained drones. It also shines for sound design and adventurous, experimental processing.

Here the _Grain Size_ control again sets the grain size in use, yet — in contrast to Tones mode — the tonal qualities of the audio play no part in how that size is calculated.

_Fluctuation_ feeds a degree of randomness into the way the sample gets handled; the larger the value, the wider the random variation.

### 9.3.4 Re-Pitch Mode

Turn to Re-Pitch mode when you want to alter the sample’s playback rate. Doing so shifts the sample’s pitch as its tempo changes — the same effect a DJ gets nudging a turntable, or that vintage samplers produce when audio is sped up or slowed down. Double the rate, for instance, and the pitch climbs a full octave.

Because speed and pitch are bound together here, the sample’s transposition controls are switched off while this mode is active.

### 9.3.5 Complex and Complex Pro Mode

Complex mode comes in handy for warping audio that blends rhythm, melody, and texture together — full tracks being a prime example.

Complex Pro mode runs a refined take on the engine behind Complex mode and can deliver cleaner-sounding output. As with its sibling, Complex Pro is at its best on polyphonic material or complete tracks.

The _Formants_ control dictates what happens to the sample’s formants — the tone’s resonant frequencies — once you transpose the pitch. Set to 100%, it holds the original formants in place even under heavy pitch shifts, which keeps the source timbre intact. Bear in mind the control does nothing at all unless the sample’s transposition has actually been altered.

The _Envelope_ control likewise shapes the broad tonal character. Its default of 128 suits the majority of samples. With bright, high-register sources you may get nicer results by dialing the Envelope down, whereas darker, low-register sources often benefit from pushing it up.

On many systems, the Complex and Complex Pro modes draw more processing power than the remaining Warp Modes. When you need to free up CPU headroom, [freeze](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#track-freeze) or [resample](https://www.ableton.com/en/live-manual/12/routing-and-i-o/#resampling) any tracks running these modes.
