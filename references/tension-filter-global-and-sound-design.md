# Tension Filter Global And Sound Design

Open when you need guidance on Tension Filter Global And Sound Design in Ableton Live.

Context: [Tension](simpler-and-tension-routes.md#3012-tension).

<a id="source-30123-filterglobal-tab"></a>
### 30.12.3 Filter/Global Tab

Tension’s Filter/Global Tab.

On Tension’s Filter/Global tab you’ll find a polyphonic filter complete with envelope, LFO, and MIDI modulation, alongside keyboard and portamento settings plus a built-in Unison audio effect.

Tension’s Filter Section.

The Filter section provides a deeply adjustable multi-mode filter positioned between the String and Body sections. On top of that, it can be driven by its own envelope generator and a low-frequency oscillator (LFO).

Keep in mind that a switch in the Filter subsection enables or disables the whole Filter section, whereas the Filter Envelope and Filter LFO sections come with separate toggles of their own.

Picking the filter type happens at the filter’s chooser. The available choices are low-pass, band-pass, notch, high-pass and formant filters, each offered in 2nd and 4th order.

Use the Freq slider to set the filter’s resonance frequency and the Res control to set how much resonance there is. With a formant filter active, the Res control steps through a series of vowel sounds. Both the Freq and Res controls accept modulation from LFO, envelope or note pitch by way of the sliders underneath. Bear in mind the LFO and Env sliders do nothing until the Envelope and LFO subsections have been switched on.

A switch beside its name turns the Filter Envelope subsection on or off. It follows the familiar ADSR (attack, decay, sustain, release) layout but adds a couple of wrinkles:

- The Attack knob defines the attack time, but the Vel slider sitting under it lets MIDI note velocity modulate that time too. Raising the Vel value makes harder-played notes attack progressively faster.
- After the attack stage, the Decay knob determines how quickly the envelope falls to the sustain level.
- Using the Sustain knob you set the level the envelope holds once decay finishes, lasting until the key lifts. All the way left removes the sustain stage entirely; all the way right removes the decay stage. Note velocity can also shape the sustain level through the Vel slider beneath the knob — larger settings raise the sustain level as velocity climbs.
- The Release knob defines release time, meaning how long the envelope takes to fall back to zero once the key is let go.

An extra modulation source for the filter comes from the Filter LFO subsection, which you enable or disable with the switch beside its name.

The waveform driving the LFO is chosen at the LFO waveform chooser, offering sine, triangle, rectangular and a pair of random waveforms. One random option jumps between random levels, while the other transitions with gentler ramps.

You set how fast the LFO runs with the Rate knob, and the switches under it flip the Rate between a frequency in Hertz and tempo-synced beat divisions.

Finally, the Attack knob governs how long the oscillator needs to climb to full amplitude, and the Delay knob governs how much time passes before the LFO kicks in after a note starts.

Tension’s MPE Section.

Within the MPE section you can route MPE pressure and slide data to destinations and define Tension’s global and per-note pitch bend ranges. Each of the three MPE sources carries an Activity LED that illuminates whenever Tension picks up an incoming MPE signal.

Both the Pressure and Slide sources let you pick two destinations to send their MPE data to, with the Amount sliders setting how much modulation is applied.

Through the Pitch Bend controls you set the modulation range for the global pitch bend together with the MPE per-note pitch bend (Note PB), expressed in semitones.

Tension’s Keyboard Section.

Everything to do with Tension’s polyphony, tuning, and MIDI parameters lives in the Keyboard section.

Coarse and fine tuning duties fall to the Octave, Semi and Detune controls. Octave shifts the whole instrument in octave steps, Semi moves it up or down by semitones, and the Detune slider nudges things one cent at a time (out to a ceiling of 50 cents in either direction).

How many voices are available is set by the Voices chooser.

Stretch reproduces a method called stretch tuning, a tuning tweak frequently applied to both electric and acoustic pianos. Leave it at 0% and Tension performs in equal temperament — meaning two notes form an octave when the higher note’s fundamental is precisely double that of the lower one. Because a real vibrating tine or string doesn’t resonate exactly as the theory predicts, equal temperament can sound “wrong“ on pianos. Dialing Stretch upward sharpens the upper notes while flattening the lower ones, producing a brighter character. Going negative mimics “negative“ stretch tuning, in which the upper notes flatten and the lower notes sharpen.

Pushing the Error slider up introduces more random tuning error on every note. Crank it high if you’re feeling nostalgic for your junior high school orchestra days.

Finally, Priority decides which notes get dropped once you exceed the maximum polyphony. With Priority set to High, incoming notes pitched above the notes already sounding take precedence, and the cull begins from the lowest pitch. The Low setting reverses this. Choosing Last favors whatever was played most recently, dropping the oldest notes when room is needed.

Tension’s Portamento Section.

Rather than letting pitch jump straight from one note to the next, the Portamento section makes it glide between them. Flip the switch beside its name to engage or disengage the effect.

The slide’s overall pace is governed by the Time slider.

Turn on Legato and the glide happens only when you strike the second note before letting go of the first.

Enabling Prop. (Proportional) ties the glide duration to the size of the interval between notes, so wider intervals glide more slowly than narrow ones. Switch it off and the glide time stays fixed no matter the interval.

Tension’s Unison Section.

With the Unison section you can layer several voices onto each note you play. The Unison toggle switches the whole section on or off.

Use the Voices switch to pick either two or four layered voices, and Detune to set how much tuning spread is applied across those layers. Modest amounts yield a gentle chorus, whereas large amounts offer yet another route to that youth-orchestra feel.

Raising the Delay amount introduces a lag before each layered voice comes in.

Tension’s Volume Knob.

Sitting in the corner, the Volume knob controls the instrument’s total output level. You can also get to this same control from the String tab.

<a id="source-30124-sound-design-tips"></a>
### 30.12.4 Sound Design Tips

On the surface, Tension’s modular layout might look fairly familiar compared with other synths — a set of functional blocks passing a signal down a path and reshaping it along the way. The crucial thing to keep in mind, though, is that these blocks aren’t walled off from each other; adjusting a single parameter can ripple out and strongly affect another one elsewhere. As a result, certain parameter combinations will yield silence, and others will generate punishingly loud output — so take care when you set your levels!

It often helps, while working with Tension, to picture the sections as genuine parts of one physical object. Imagine a bow drawn slowly across a string with no damping — it may set that string in motion. Clamp the same string with a massive damper, however, and the bow has to move much faster to produce any result.

A good way to appreciate the range on offer is to dig into how the factory presets were built. It won’t take long to discover that Tension reaches well beyond plain string sounds.
