# Live Instrument Reference (part 8)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

_Fixed_ — Switch this on and the modulation oscillator holds a constant frequency, set by the Freq and Multi parameters; played MIDI notes no longer shift that rate.

_Freq_ — When Fixed is On, the Multi parameter scales this value to arrive at the modulation oscillator’s constant frequency.

_Multi_ — When Fixed is On, this factor multiplies the Freq parameter to arrive at the modulation oscillator’s constant frequency.

_Coarse_ — Broad tuning for the modulation oscillator’s frequency (0.125-48). It is accessible only while Fixed is Off.

_Fine_ — Detailed tuning for the modulation oscillator’s frequency (0-1000). It is accessible only while Fixed is Off.

#### 30.10.7.2 The Pitch Envelope

As time passes, the pitch envelope shapes the pitch of the sample and also that of the Modulation Oscillator whenever it is turned on. It is a multi-stage envelope offering ADSR plus Initial, Peak, and End levels, just as the [Sample Playback](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sample-playback) section explains. You can set each envelope parameter with its slider or by moving the breakpoints inside the envelope’s display.

The Amount slider sits at the lower-left corner of the Pitch Envelope section. It sets how far, in semitones, the pitch envelope can reach. Exactly how wide that span turns out depends on how the envelope itself behaves.

Along the right edge of this section sit five sliders plus a single chooser; none of them belong to the Pitch Envelope, yet each can shape Sampler’s overall output:

_Spread_ — Turning on Spread spawns a pair of detuned voices for every note. The trade-off is that CPU usage is doubled as well.

_Transpose (Transp)_ — Overall transpose value, given in semitones.

_Detune_ — Overall detune value, given in cents.

_Key Zone Shift (Zn Shft)_ — This shifts MIDI notes within the Key Zone Editor alone, letting alternate samples be picked for playback while still tracking the pitch you play. Handy for coaxing unusual textures out of multisamples.

_Glide_ — The overall Glide mode, paired with the Time parameter so pitches slide smoothly into one another. ’Glide’ behaves as a conventional monophonic slide, whereas ’Portamento’ operates across polyphony.

_Time_ — Switching on a Glide mode causes the pitch of successive notes to slide rather than jump. The duration of that slide is governed by this parameter.

### 30.10.8 The Filter/Global Tab

The Filter/Global Tab.

#### 30.10.8.1 The Filter

Sampler includes a polyphonic filter that can optionally route through a built-in waveshaper. Within the filter section you can pick from several filter shapes: low-pass, high-pass, band-pass, notch, and the distinctive Morph filter. Every filter toggles between 12 and 24 dB slopes, and you can also choose among various analog-modeled circuit characters, created together with Cytomic, that reproduce the hardware filters of certain vintage analog synthesizers.

