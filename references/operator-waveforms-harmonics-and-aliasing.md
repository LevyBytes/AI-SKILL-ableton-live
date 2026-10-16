# Operator Waveforms Harmonics And Aliasing

Open when you need guidance on Operator Waveforms Harmonics And Aliasing in Ableton Live.

Context: [Oscillator Section](meld-and-operator-routes.md#3092-oscillator-section).

<a id="source-30921-built-in-waveforms"></a>
#### 30.9.2.1 Built-in Waveforms

Each oscillator ships with a stock set of fundamental waveform types — sine, sawtooth, square, triangle and noise — picked from the Wave chooser inside the individual oscillator displays. Leading the list is a pure, mathematical sine wave, the go-to starting point for a great many FM timbres. We threw in “Sine 4 Bit“ and “Sine 8 Bit“ as well, delivering the retro flavor that C64 fans cherish, alongside the “Saw D“ and “Square D“ digital waveforms that excel at digital bass sounds. The square, triangle and sawtooth options are resynthesized stand-ins for their ideal counterparts. Whatever number rides along in the displayed name (say, “Square 6“) tells you how many harmonics drive that resynthesis. Smaller counts come across as mellower and are far less prone to aliasing up in the high register. Two noise waveforms round things out: “Noise Looped,“ which is a looped chunk of noise, and “Noise White,“ which you should reach for when you want genuinely random noise.

<a id="source-30922-user-waveforms"></a>
#### 30.9.2.2 User Waveforms

Picking the “User“ entry in the Wave chooser lets you build waveforms from scratch by drawing the amplitudes of the oscillator’s harmonics. Equally, you can grab one of the stock waveforms and reshape it the very same way. A compact display beside the Wave chooser tracks your waveform live as you work.

Hover the mouse across the Oscillator display area and the cursor becomes a pencil. Drawing there pushes the harmonic amplitudes up or down. While you’re shaping them, the Status Bar reports both which harmonic you’re editing and its current amplitude. Hold Shift as you drag to lock the motion horizontally, which lets you tweak a single harmonic’s amplitude on its own.

Switches off to the right of the display let you toggle between editing the first 16, 32 or 64 harmonics. To reach beyond those, the drawn partials can be echoed upward with a tapering fade governed by the Repeat chooser. A low Repeat figure yields a brighter tone, whereas a higher one rolls off more top end and leaves the fundamental more pronounced. Switch Repeat off and any partials past the 16th, 32nd or 64th harmonic are simply cut.

Right-clicking the harmonics display brings up a context menu for restricting edits to just the even or just the odd harmonics; “All“ is the default. That same menu carries a Normalize toggle. Switch it on and the oscillator holds a steady overall output level as you keep adding harmonics; switch it off and each new harmonic piles on more level. Watch out — with Normalize off the volume can climb to extremes.

A context-menu option lets you save your waveform in .ams format into the Samples/Waveforms folder within your User Library. To bring Ams files back into Operator, drag them out of the browser and onto one of the oscillator’s display areas. Those Ams files load into Simpler or Sampler just as readily.

Right-click via the Osc Preview’s context menu to copy and paste either stock or user waveforms from one oscillator to another.

<a id="source-30923-more-oscillator-parameters"></a>
#### 30.9.2.3 More Oscillator Parameters

Dial an oscillator’s frequency from the shell using its Coarse and Fine controls. Ordinarily an oscillator’s frequency tracks the notes you play, yet certain sounds call for pinning one or more oscillators to set frequencies instead. Engage the Fixed option on any individual oscillator to do exactly that. The payoff is a sound whose timbre shifts across the keyboard while its tuning holds steady — Fixed Mode is handy, say, for building live drum sounds. It can also reach down to frequencies as low as 0.1 Hz. Keep in mind that with Fixed Mode on, the oscillator’s frequency is steered from the shell through the Frequency (Freq) and Multiplier (Multi) controls.

Each oscillator also carries a dedicated Osc < Vel control in Operator, letting velocity reshape frequency. That comes in especially handy with sequenced parts, where you can fine-tune every note’s velocity. Riding alongside it is the Q (Quantize) button: switch it on and frequency steps only in whole numbers, exactly as though you were turning the Coarse control by hand. Leave quantize off and frequency glides without snapping, producing detuned or inharmonic results (which might be precisely the effect you’re after…).

An oscillator’s amplitude rests on two things: its Level setting in the shell and its envelope, which appears and can be edited whenever the Envelope display is showing. Those envelopes also respond to note velocity and note pitch through the Vel and Key parameters found in the Envelope section of each oscillator’s display.

Set each oscillator’s phase with the Phase control in its display. Enable the R (Retrigger) button and the waveform snaps back to the same phase position on every note; disable R and the oscillator simply free-runs.

As noted earlier, oscillators can modulate one another once you arrange them with the global display’s algorithms. Where one oscillator modulates a second, the outcome hinges on two factors: how loud the modulating oscillator is and the frequency ratio linking the pair. And any oscillator that nothing else is modulating can feed back on itself through the Feedback parameter in its display.

<a id="source-30924-aliasing"></a>
#### 30.9.2.4 Aliasing

Aliasing distortion turns up across every kind of digital synthesis, stemming from the limited sample rate and precision inherent to digital systems, and it shows itself mainly up high. FM synthesis is a particularly fertile breeding ground for it, since rich stacks of high harmonics come so easily. By the same token, busier oscillator waveforms like “Saw 32,“ prove more aliasing-prone than clean sine waves. The thing cuts both ways: a touch of aliasing can be just the seasoning a cool sound needs, yet too much renders the timbre unplayable, because pitch perception collapses once high notes fold back to arbitrary frequencies. Operator holds aliasing in check with a high-quality Antialias mode, switched on by default for fresh patches but available to disable in the global section. The global section’s Tone parameter offers another handle on aliasing; it can behave somewhat like a low-pass filter, though that varies with the sound and isn’t reliably predictable. To get acquainted with how aliasing sounds, crank Tone all the way up and strike a handful of very high notes — you’ll probably hear certain notes diverge wildly from the rest. Then bring Tone back down: the artifact eases off, but the tone loses some of its brightness too.
