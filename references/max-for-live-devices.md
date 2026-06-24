# Max For Live Devices (part 1)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

### 32. Max for Live Devices

Bundled with Live is an assortment of purpose-built Max for Live devices that ship ready to use. The set spans instruments, effects, and [MIDI Tools](https://www.ableton.com/en/live-manual/12/midi-tools/#midi-tools).

Owners of the Suite edition — or of the Standard edition paired with the Max for Live add-on — are able to launch these devices inside [Max](https://cycling74.com/products/max). That opens the door to tweaking and reshaping them within the Max editor, something the stock Live devices don't permit.

Want deeper guidance on reworking devices inside Max? Have a look at the [Editing Max for Live Devices](https://www.ableton.com/en/live-manual/12/max-for-live/#editing-max-for-live-devices) and [Building Max for Live MIDI Tools](https://www.ableton.com/en/live-manual/12/max-for-live/#building-max-for-live-midi-tools) sections.

For a grounding in how devices work in Live generally, consult the [Working with Instruments and Effects](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects) chapter.

Keep in mind that Live ships in several [feature sets](https://www.ableton.com/en/live/compare-editions/) that vary by edition, so a handful of the devices described here might be absent from yours.

### 32.1 Max for Live Instruments

### 32.1.1 DS Clang

The DS Clang Instrument.

Built from a pair of tones plus white noise and a filter, DS Clang turns out an assortment of cowbell, clave, and noise-based percussion timbres.

Independent level control for each cowbell tone is handled by the Tone A/B sliders.

By adjusting the Filter control — which governs the high-pass and band-pass filter cutoff — you reshape the sound's character. Push the value up and the signal gains more high-frequency content.

How much white noise gets folded into the signal is dialed in with the Noise slider.

Switch on the Clave toggle and the Repeat slider becomes available for layering additional hits onto the clave sound.

Retuning the instrument is done through the Pitch parameter. Length is governed by the Decay knob, and the instrument's overall output is trimmed with the Volume control.

For an audition of the instrument as it is currently dialed in, click anywhere across the top portion of the display.

### 32.1.2 DS Clap

The DS Clap Instrument.

DS Clap blends filtered noise with an impulse that travels through panned delay lines. With it you can conjure anything from a crisp electronic clap to a looser, more lifelike handclap.

Spacing between the two delay lines is governed by the Sloppy control, which lets you tune how tightly or loosely the panned claps line up. Filtered noise is layered onto the clap's impulse via Tail.

Stereo width comes from the Spread slider: a setting of 0% collapses to mono, whereas 100% spreads the image wide. Color is handled by the Tone slider — raising it pushes more high-frequency content into the signal.

Repitching the clap is done with the Tune parameter. Its duration follows the Decay knob, and the device's overall output is set by the Volume control.

Click anywhere in the display's top half to hear how the instrument sounds with its present settings.

### 32.1.3 DS Cymbal

The DS Cymbal Instrument.

By marrying sine and pulse waveforms to high-passed noise, DS Cymbal can reproduce timbres across a wide span — from a delicate ride to a weighty crash.

Within the display, the Tone slider governs the high-pass filter cutoff, which reshapes the cymbal's color. The higher you set it, the more high-frequency content enters the signal.

Tuning of the cymbal is handled by the Pitch parameter. The Decay knob fixes how long the cymbal rings, and its overall output is adjusted with the Volume control.

To audition the current sound, click somewhere in the upper portion of the display.

### 32.1.4 DS FM

The DS FM Instrument.

Modeled after a vintage Japanese FM synth, DS FM opens up a spread of sounds that range from gritty static bursts to metallic lasers.

The display's Tone slider drives the low-pass filter cutoff, so adjusting it recolors the drum. Crank it higher and the signal carries more high-frequency content.

How strongly feedback feeds the FM algorithm is governed by Feedb. Larger settings push the result toward noise.

The depth of FM modulation is set by Amnt, while the Mod slider crossfades among the available modulation types.

Global tuning lives on the Pitch parameter. The Decay knob fixes the drum's length, and overall output is trimmed using the Volume control.

Click anywhere over the top half of the display to preview the instrument at its current settings.

### 32.1.5 DS HH

The DS HH Instrument.

DS HH mixes noise with sine waveforms, giving you a broad palette that runs from crisp closed hats all the way to sizzling open ones.

Two noise flavors — white or pink — are available through the Noise toggle.

In the display, the Tone slider governs the high-pass filter cutoff, letting you recolor the hat. Raise the value and the signal gains more high-frequency content.

A resonant high-pass filter shapes the pitched part of the sound. You can flip this filter between 12 and 24 dB slopes, and its onset is timed with the Attack slider.

For global tuning, reach for the Pitch parameter. The hat's length is fixed by the Decay knob, and overall output is adjusted with the Volume control.

To hear the instrument as it stands, click anywhere across the upper part of the display.

### 32.1.6 DS Kick

The DS Kick Instrument.

At its heart, DS Kick is a kick-drum synthesizer driven by a modulated sine wave.

Tuning in Hz is performed with the Pitch slider. To give the kick more character, introduce grit through the Drive slider or stack harmonics with the OT slider.

Smoothing of the sine wave is handled by the Attack parameter. Flip the Click switch to graft a click onto the kick, sharpening its transient.

The kick's length is fixed by the Decay knob. Pitch modulation is dialed in with Env. Overall output is governed by the Volume control.

For a preview at the present settings, click anywhere in the display's upper half.

### 32.1.7 DS Snare

The DS Snare Instrument.

Combining a pitched oscillator with noise, DS Snare covers everything from a classic acoustic snare to the gated noise snare that turns up so often in electronic dance music.

Tone of the pitched signal is shaped by the Color parameter, whereas the noise signal's prominence is set with the Tone parameter.

The noise signal can be routed through any one of three filter types: low-pass, high-pass, or band-pass.

How long the snare lasts is set by the Decay knob, and global tuning comes from the Tune parameter. The instrument's overall output is handled by the Volume control.

Click anywhere across the top half of the display to audition the current sound.

### 32.1.8 DS Tom

The DS Tom Instrument.

DS Tom pairs an impulse with a choice of pitched oscillator waveforms, so you can build toms across a range of timbres — from deep and thunderous through sharp and tappy.

Tuning in Hz is set with the Pitch slider. Filter gain and cutoff are governed by the Color parameter, while the Tone slider drives the level of resonant band-pass filters that emulate how the drum membrane is tuned.

Shaping of the pitch envelope falls to the Bend parameter. The tom's length is fixed by the Decay knob, and overall output is trimmed with the Volume control.

To preview the instrument as currently set, click anywhere over the top portion of the display.

### 32.2 Max for Live Audio Effects

### 32.2.1 Align Delay

The Align Delay Effect

A utility device, Align Delay holds back the signals coming into it by a measure given in samples, milliseconds, or meters/feet.

The Delay Mode drop-down menu offers three modes to pick from: Time, Samples, and Distance.

In Time mode the delay is expressed in milliseconds, which is handy for lining audio up with A/V equipment or for adding gentle stereo widening.

Samples mode states the delay in samples and serves to offset the latency that other devices introduce.

Distance mode gives the delay in meters or feet and is useful for fixing timing offsets that arise from the physical spacing of components in a PA system.

Distance mode also carries a Temperature option, comprising a toggle to pick Celsius or Fahrenheit alongside a slider that sets the temperature. Aligning these with the room's actual temperature sharpens the timing, since sound propagates at different rates in warm versus cold air.

Switch on the Link L/R toggle to copy the left channel's delay settings onto the right. With it active, the Delay Right slider is grayed out, and moving the Delay Left slider drives both channels together.

### 32.2.2 Envelope Follower

The Envelope Follower Effect.

As a modulator device, Envelope Follower reads the amplitude of whatever signal arrives and traces it as a smooth, continuous curve. That curve then drives whatever parameters you've mapped. One classic use of envelope following is the auto-wah.

Within Live, any automatable parameter — device or mixer controls among them — can be mapped to Envelope Follower. To do that, switch on the Map button and click a parameter to set it as the mapping target.

The Show/Hide Multimap button in the display's top-right corner reveals further mapping buttons, bringing the total you can map to eight.

You Can Map up to Eight Parameters.

Clearing an assignment is done with the Unmap button, found just to the right of the Map button.

Two routes exist for Envelope Follower to drive its mapped parameters: Modulation and Remote Control. The default is Modulation, though flipping the Mod toggle moves you to Remote Control.

With Modulation active, you remain free to change parameter values by hand even once they're mapped. The Modulation Polarity toggle flips between Bipolar and Unipolar modes. Under Bipolar, modulation swings both ways around a centered base value; under Unipolar, it moves in a single direction starting from the base value. The Modulation Amount slider fixes the modulation depth, defining the range relative to that base value.

Switch to Remote Control and the mapped parameter values are dictated entirely by Envelope Follower, with no manual adjustment possible. Scaling of the modulation range is handled by the Min and Max sliders.

The Gain knob applies gain to whatever signal comes in. Smoothing of the envelope's onset is handled by the Rise parameter, and smoothing of its tail by the Fall control — together these fine-tune the envelope's contour.

Delay time for the envelope is fixed by the Delay control. The Delay Mode buttons let you toggle between time-based delay and tempo-synced beat divisions.

By default, Envelope Follower derives its envelope from the track's own input signal. Turn on sidechain routing and it will instead read an external signal pulled from another track. As an example, sidechaining from a Drum Rack lets you build rhythmic ducking or gating effects.

The Sidechain Section in Envelope Follower.

The triangle toggle in the device's top-left corner unfolds the Audio Routing panel, where the sidechain controls live.

To configure sidechain routing, switch on the Sidechain toggle and pick the audio source from the first drop-down in the Audio From section. The second drop-down decides whether the signal is taken Pre FX, Post FX, or Post Mixer. When Racks are involved, you may also target a specific input channel.

Track-input and external-sidechain levels are shown respectively on the Direct and S.C. meters.

The Sidechain Mix control balances the track input against the external sidechain signal. Set to 0%, the envelope is built from the track input alone; set to 100%, it relies entirely on the external sidechain signal.

### 32.2.3 LFO

The LFO Effect.

LFO is a modulator device that steers mapped parameters by way of low-frequency oscillation.

Within Live, any automatable parameter — device or mixer controls included — can be assigned to LFO. Do this by turning on the Map button and clicking the parameter you want to use as the mapping target.

Additional mapping buttons appear when you press the Show/Hide Multimap button at the display's top right; in all, up to eight parameters can be mapped.

You Can Map up to Eight Parameters.

To drop an assignment, click the Unmap button sitting to the right of the Map button.

LFO offers two ways to govern mapped parameters: Modulation and Remote Control. Modulation is the default, and the Mod toggle switches you over to Remote Control.

While Modulation is on, you can still tweak parameter values manually after mapping them. The Modulation Polarity toggle alternates between Bipolar and Unipolar modes. Bipolar mode modulates in both directions around a centered base value, whereas Unipolar mode pushes in just one direction away from the base value. Modulation depth is fixed by the Modulation Amount slider, which sets the range measured against the base value.

Once Remote Control is on, the mapped values are set entirely by LFO and can't be edited by hand. The Min and Max sliders scale the modulation range.

The Waveform drop-down menu lets you pick from nine shapes: Sine, Up, Down, Triangle, Square, Random, Bin, Stray, and Glider.

Bending or skewing the LFO waveform is done with the Shape control, and the Steps slider can divide the waveform into as many as 24 steps. Because of how their values arise, some waveforms can't be shaped or stepped — so the Shape control grays out for Random, Bin, Stray, or Glider, and the Steps control grays out for Random, Bin, or Square.

Randomness is sprinkled onto the LFO output by the Jitter slider, while the Smooth control rounds off abrupt changes in the output, including the ones jitter introduces.

The LFO rate is fixed by the Rate control. The Time Mode toggles flip between frequencies in Hertz and tempo-synced beat divisions, and when Hz is active the ×10 button multiplies the frequency value.

For every mapped parameter, the modulation amount is governed by Depth. At 0% nothing is modulated, and at 100% the LFO output reaches its full strength.

The Offset control repositions the center point of the LFO output. At 0% the output sits centered. Positive values raise the output, negative values lower it. A horizontal line in the display marks the center, serving as a handy visual cue while you adjust Offset.

You Can Shift the Center Point of the LFO Output Using Offset.

Where the LFO sits within its cycle is set by the Phase slider, running from 0% (cycle start) to 100% (cycle end).

To lock the LFO output at its present value, turn on the Hold toggle. Turning Hold off resumes the LFO from the value that was held.

Press the R (Retrigger) button to restart the LFO from the spot set by the Phase control.

### 32.2.4 Shaper

The Shaper Effect.

Shaper is a modulator device that builds mappable modulation data out of a breakpoint envelope.

Within Live, any automatable parameter — device or mixer controls among them — may be routed to Shaper. To set this up, switch on the Map button and click the parameter you wish to use as the mapping target.

Pressing the Show/Hide Multimap button at the display's top right surfaces extra mapping buttons, raising the total to eight parameters.

You Can Map up to Eight Parameters.

To clear an assignment, click the Unmap button positioned to the right of the Map button.

Shaper drives mapped parameters in one of two ways: Modulation and Remote Control. The default is Modulation, and the Mod toggle takes you to Remote Control.

With Modulation engaged, parameter values stay editable by hand even once mapped. The Modulation Polarity toggle alternates between Bipolar and Unipolar modes. Bipolar modulation runs in both directions about a centered base value, while Unipolar modulation extends one way from the base value. Modulation depth is set with the Modulation Amount slider, establishing the range relative to the base value.

When Remote Control is engaged, the mapped values come solely from Shaper and admit no manual edits. Use the Min and Max sliders to scale the modulation range.

Click anywhere in the display to drop a breakpoint. Holding the Alt (Win) / Option (Mac) key as you drag between breakpoints yields curved segments, and holding Shift while clicking a breakpoint removes it.

To wipe the whole envelope from the display, hit the Clear button in the lower-left corner. Just to its right, six presets let you spin up a fresh breakpoint envelope in a hurry.

The number of grid divisions in the display is set with the Grid slider. Turn on Snap and any breakpoint you add or move will lock to the nearest grid line.

A smaller display at the device's top right offers an oscilloscope-style look at the envelope's output signal.

Randomness is added to the envelope output by the Jitter slider, while abrupt output changes — jitter-induced ones included — are smoothed out by the Smooth control.

Where the envelope output falls within its cycle is set by the Phase control, spanning 0% (cycle start) to 100% (cycle end). The R (Retrigger) button restarts the envelope output from the spot Phase defines; note that this Retrigger button grays out whenever Time Mode is set to Sync.

The Offset control repositions the center of the envelope output. At 0% the output is centered, positive values lift it, and negative values drop it. A horizontal line in the oscilloscope display marks the center, a useful visual reference as you adjust Offset.

You Can Shift the Center Point of the Envelope Output Using Offset.

Three trigger modes are available in Shaper: Loop, 1-Shot, and Manual. Switching among them is done with the matching toggles.

- Loop — The envelope cycles without pause at whatever rate the Rate control specifies.
- 1-Shot — A single pass of the envelope is fired off using the mappable T button.
- Manual — You scrub the envelope back and forth by hand with the Manual control.

The envelope rate is set by the Rate control. The Time Mode toggles switch between frequencies in Hertz and tempo-synced beat divisions.

Across all mapped parameters, the modulation amount is set by Depth. At 0% none is applied, and at 100% the envelope output hits its full level.

### 32.3 Max for Live MIDI Effects

### 32.3.1 Envelope MIDI

The Envelope MIDI Effect.

Envelope MIDI is a modulator device that drives mapped parameters through an ADSR envelope.

Within Live, any automatable parameter — device or mixer controls included — can be tied to Envelope MIDI. To do so, switch on the Map button and click the parameter you want as the mapping target.

The Show/Hide Multimap button at the display's top right exposes more mapping buttons, allowing as many as eight parameters to be mapped.

You Can Map up to Eight Parameters.

To remove an assignment, click the Unmap button located to the right of the Map button.

Envelope MIDI steers mapped parameters by one of two methods: Modulation and Remote Control. Modulation is chosen by default, and the Mod toggle moves you to Remote Control.

While Modulation is active, you can keep adjusting parameter values by hand after mapping. The Modulation Polarity toggle alternates between Bipolar and Unipolar modes. Bipolar mode modulates both ways around a centered base value; Unipolar mode works in a single direction out from the base value. Set the modulation depth with the Modulation Amount slider, which determines the range relative to the base value.

Once Remote Control is active, the mapped values are fixed entirely by Envelope MIDI and resist manual change. Scale the modulation range using the Min and Max sliders.

The Loop Mode drop-down offers four choices: Free, Sync, Loop, and Echo.

- Free — Every note that plays fires the envelope once.
- Sync — The envelope retriggers on the beat division chosen in the Sync Rate drop-down.
- Loop — The envelope repeats at the rate the Global Time control specifies.
- Echo — The envelope spawns echoes spaced by the Env Echo Time control. How much of each echo carries into the following one is set by the Env Feedback control, which in turn governs how long the echoes linger; raising feedback yields longer-lasting repeats.

Each time the envelope fires, the LED beside the Loop Mode drop-down flashes.

The envelope's duration is scaled by Global Time. Its default of 1.00 keeps the envelope at the timing the ADSR values dictate. Settings above 1.00 stretch the envelope proportionally, and settings below 1.00 squeeze it.

For all mapped parameters, the modulation amount is governed by the Amount control. At 0% nothing is modulated; at 100% the envelope output reaches its peak strength.

Attack fixes how long the envelope takes to climb to its peak once a note sounds. Decay sets how long it takes to fall from that peak down to the Sustain level.

The level the envelope holds after the Decay stage while a note stays down is defined by the Sustain control. The Release control determines how long the envelope takes to fall back to zero after the note lifts.

For the matching stages, curved envelope segments can be drawn using the Slope sliders sitting beneath Attack, Decay, and Release.

You can likewise set the Attack, Decay, Sustain, and Release values — plus the ADR slopes — by grabbing and dragging the envelope handles in the display.

Turn on the Velocity toggle and the envelope's peak scales in proportion to each incoming note's velocity. Softer notes yield a lower peak and gentler modulation, whereas harder ones produce a higher peak and stronger modulation.

The Sustain toggle turns the sustain behavior on or off. When on, the envelope holds at the Sustain level for the duration the note is held and only advances to the Release stage once the note lifts. When off, the envelope acts as a one-shot — it runs through the Attack and Decay stages and then moves into Release no matter how long the note is held.

### 32.3.2 Expression Control

The Expression Control Effect.

Expression Control is a modulator device that governs mapped parameters from a choice of MIDI and MPE sources.

It provides five Mod Source tabs, and each one can be pointed at a particular MIDI or MPE source. From the MIDI Input Source drop-down menu you pick whichever expression parameter you need; the ten on offer are Velocity, Modwheel, Pitchbend, Pressure, Keytrack, Expression, Random, Increment, Slide, and Sustain.

Within Live, any automatable parameter — device or mixer controls among them — can be assigned to the chosen modulation source. To do this, switch on the Map button and click a parameter to set it as the mapping target.

Which controls appear in the Output Range section is dictated by the Modulation toggle at the device's top right. That toggle decides how Expression Control produces its modulation values and offers two modes: Modulate or Remote Control.

Pick Modulate and you can still nudge a mapped parameter's base value with the cursor. In this mode, whatever Expression Control sets or automates blends with the value you dial in as you adjust that parameter. Pick Remote Control instead and Expression Control alone determines the modulated values, leaving the base parameter values beyond reach.