Clean is a refined, light-on-CPU circuit identical to the filtering in [EQ Eight](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#eq-eight). Every filter type can use it.

OSR is a state-variable circuit whose resonance is reined in by a distinctive hard-clipping diode. Modeled after the filters in a fairly uncommon British monosynth, it works with all filter types.

MS2 employs a Sallen-Key topology together with soft clipping to keep resonance in check. Patterned after the filters in a well-known semi-modular Japanese monosynth, it is offered for the low-pass and high-pass filters.

SMP is a bespoke circuit that follows no specific piece of hardware. Blending traits drawn from the MS2 and PRD circuits, it is offered for the low-pass and high-pass filters.

PRD relies on a ladder topology and applies no dedicated resonance limiting. Modeled on the filters of a classic dual-oscillator monosynth from the United States, it is offered for the low-pass and high-pass filters.

Frequency and Resonance are the two controls that matter most and are familiar from any synth. Frequency picks the spot in the harmonic spectrum where the filter acts, and Resonance lifts the frequencies surrounding that spot.

Whenever the low-pass, high-pass, or band-pass filter runs through any circuit other than Clean, a supplementary Drive control appears, letting you push gain or distortion into the signal ahead of the filter.

A dedicated Morph control accompanies the Morph filter, smoothly cycling the response from low-pass through band-pass and high-pass to notch before returning to low-pass.

Through dedicated entries in the Morph slider’s context menu, the Morph control can be snapped at once onto whichever position you need — low-pass, band-pass, high-pass, or notch.

Over on the right, a dedicated filter envelope can modulate the filter’s cutoff frequency across time. It behaves much like the Pitch/Osc tab envelopes, providing Initial, Peak, Sustain and End levels along with ADSR, Loop mode and slope points. The F. Env button switches this section on and off. The Amount slider governs how strongly the filter envelope acts on the cutoff frequency and must hold a non-zero value before the envelope produces any result.

A waveshaper sits beneath the Filter and is engaged with the Shaper button. The Type selector offers four shaping curves: Soft, Hard, Sine and 4bit. You dial in Shaper’s strength with the Amount slider. The button positioned above the waveshaper area also lets you flip the order of processing: point the triangle upward and the signal travels from the shaper into the filter; point it downward and it travels from the filter into the shaper.

#### 30.10.8.2 The Volume Envelope and Global Controls

Operating globally, the volume envelope shapes the articulation of Sampler’s tones through the usual ADSR (attack, decay, sustain, release) parameters. Refer to the [Sample Playback](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sample-playback) section for an explanation of those parameters.

You can loop this envelope as well, using the Loop chooser. Once a Loop mode is active, the Time/Repeat slider takes on significance. Under Loop and Trigger modes, a note held past the close of the Decay stage sends the envelope back to its starting value. How quickly it travels from the Sustain level down to that starting value is governed by the Time parameter. Under Beat and Sync modes, a note held longer than the span set on the Repeat slider sends the envelope back to its starting value.

Acting across every sample, the Pan slider is a global pan control, and Pan < Rnd injects some randomness into that global pan placement. Time (Global Time Envelope) stretches or compresses, in proportion, the duration of all of Sampler’s envelopes. Time < Key (Global Envelope Time < Key) stretches or compresses that duration in proportion to the pitch of arriving MIDI notes.

Lastly, the Voices selector grants as many as 32 concurrent voices to every Sampler instance. You can switch on voice retriggering with the Retrigger button (R) located beside the Voices chooser. With it on, a note that is already sounding gets retriggered instead of spawning an extra voice. Enabling Retrigger can conserve CPU, particularly when a note carrying a long release tail is retriggered repeatedly in rapid succession.

### 30.10.9 The Modulation Tab

The Modulation Tab.

Within the Modulation tab you get one more loopable envelope alongside three LFOs, every one of them able to modulate several parameters and even one another. An LFO may run freely or lock to the Live Set’s tempo, and stereo modulation effects are possible with LFOs 2 and 3.

#### 30.10.9.1 The Auxiliary Envelope

Over on the left, the Auxiliary (Aux) envelope behaves a great deal like the Pitch/Osc tab envelopes, supplying Initial, Peak, Sustain and End levels together with ADSR, Loop mode and slope points. You can send this envelope to any of 29 destinations via both the A and B choosers. The depth with which the Auxiliary envelope modulates destinations A and B is dialed in with the pair of sliders to the right.

#### 30.10.9.2 LFOs 1, 2 and 3

Whatever room is left on the Modulation tab holds three Low Frequency Oscillators (LFOs). True to their name, Sampler’s LFOs work by feeding a low frequency (under 30 Hz) into a parameter so as to modulate it. Activate any oscillator by clicking the LFO 1, LFO 2 or LFO 3 switches.

_Type_ — Six waveshapes are on offer for Sampler’s LFOs: Sine, Square, Triangle, Sawtooth Down, Sawtooth Up, and Sample and Hold.

_Rate_ — When Hz is chosen, the Freq slider on the right governs the LFO’s speed. When the note head is chosen instead, the LFO locks to beat-time, which you adjust on the Beats slider to the right.

_Freq_ — The LFO’s speed expressed in Hertz (cycles per second), tunable from 0.01 to 30 Hz.

_Beats_ — Specifies the LFO’s speed in beat-time (64th notes to 8 bars).

_LFO Attack (Attack)_ — The interval the LFO requires to climb to full intensity. It lets you, say, ease vibrato in gradually while a note sustains.

_LFO Retrigger (Retrig)_ — Switching on Retrigger for an LFO resets it to its origin, the initial phase, with every fresh MIDI note. Retriggering the LFO before it finishes a cycle can yield hybrid LFO contours.

_LFO Offset (Offset)_ — This shifts an LFO’s origin, or initial phase, so the oscillator launches from somewhere else in its cycle. Retriggering the LFO before it finishes a cycle can yield hybrid LFO contours.

_LFO Rate < Key (Key)_ — Commonly called keyboard tracking, any non-zero setting makes an LFO speed up in line with the pitch of incoming MIDI notes.

LFO 1 carries four sliders for swiftly modulating global parameters:

_Volume (Vol)_ — LFO 1 is able to modulate the global volume level. This slider sets the modulation depth across a 0-100 scale.

_Pan (Pan)_ — LFO 1 is able to modulate the global pan placement. This slider sets the modulation depth across a 0-100 scale.

_Filter_ — LFO 1 is able to modulate the filter cutoff frequency (Freq in the Filter/Global tab). This slider sets the modulation depth across a 0-24 scale.

_Pitch_ — LFO 1 is able to modulate the pitch of samples. This slider sets the modulation depth across a 0-100 scale.

_LFO Stereo Mode (Stereo)_ — Two flavors of stereo modulation are available from LFOs 2 and 3: _Phase_ or _Spin_. Under phase mode, the left and right LFO channels move at the same speed, and the Phase parameter shifts the right channel away from the left. Under spin mode, the Spin parameter lets the right LFO channel run as much as 50% quicker than the left.

As with the Auxiliary envelope, LFOs 2 and 3 provide A and B choosers through which you can direct the LFOs toward numerous destinations.

### 30.10.10 The MIDI Tab

The MIDI Tab.

By way of its parameters, the MIDI tab makes Sampler an expressive, responsive performance instrument. Up to a pair of destinations apiece can be assigned to these incoming MIDI sources: _Key, Velocity, Release Velocity, Aftertouch, Modulation Wheel, Foot Controller_ together with _Pitch Bend_, while the Amount A and Amount B sliders govern how strongly each one acts.

Say you route Velocity’s Destination A to Loop Length and push its Amount A to 100: strong velocities then yield lengthy loops, and gentle velocities yield shorter ones.

A Pitch Bend Range slider (0 to 24 steps) lives at the bottom. Sampler can map the 14-bit span of pitch wheel values onto as much as 24 semitones of pitch bend.

Lastly, a click on the Sampler graphic at the right launches a scrolling, film-style credit roll for Sampler. Those are the folks who deserve your thanks!

### 30.10.11 Importing Third-Party Multisamples

The third-party [sample formats](https://help.ableton.com/hc/en-us/articles/115001134410) that Sampler can read are:

- REX files (supported in Live Standard and Suite only)
- ACID Loops
- Soundtrack Loops

Be aware that Live cannot read the tags embedded in ACID Loops or Soundtrack Loops.

To bring in a third-party multisample, locate the file in Live‘s browser and drop it onto a Live Set. Doing so imports it into your User Library.

The import process generates fresh Sampler presets, which appear in the browser at User Library/Sampler/Imports.

Be aware that certain multisample files are turned into [Instrument Rack](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#instrument-drum-and-effect-racks) presets holding multiple Sampler instances, so the original is reproduced with greater accuracy.

### 30.11 Simpler

The Simpler Instrument.

Simpler is an instrument that merges a sampler’s core building blocks with a handful of familiar synthesizer parameters. Each Simpler voice plays a region of a sample that you define, and that region then runs through envelope, filter, LFO, volume and pitch stages. What sets it apart from an ordinary sampler is a set of special abilities carried over from Live’s clips. In particular, Simpler can reproduce samples through Live’s warping. A warped sample sounds at your Set’s tempo no matter which note you strike. Warping inside Simpler operates almost identically to warping in audio clips, and when you drag such a warped clip into it — whether sourced from an audio track, the browser, or your desktop — the manual warp settings you made are kept. The [Audio Clips, Tempo, and Warping](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#audio-clips-tempo-and-warping) chapter has further details on warping.

Two areas make up Simpler’s interface: the Sample and Controls tabs. For an enlarged view, click the button in Simpler’s title bar to move the Sample controls between the device chain and Live’s main window. In that expanded layout, the Controls tab parameters spread Simpler out across the Device View.

The sample waveform is shown on the Sample Tab. You can drag samples into Simpler straight from the browser, or as clips out of the Session or Arrangement View. When you do the latter, Simpler uses solely the portion of the sample bounded by the clip’s start/end or loop markers. Whatever edits were applied to a clip’s Warp Markers and its other warp properties carry over as you drag the clip into Simpler. To swap a sample, drag a replacement in, or switch on the Hot-Swap button at the waveform display’s lower-right corner.

Hot-Swapping a Sample.

Zoom into the sample waveform by scrolling on the mousewheel or trackpad as you hold the Ctrl (Win) / Cmd (Mac) modifier.

### 30.11.1 Playback Modes

How Simpler handles samples hinges above all on the mode switch, the control you use to pick one of Simpler’s three playback modes. You will find this switch on the Sample tab’s left edge or running along the lower part of the expanded sample view.

Mode Switch in the Sample Tab.Mode Switch in the Expanded View.

- _Classic Playback Mode_ is what Simpler starts in by default and is geared toward building “conventional” melodic and harmonic instruments from pitched samples. It provides a full ADSR envelope and permits looping, so a sample can sustain for as long as you keep a note down. By default Classic Mode is polyphonic.
- _One-Shot Playback Mode_ handles monophonic playback only and suits one-shot drum hits or brief sampled phrases. It pares down the envelope controls and offers no looping. Out of the box, triggering a note plays the whole sample, no matter how briefly the note is held.
- _Slicing Playback Mode_ cuts the sample into slices without altering it, letting each slice be triggered chromatically. You may add and reposition slices by hand, or pick from several options for how Simpler generates slices on its own. The mode excels at rhythmic drum breaks.

#### 30.11.1.1 Classic Playback Mode

The Sample Tab in Classic Playback Mode.

Under Classic Playback Mode, the assorted sample position controls govern which part of the sample is played. Among them are the Start and Length parameters together with the two “flags” shown on the waveform display. The left flag fixes the absolute spot in the sample where playback may begin, and the End control fixes where playback may stop. Start and Length are then expressed as percentages of the full sample length that the flags allow. A Length value of 50%, for instance, sounds precisely half of the region lying between the flags. The Loop slider sets what portion of the available sample loops. It only does anything when the Loop switch is on.

You can build sustaining loops short enough to acquire a glitchy or granular quality, or even to ring out as a pitch from looping at audio rates. That may be precisely the effect you are after, yet it can drive CPU very high, especially under the Complex or Complex Pro Warp Modes.

Frequently you will begin with a wide region of a sample and wind up keeping just a sliver of it. You can zoom and pan Simpler’s waveform display the same way you do elsewhere in Live — to zoom, drag up and down or scroll on the mousewheel or trackpad while holding the Ctrl (Win) / Cmd (Mac) modifier, and to pan, drag sideways to bring other parts of the sample into view. The zooming behaves identically across all three playback modes.

Clicking the Loop On/Off button decides whether the sample loops while a note is held. Clicks or pops can arise at a looped sample’s start and end points because of the jump in waveform amplitude (that is, the sample’s loudness). The Snap switch helps reduce these by pinning Simpler’s loop and region markers to _zero-crossing_ spots within the sample (spots where the amplitude reads zero). Snapping uses the left channel of a stereo sample as its reference. As a result, glitches with stereo samples remain possible even when Snap is on.

You can smooth the jump from loop end back to loop start using the Fade control, which crossfades the two points together. The technique pays off particularly with lengthy, textural samples.

With the Gain slider you can raise or lower the sample’s level. Keep in mind that it is a gain stage apart from Simpler’s Volume knob, which fixes the instrument’s final output level (once the signal has passed through Simpler’s filter). The parameter is present in all three playback modes.

How many voices Simpler can sound at once is capped by the Voices parameter. Should more voices be required than the Voices chooser permits, “voice stealing“ kicks in, dropping the oldest voice(s) so the newest ones can sound. If, say, your Voices parameter sits at 8 while ten voices all compete to play, the two oldest get dropped. (Simpler does its best to keep voice stealing unobtrusive.)

When Retrig is on, replaying a note that is still sustaining cuts off the prior instance. With Retrig off, several copies of the same note may layer over one another. Bear in mind that Retrig produces an audible difference only when the sample has a long release time and Voices is set above one.

Across all three playback modes the assorted [warp parameters](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#warp-controls) behave identically and are covered below.

#### 30.11.1.2 One-Shot Playback Mode

The Sample Tab in One-Shot Playback Mode.

Under One-Shot Playback Mode, the left and right flags delimit the available playback region exactly as in Classic Mode, but Loop and Length controls are absent. A Voices control is missing too, since One-Shot Mode is purely monophonic.

When Trigger is on, the sample keeps sounding after you let go of the note; how long you hold the pad makes no difference while Trigger is on.

The Fade In and Fade Out controls let you contour the sample’s loudness. Fade In sets how long the sample takes to reach full volume once a note is struck, and Fade Out starts fading the specified span before the sample region finishes.

When Gate is on, the sample starts to fade the moment you release the note. The Fade Out time fixes how long it takes to reach silence following release.

Snap operates much as it does in Classic Mode, except here it influences only the start and end flags (since there are no loop options.)

#### 30.11.1.3 Slicing Playback Mode

The Sample Tab in Slicing Playback Mode.

Under Slicing Playback Mode (just like One-Shot Playback Mode), the left and right flags delimit the available playback region.

Which method governs slice creation is set by the Slice By chooser:

- _Transient_ - Slices land automatically on the sample’s transients. The Sensitivity slider controls how responsive Simpler is to transient levels in the sample, and therefore how many slices it makes on its own. Larger values yield more slices, capped at 64 slices.
- _Beat_ - Slices land at musical beat divisions. The Division chooser picks the beat division Simpler uses to slice the sample region.
- _Region_ - Slices land at uniform time divisions. The Regions chooser picks how many equally spaced slices get created.
- _Manual_ - Slices are made by hand through double-clicking inside the sample region. With Manual chosen, no slices appear automatically.

How many slices can sound at the same time is set by the Playback chooser. Mono is monophonic, allowing one slice to play at any moment. With Poly chosen, several slices can fire together. The Voices and Retrig controls become available under Poly and operate just as in Classic Playback Mode. With Thru chosen, playback stays monophonic, yet triggering a single slice carries playback onward through the remainder of the sample region.

The Trigger/Gate switch operates identically to its behavior in One-Shot Playback Mode. The Fade In and Out controls act a bit differently according to the Playback chooser’s setting. Under Mono or Poly, the Fade times span from the start to the finish of each separate slice, whereas under Thru they span from the triggered slice to the region’s end. Consequently the fade times can sound unlike one another depending on where within the region you trigger.

Slices generated automatically show up as vertical blue lines across the waveform display. A double-click on a slice removes it. Should Simpler’s automatic slice positions not please you, you can drag a slice to relocate it. Double-clicking on the waveform in the gap between slices adds manual slices, which display in white. While in Transients mode, holding Alt (Win) / Option (Mac) and clicking a slice flips it between a manual and an automatic slice. Manual slices made in Transients mode survive no matter what the Sensitivity amount is.

### 30.11.2 Warp Controls

Simpler’s Warp Controls.

With the Warp switch off, Simpler acts like a “conventional” sampler: play the sample at various pitches and it sounds at various speeds. Now and then that is precisely the result you want. Yet for samples that carry their own built-in rhythm, you may prefer to turn on Warp. That makes Simpler reproduce the sample locked to the current song tempo, whatever notes you play.

Anyone acquainted with warping in audio clips will recognize that Simpler’s Warp Modes and settings work the very same way. The section titled [Warp Modes](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warp-modes) offers more details.

The Warp as… button tunes the sample’s warping so that it sounds exactly across the stated count of bars or beats. Live estimates that figure from the sample’s length, and if the guess is off, the ÷2 or ×2 buttons let you halve or double the playback speed accordingly.

### 30.11.3 Filter

Simpler’s Filter Controls.
