# Collision Mallet Noise And Architecture

Open when you need guidance on Collision Mallet Noise And Architecture in Ableton Live.

Context: [Collision](analog-and-collision-routes.md#302-collision).

<a id="source-3021-architecture-and-interface"></a>
### 30.2.1 Architecture and Interface

Two oscillators named _Mallet_ and _Noise_ generate Collision's sound, and they drive a pair of separate (or linked) stereo _resonators_. The oscillators supply the opening portion of the sound, yet it is the resonator settings that shape the sound's character the most.

Bear in mind that should both the Mallet and Noise sections be switched off, Collision yields no sound at all.

Collision's interface splits into sections and tabs. Controls for the matching Mallet and Noise oscillators live in the Mallet and Noise sections. Parameters for each individual resonator sit in the Resonator 1 and Resonator 2 tabs.

Two separate low-frequency oscillators (LFOs) reside in the LFO tab, and each one is able to modulate several parameters. In a similar way, the MIDI/MPE tab routes MIDI pitch bend, modulation wheel and aftertouch messages — plus their MPE (MIDI Polyphonic Expression) counterparts — to a number of destinations.

Sitting to the right of the MIDI/MPE tab, a block of global parameters covers voice polyphony, note retrigger, resonator structure, and total output volume.

Note: Switching off sections and tabs you aren't using can free up CPU resources.

<a id="source-3022-mallet-section"></a>
### 30.2.2 Mallet Section

Collision’s Mallet Section.

The Mallet section models a mallet striking a surface. Its parameters tune the physical traits of the mallet itself.

Use the Mallet button to flip the section on or off.

Volume governs the mallet's total output level. Pitch and velocity can modulate the Volume parameter when you set the Key and Vel sliders found in the MIDI tab.

Stiffness sets how hard the mallet is. Kept low, the mallet stays soft, giving fewer high frequencies and a longer, less defined hit. Raise the stiffness and the impact grows shorter while high frequencies build. Pitch and velocity may also modulate this parameter through the Key and Vel sliders in the MIDI tab.

Noise determines how much impact noise rides along with every mallet hit. It comes in handy for recreating the "chiff" of a felt-covered mallet head. The Noise parameter responds to pitch and velocity modulation via the Key and Vel sliders in the MIDI tab.

Color sets the noise component's frequency. The higher you go, the fewer low frequencies remain in the noise. Setting Noise to 0 renders this parameter inert.

<a id="source-3023-noise-section"></a>
### 30.2.3 Noise Section

Collision’s Noise Section.

As with the Mallet, the Noise section creates the opening impulse of Collision's sound. White noise comes out of the Noise oscillator and then runs into a multimode filter that has its own envelope generator. You may employ this section in place of the Mallet section, or alongside it.

Use the Noise button to flip the section on or off.

<a id="source-live-instrument-reference-part-2"></a>

Beside the Noise button sits a drop-down listing the noise filter types on offer. The available picks are LP, HP, BP, and LP+HP. To shape cutoff and resonance, turn the Freq knob and move the Res slider.

When BP is active, the Res slider works on resonance; under LP+HP it instead governs bandwidth. Filter frequency responds to modulation too — from note pitch, from velocity, or from the envelope generator — routed through the Key and Vel sliders on the MIDI tab or through the Env Amt knob.

Output level for the entire Noise section comes from Volume, which pitch and velocity can drive through the Key and Vel sliders found on the MIDI tab.

A conventional ADSR envelope generator — covering attack, decay, sustain, and release stages — is governed by the Env Amt knob.

How rapidly Noise climbs to its peak loudness is dialed in with the A (Attack) slider; the span needed for the envelope to settle at the sustain level once the attack stage finishes is dialed in with the D (Decay) slider.

Where the envelope holds from the close of decay until the key lifts is determined by the S (Sustain) slider. A setting of 0 removes any sustain stage entirely. A setting of 100 removes the decay stage instead.

The R (Release) slider, lastly, governs release time — the span the envelope needs to fall back to zero once you let go of the key.

Center or cut-off frequency for the filter is established by the Freq knob. Across the LP, HP, and BP filters the Res slider controls resonance at that frequency, and for the LP+HP filter it instead sets its width.
