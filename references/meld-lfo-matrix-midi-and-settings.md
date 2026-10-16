# Meld LFO Matrix MIDI And Settings

Open when you need guidance on Meld LFO Matrix MIDI And Settings in Ableton Live.

Context: [Meld](impulse-and-meld-routes.md#308-meld).

<a id="source-3085-lfos-tab"></a>
### 30.8.5 LFOs Tab

Engine A’s LFOs.

Two LFOs of its own come with each of Meld’s engines. You can dial in the rates of LFO 1 and LFO 2 in Hertz or lock them to tempo, and a Phase Offset slider nudges each LFO’s phase. With Retrigger switched on, the LFO begins again from the point fixed by the Phase Offset slider.

You choose LFO 1’s waveform from the LFO 1 Type drop-down menu, which offers six waveform types: Basic Shapes, Ramp, Wander, Alternate, Euclid, and Pulsate. You can sculpt these waveforms further with the LFO’s Rate knob and the two macro knobs beside it, whose behavior depends on the chosen waveform type.

There’s also the LFO 1 FX panel for modulating LFO 1. Each of the FX1 and FX2 drop-down menus holds eighteen effect types you can chain onto LFO 1 in series. You set how strongly an effect is applied through its matching macro knob. Be aware that LFO 1 and LFO1 FX can each serve as a standalone modulation source within Meld’s Modulation Matrix.

LFO 2 hands you six classic waveform types to pick from: Sine, Tri, Saw Up, Saw Down, Rectangle, Random S&H. Within Meld’s Modulation Matrix, LFO 2 can act as a third standalone modulation source.

<a id="source-3086-matrix-tab"></a>
### 30.8.6 Matrix Tab

Engine B’s Modulation Matrix.

Within the device, Meld’s Modulation Matrix is where you route modulation sources to modulation targets. You might, for instance, set Engine A’s LFO 1 to modulate its Volume, or have Engine B’s Modulation Envelope modulate its Filter Frequency.

The modulation sources run along the horizontal axis while the modulation targets run down the vertical one. To apply modulation between two parameters, click a cell and drag it up or down. Going negative speeds up envelopes and LFOs, while going positive slows them down. Keep in mind that certain parameters receive additive modulation, whereas others receive multiplicative modulation.

Clicking a parameter drops it into the Modulation Matrix. A parameter lands in the Modulation Matrix belonging to whichever engine is currently chosen via the Display Selector Tab. Any parameter that isn’t being modulated drops out of the Modulation Matrix the moment you click a different one.

<a id="source-3087-midi-and-mpe-tabs"></a>
### 30.8.7 MIDI and MPE Tabs

Engine A’s MIDI Tab.

Through Meld’s MIDI and MPE tabs you can press MIDI and MPE features into service as modulation sources, turning Meld into a responsive performance tool.

With Velocity chosen as a modulation source, Meld takes the velocity value of an incoming MIDI note and uses it to modulate its modulation target across the length of that note.

With Pitch chosen as a modulation source, Meld takes the pitch value of an incoming MIDI note and uses it to modulate its modulation target across the length of that note.

With Random chosen as a modulation source, Meld modulates its modulation target using a random value, freshly computed every time a note fires.

Many MIDI controller devices carry the Pitch Bend, Press, and Modulation Wheel hardware controls. Many MPE controller devices carry the Note Pitch Bend, Slide, and Press hardware controls. Lacking a MIDI or MPE controller, you can still drive these parameters through [clip envelopes](https://www.ableton.com/en/live-manual/12/clip-envelopes/#midi-controller-clip-envelopes).

<a id="source-3088-settings-tab"></a>
### 30.8.8 Settings Tab

Meld’s Engine Settings.

Three global settings live in Meld’s Settings tab, each adjustable on a per-engine basis: Osc Key Tracking, Scale Awareness, and Glide.

Oscillator key tracking is turned on or off by the Osc Key Tracking switch. With it on, an oscillator sounds the pitch of whichever incoming MIDI note it gets. With it off, an oscillator holds a fixed C3 pitch for every incoming MIDI note, or the scale’s root within the C3 octave should Scale Mode be on. This proves handy for, say, playing drones or percussive sounds.

Turning on the Phase Reset switch snaps the oscillator’s phase back to a fixed value at every new note. Enabling Phase Reset also unlocks the Phase Spread switch. With Phase Spread on, the oscillator’s starting phase gets spread according to the Spread modulation source in the Modulation Matrix. With Phase Spread off, the starting phase is pinned to zero.

The Scale Awareness section holds two switches you can turn on: Oscillator Scale Awareness and Filter Scale Awareness.

Turn on Oscillator Scale Awareness and the pitches driven by scale-aware oscillator types stay in scale as well. The (♭♯) tag flags the scale-aware oscillator types, namely Dual Basic Shapes along with all four swarm variants — Swarm Sine, Swarm Triangle, Swarm Saw, Swarm Square — plus Chip.

Switch on Filter Scale Awareness and the resonant frequencies of scale-aware filter types stay in scale too. These filter types, tagged with a (♭♯), are scale aware: Plate Resonator and Membrane Resonator.

Within the Glide section sit two glide modes — Portamento (Porta) and Glissando (Gliss) — together with a Glide Time control.

How long overlapping notes take to glide into the next incoming pitch is fixed by the Glide Time control. Glide works in both Mono and Poly modes.

With Portamento on, playing a note while another is still held causes the first note’s pitch to glide steadily into the pitch of the second. With Glissando on, playing a note while another is still held makes the first note’s pitch climb or fall into the second note’s pitch through discrete steps. If scale awareness is on, Glissando lays out those steps as scale degrees. Bear in mind that portamento and glissando are only heard once Glide Time sits at a value greater than zero.
