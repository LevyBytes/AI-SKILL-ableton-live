# Live Instrument Reference (part 7)

> Ableton Live reference. Original prose; identifiers preserved verbatim.

Whatever depth of multisampling suits you, Sampler accommodates it: feel free to load and audition multisample presets, [import multisamples](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#importing-third-party-multisamples) from third-party vendors, or build your own from the ground up. And multisamples aren't even required — just drop a single sample into Sampler and exploit its built-in modulation engine in whatever way you prefer.

### 30.10.3 Title Bar Options

Sampler’s Title Bar Context Menu.

Before we dive into the rich modulation capabilities Sampler offers, it's worth surveying the entries available in its title bar context menu.

While Cut, Copy, Rename, Edit Info Text, and Delete are likely things you already recognize, a few of the remaining choices warrant a closer look:

_Group_ — Choosing this option places Sampler inside a fresh Instrument Rack.

_Fold_ — Collapses Sampler down to just its device title bar. A quick double-click on that title bar brings it back open again.

_Show Preset Name_ — Normally, Sampler adopts the name of the uppermost sample in the sample layer list for its title. Turn off Show Preset Name and the title becomes “Sampler.” instead.

_Lock to Control Surface_ — Ties Sampler to a control surface that Live natively supports, as configured in the Link, Tempo & MIDI Settings, so you keep direct control regardless of what currently has focus in your Live Set. Whenever a track is armed for recording, Sampler locks to the control surface on its own by default. To signal this state, a hand icon appears in the title bar of any locked device.

_Save as Default Preset_ — Stores Sampler’s present configuration to serve as the default preset.

_Use Constant Power Fade for Loops_ — Out of the box, Sampler applies constant-power fades where loops meet. Disable this option and looping points instead receive linear crossfades.

_Sampler -> Simpler_ — Translates Sampler presets into [Simpler](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#simpler) presets. That makes it simple to pass Sets along to collaborators whose Live edition lacks Sampler.

### 30.10.4 Sampler’s Tabs

Sampler’s Tabs in the Title Bar.

Reachable from Sampler‘s title bar, Sampler’s capabilities are grouped by category across a set of tabs: Zone, Sample, Pitch/Osc, Filter/Global, Modulation and MIDI. Selecting a tab exposes the relevant properties underneath it — the lone exception being the Zone tab. Beyond just keeping things tidy, each tab carries one or more LEDs that light up to show whether modulation data exists in that section. Our tour of Sampler proceeds tab by tab.

### 30.10.5 The Zone Tab

The Zone Tab.

Selecting the Zone tab switches Sampler‘s Zone Editor on or off. That editor gives you a direct, visual way to assign any quantity of samples across three kinds of ranges, handled by the Key Zone, the Velocity Zone and Sample Select Editors in turn.

The Key Zone Editor.

Rather than sharing space, the Zone Editor appears in its own view positioned immediately above the Device View. Paired with Sampler’s remaining tabs, this arrangement makes building and tweaking multisamples considerably faster.

Running down the left edge of the Zone Editor sits the sample layer list, which keeps multisamples organized. Each separate sample that makes up a multisample appears in this list, and here such samples carry the name _layers_. With intricate multisamples, the list may grow rather lengthy.

Sitting just above the sample layer list is a row of buttons used to set up the sample layers and switch among the various editors:

_Auto Select (Auto)_ — When MIDI notes reach Sampler, each one passes through the key, velocity and sample select zones belonging to every sample layer. Turn on Auto Select and every sample layer capable of sounding an arriving note gets highlighted in the sample layer list for as long as that note lasts.

_Zone Fade Mode (Lin/Pow)_ — Pressing this button switches the fade slope of all zones back and forth between linear and constant-power (exponential).

_Round Robin (RR)_ — Use this button to switch [Round Robin sample playback](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#round-robin-sample-playback) either on or off.

_Zone Editor View (Key/Vel/Sel)_ — These buttons control whether the Key Zone, Velocity Zone and Sample Select Editors are shown.

Filling the remainder of the view is whichever of three sample-layer editors is active: the [Key Zone Editor](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#key-zones), the [Velocity Zone Editor](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#velocity-zones) and the [Sample Select Editor](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sample-select-zones). To adjust their horizontal zoom, right-click inside one to open a context menu and pick Small, Medium or Large.

#### 30.10.5.1 Round Robin Sample Playback

Using Different Samples for Round Robin Playback.

With Round Robin, a fresh sample sounds on each successive note you play. The result is that, over time, you step through a group of samples following a set sequence.

One use, for instance, is to step Round Robin through samples of the same note or sound captured with varied articulations, lending gentle variety to otherwise repetitive drum or note figures. Alternatively, feeding it samples that sound wildly different produces surprising rhythmic or tonal twists across a pattern.

Turning Round Robin on is done by flipping the RR toggle within the Zone Editor.

Enable the RR Toggle to Activate Round Robin Playback.

After it's active, whichever samples in the [sample layer list](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#the-sample-layer-list) occupy the same [key zone](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#key-zones) become eligible to fire whenever a note lands in that range.

The Round Robin Mode chooser lets you pick how those samples get triggered:

_Forward_ — Steps through samples in sequence, beginning at the top of the sample layer list and moving downward. After the final sample sounds, the sequence loops back around to the uppermost sample.

_Backward_ — Steps through samples in sequence, beginning at the bottom of the sample layer list and working upward. After the topmost sample plays, the sequence starts over.

_Other_ — Draws samples in random order, but guarantees the same sample is never fired two times back-to-back.

_Random_ — Draws samples in random order, and here the same sample may indeed repeat several times in succession.

The Round Robin Mode Chooser.

Through the Reset Interval chooser you can dictate a fixed point at which the sequence starts over. That helps fire samples in a steady, predictable way. As an example, with the Round Robin Mode set to Forward and a reset interval of 1 bar, the uppermost sample sounds on each bar's opening note. With Backward, the sequence resets to the bottommost sample. With Other or Random, it resets to whichever sample played first.

The Reset Interval Chooser.

#### 30.10.5.2 The Sample Layer List

The Sample Layer List.

Every sample held within the multisample you currently have loaded shows up here, each occupying its own layer. With extremely large multisamples, the list could stretch to hundreds of layers! Happily, you can give layers meaningful names (based on their root key, say). Hover over a layer here, or over a zone in the zone editors, and the Status Bar (bottom of screen) presents details about that sample. Pick any layer and its sample loads into the Sample tab so you can inspect it.

A right-click anywhere in the sample layer list brings up a context menu with choices for ordering and presenting the layers, spreading them across the keyboard, and assorted other sample-management and “housekeeping“ tasks.

_Delete_ — Removes whichever sample(s) you currently have selected.

_Duplicate_ — Makes a copy of whichever sample(s) you currently have selected.

_Rename_ — Gives the chosen sample a new name.

_Distribute Ranges Equally_ — Spreads samples uniformly across the editor’s full MIDI note range (C-2 to G8).

_Distribute Ranges Around Root Key_ — When layers carry differing root keys, this choice spaces their ranges as evenly as it can around each root key while avoiding any overlap. When layers share one root key, their ranges come out evenly spaced.

_Small/Medium/Large_ — Changes how far the Zone Editor is zoomed.

_Show in Browser_ — Jumps to the chosen sample within the browser and highlights it.

_Manage Sample_ — Brings up the File Manager with the chosen sample selected.

_Normalize Volume_ — Tunes Sampler’s Volume control so that the loudest peak in each selected sample fills the full available headroom.

_Normalize Pan_ — Tunes Sampler’s Pan control so each selected sample carries matching volume on both sides of the stereo field. Keep in mind this won't always recenter panned stereo samples; instead, Live works out a pan setting that yields a balanced stereo spread.

_Select All With Same Range_ — Highlights every layer sharing the zone range of the layer you've currently selected. What you get back varies with whichever Zone Editor (Key, Velocity or Sample Select) happens to be active.

_Sort Alphabetically (Ascending and Descending)_ — Orders samples by name in alphabetical sequence.

_Sort by Key (Ascending and Descending)_ — Orders key zones either ascending or descending.

_Sort by Velocity (Ascending and Descending)_ — Orders velocity zones either ascending or descending.

_Sort by Selector (Ascending and Descending)_ — Orders sample select zones either ascending or descending.

#### 30.10.5.3 Key Zones

The Key Zone Editor.

A sample's key zone sets the span of MIDI notes across which that sample sounds. A sample fires only when an arriving MIDI note falls inside its key zone. Each sample owns a key zone of its own, and that zone may cover anything from one solitary key right up to all 127.

The usual multisampled instrument is built from numerous separate samples spread among numerous key zones. A sample is recorded at one specific key within an instrument’s voice range (that key being its _root key_), yet it can still ring true when shifted a handful of semitones either way. That playable span typically becomes the sample’s key zone, while pitches outside it are covered by further samples wherever required.

Newly imported samples start out with key zones spanning the entire MIDI note range. Much like clips in the Arrangement View, you can reposition and resize zones — drag a left or right edge to resize, then slide the zone where you want it.

Either end of a zone can also be faded across several semitones by dragging its upper-left or upper-right corner. That lets neighboring samples crossfade cleanly into one another as you move along the keyboard. Above the sample layer list, the Lin and Pow boxes show whether a zone fades in linear or exponential fashion.

#### 30.10.5.4 Velocity Zones

The Velocity Zone Editor.

A velocity zone fixes which span of MIDI Note On velocities (1-127) a given sample reacts to. Since how hard you play dramatically alters the tone of most instruments, the finest multisamples record not just the individual notes but also each note captured at several velocities.

Switch on the Velocity Zone Editor and it shows up beside the sample layer list. Velocity runs along a scale of 1-127, and that range of numbers is printed across the editor's top edge. Apart from that, the Velocity Zone Editor behaves exactly like the Key Zone Editor.

#### 30.10.5.5 Sample Select Zones

The Sample Select Editor.

On top of that, every sample carries a Sample Select zone — a filter for data that has no connection to any specific form of MIDI input. These Sample Select zones closely resemble the [Chain Select Zones](https://www.ableton.com/en/live-manual/12/instrument-drum-and-effect-racks/#chain-select-zones) used in Racks: only those samples whose sample select values cross the present setting of the _sample selector_ end up triggered.

Toggle on the Sample Select Editor and it sits next to the sample layer list. Like the Velocity Zone Editor, this editor uses a scale of 0-127. Riding above that value scale is a draggable marker called the sample selector.

The Sample Selector.

Where you place the sample selector merely governs which samples become eligible to trigger. After a sample has already fired, moving the sample selector won't swap in a different sample mid-playback.

### 30.10.6 The Sample Tab

The Sample Tab.

You configure how individual samples play back from inside the Sample tab. The bulk of this tab is given over to showing the waveform of whichever sample is currently selected. Hover the pointer above the waveform and the Status Bar (bottom of screen) reports details about the sample. Bear in mind that nearly all of this tab's values pertain solely to the sample you currently have selected. The Sample chooser perpetually shows the active sample layer’s name and doubles as a means of moving between layers while you edit.

Holding the Ctrl (Win) / Cmd (Mac) modifier while scrolling with the mousewheel or trackpad zooms into the current sample.

_Reverse_ — A global, modulatable control that plays the whole multisample in reverse. In contrast to the Clip View's Reverse function, no fresh sample file gets written. Rather, playback departs from the Sample End point, runs backward through the Sustain Loop (when it's active), and finishes at the Sample Start point.

_Snap_ — Pulls every start and end point onto the waveform zero-crossings (spots where amplitude equals zero) so as to prevent clicks. Trying Snap on square wave samples makes the effect easy to observe. Just like Simpler, this snapping references the left channel of a stereo sample, so occasionally a modest Crossfade value is required to wipe out clicks entirely. To snap a single loop region, right-click its loop brace and choose “Snap Marker.”

_Sample_ — Shows the name of the active sample layer and serves to rapidly pick out other layers within the loaded multisample.

_Root Key (RootKey)_ — Sets the root key for the current sample.

_Detune_ — Lets you fine-tune the sample by +/- 50 cents.

_Volume_ — A broad-range volume control spanning from total attenuation up to a gain of +24 dB.

_Pan_ — Each sample can be placed anywhere you like within the stereo panorama.

#### 30.10.6.1 Sample Playback

Every parameter below operates together with the global volume envelope (located in the Filter/Global tab) to shape Sampler's fundamental voicing. Among other things, these envelopes rely on the familiar ADSR (Attack, Decay, Sustain, Release) parameters:

Envelope Attack Time (Attack) — Determines how long an envelope takes to climb from its initial level up to the peak level. You can reshape that climb with the Attack Slope (A. Slope) parameter.

Envelope Decay Time (Decay) — Determines how long an envelope takes to fall from the peak level down to the sustain level. You can reshape that fall with the Decay Slope (D. Slope) parameter.

Envelope Sustain Level (Sustain) — The level held once the envelope decay concludes. The envelope holds here right up until note release, unless it happens to be running in Loop, Sync or Beat Mode.

Envelope Release Time (Release) — How long an envelope takes to arrive at the end level once a Note Off message comes in. The Release Slope (R. Slope) value dictates the contour of this portion of the envelope.

Envelope Initial Level (Initial) — Determines where the envelope begins.

Envelope Peak Level (Peak) — The high point reached as the envelope attack finishes and the Decay stage gets underway.

Envelope End Level (End) — (LFO, Filter and pitch envelopes only) The level arrived at once the Release stage wraps up.

Envelope Rates < Velocity (Time < Vel) — This setting governs how much note velocity modulates the envelope segments. It becomes particularly engaging when the envelopes loop. Bear in mind it doesn't touch the beat-time under Beat or Sync Modes — only the envelope segments themselves.

Envelope Loop Mode (Loop) — Set to Loop and the envelope restarts once the decay segment finishes. Set to Beat or Sync and it restarts after a specified beat-time. Under Sync Mode that restart locks to song time. Under Trigger mode the envelope pays no attention to Note Off.

Envelope Beat/Sync Rate (Repeat) — So long as it remains on, the envelope re-fires after this span of beat-time. On each re-fire it climbs at the set attack rate from wherever it currently sits up to the peak level.

Envelope Loop Time (Time) — Should a note still be held after the decay/sustain segment ends, the envelope restarts from its initial value. This parameter sets how long the trip from sustain level back to the initial value takes.

As noted earlier, Sampler’s envelopes additionally offer parameters for tuning the slope of each envelope segment. A positive slope value makes the envelope race ahead at first and then ease off. A negative slope value keeps the envelope flat for a stretch before accelerating toward the finish. At a slope of zero the motion is linear, holding one constant rate across the whole segment.

This tab presents every time-based value in either samples or minutes:seconds:milliseconds, a choice you flip via the context menu on any of the parameter boxes. Here, "samples" denotes the tiniest measurable increment of digital audio rather than the audio files themselves, which are what we usually call “samples.“

_Sample Start_ — The time position at which playback kicks off. Should the volume envelope’s Attack parameter be cranked high (a slow attack), what you actually hear might commence somewhat after the point indicated here.

_Sample End_ — The time position at which playback stops (assuming no loop is enabled), regardless of whether the volume envelope has finished.

_Sustain Mode_ — The optional Sustain Loop marks out a portion of the sample that repeats for as long as the note sits in the sustain stage of its envelope. Switching on the Sustain Loop additionally makes the Release Loop available. That opens up a handful of playback choices:

_No Sustain Loop_ — Playback runs straight through until it hits the Sample End or until the volume envelope finishes its release stage, whichever comes first.

_Sustain Loop Enabled_ — Playback runs straight through to Loop End, then leaps at once to Loop Start and keeps looping. With Release Mode OFF, that looping persists within the Sustain Loop right up until the volume envelope finishes its release stage.

_Back-and-Forth Sustain Loop Enabled_ — Playback advances to Loop End, then runs backward to Loop Start, then heads forward toward Loop End once more. With Release Mode OFF, the cycle keeps repeating until the volume envelope finishes its release stage.

_Link_ — Flipping the Link switch makes Sample Start match Loop Start. Note that the Sample Start parameter box keeps its original value — it merely grays out, ready to be restored with one click.

_Loop Start_ — Where the Sustain Loop begins, expressed in samples.

_Loop End_ — Where the Sustain Loop ends, expressed in samples.

_Release Mode_ — Release Mode becomes available to enable any time the Sustain Loop is active.

— The volume envelope’s release stage runs, but stays confined to the Sustain Loop, and playback never moves past Loop End.

_Release Enabled_ — Once the volume envelope hits its release stage, playback runs straight ahead toward Sample End.

_Release Loop Enabled_ — Once the volume envelope hits its release stage, playback runs straight ahead to Sample End, then leaps at once to Release Loop and keeps looping until the volume envelope finishes its release stage.

_Back-and-Forth Release Loop Enabled_ — Once the volume envelope hits its release stage, playback runs straight ahead to Sample End, then reverses back to Release Loop, then heads forward toward Sample End again. The cycle repeats until the volume envelope finishes its release stage.

_Release Loop_ — fixes where the Release Loop begins. Sample End marks where the Release Loop ends.

_Sustain- and Release-Loop Crossfade (Crossfade)_ — Crossfading the loops helps strip clicks out of loop transitions. By default Sampler applies constant-power fades at loop boundaries, but switching off “Use Constant Power Fade for Loops“ in the context menu enables linear crossfades instead.

_Sustain- and Release-Loop Detune (Detune)_ — Because a loop is really just an oscillation, a sample's pitch can drift inside the loop in proportion to the loop’s length. Tip: very short loops make this most apparent. Detune lets you bring the pitch of those regions back in line with the rest of the sample.

_Interpolation (Interpol)_ — A global setting that controls how precisely transposed samples are rendered. Be warned that pushing the quality past “Normal“ to “Good” or “Best” taxes your CPU heavily.

_RAM Mode (RAM)_ — Another global control, this one pulls the full multisample into RAM. Doing so can improve performance while you modulate start and end points, yet loading sizable multisamples into RAM rapidly eats up the RAM your computer needs elsewhere. Either way, fitting your computer with as much RAM as you can is always advisable, since it can deliver meaningful performance benefits.

Right-clicking on the waveform to open its context menu offers several editing and viewing choices. Just as in the Sample Layer List context menu, Show in Browser, Manage Samples, Normalize Volumes and Normalize Pan all appear. You can also zoom in toward or out from the playing or looping regions, depending on the Sustain and Loop Modes currently in effect.

To close out, a few more controls sit at the far-right edge of the Sample tab:

_Vertical Zoom (slider)_ — Stretches the waveform's height within the sample display. This affects appearance only and leaves the audio untouched.

_B, M, L and R Buttons_ — Standing for Both, Mono, Left and Right, these buttons let you decide which channels of the sample get shown.

### 30.10.7 The Pitch/Osc Tab

The Pitch/Osc Tab.

#### 30.10.7.1 The Modulation Oscillator (Osc)

Each voice in Sampler comes with its own modulation oscillator capable of applying frequency or amplitude modulation (_FM_ or _AM_) to the multisample. This oscillator is fully equipped: 21 waveforms (picked from the Type chooser) plus a loopable amplitude envelope all its own for dynamic waveshaping. Keep in mind it does nothing but modulate — you never hear its output on its own. What reaches your ears is how that output acts upon the multisample.

_FM_ — Under this mode, the modulation oscillator alters the frequency of samples, yielding richer waveforms that sound noticeably different.

_AM_ — Under this mode, the modulation oscillator alters the amplitude of samples. Modulator frequencies below hearing range produce gentle or fast swings in volume level, whereas modulator frequencies within hearing range generate composite waveforms.

You steer the modulation oscillator through its Initial, Peak, Sustain, End, Loop, Attack and Time < Velocities parameters. The [Sample Playback](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#sample-playback) section covers in depth how these operate. On top of that, the right-hand portion of the modulation oscillator section holds these controls:

_Type_ — Pick the waveform for the modulation oscillator here.

_Volume_ — Governs how strongly the modulation oscillator modulates the sample.

_Vol < Vel_ — Incoming MIDI note velocity can drive the modulation oscillator’s Volume parameter. That sets the modulation's depth.
