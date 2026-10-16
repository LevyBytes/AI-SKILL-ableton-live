# Device Clip Scale And Mixer Concepts

Open when you need guidance on Device Clip Scale And Mixer Concepts in Ableton Live.

Context: [Live Concepts](live-concepts.md#3-live-concepts).

<a id="source-311-devices"></a>
### 3.11 Devices

Beyond clips, a track may also hold a [chain of devices](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#working-with-instruments-and-effects) that process signals. A double-click on a track's title bar opens the [_Device View_](https://www.ableton.com/en/live-manual/12/live-concepts/#clip-and-device-view), where that track's device chain is shown.

The Device View Displaying a MIDI Track's Device Chain.

The devices that take in and put out audio signals carry the name [_audio effects_](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#live-audio-effect-reference). Among device types, only audio effects belong on an audio track or a return track. MIDI tracks, though, accept two further device types: [_MIDI effects_](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#live-midi-effect-reference) and [_instruments_](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#live-instrument-reference).

The browser is where you'll find Live's built-in audio effects, MIDI effects, and instruments. Tracks gain devices when you drag them out of the browser into the Device View, or drop them onto a Session or Arrangement track. You can also pick instruments and effects in the browser and press Enter to load them onto a track.

Live's Built-in Devices Are Available from the Browser.

[Plug-in devices](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#using-plug-ins) are usable in Live as well. The browser's _Plug-Ins_ label is where VST and Audio Units (macOS only) plug-ins reside.

Plug-In Devices Are Available from the Browser's Plug-Ins Label.

<a id="source-312-clip-and-device-view"></a>
### 3.12 Clip and Device View

Setting and tuning clip properties — start or end points, looping, scale settings — is what the [Clip View](https://www.ableton.com/en/live-manual/12/clip-view/#clip-view) is for. From the Session View, it additionally opens up extended clip properties such as [follow actions](https://www.ableton.com/en/live-manual/12/launching-clips/#follow-actions).

The Clip View

With audio clips, the Clip View opens up [warping controls](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#warping) plus [audio transformation tools](https://www.ableton.com/en/live-manual/12/audio-clips-tempo-and-warping/#quantizing-audio).

With MIDI clips, the Clip View brings pitch and time utilities, together with MIDI [Transformation](https://www.ableton.com/en/live-manual/12/midi-tools/#transformation-tools) and [Generative tools](https://www.ableton.com/en/live-manual/12/midi-tools/#generative-tools).

A roster of the devices loaded on whichever track you've selected appears in the [Device View](https://www.ableton.com/en/live-manual/12/working-with-instruments-and-effects/#device-view). On MIDI tracks you can load MIDI effects, instruments, and audio effects. On audio, group, and return tracks you can load audio effects.

The Device View.

Stacking the Clip View and Device View lets you see both at once. To do so, click the triangle toggles beside the Clip View and Device View Selectors, sitting to the left of the Mixer View toggle down in Live's bottom-right corner. The keyboard shortcuts Ctrl+Alt+3 (Win) / Cmd+Option+3 (Mac) reveal the Clip View and Ctrl+Alt+4 (Win) / Cmd+Option+4 (Mac) reveal the Device View.

Stacked Clip and Device View.

<a id="source-313-scale-awareness"></a>
### 3.13 Scale Awareness

With Live's scale options you can pin any clip to a scale you prefer, and you can apply scales across Live's effects and devices too. The moment you switch on Scale Mode for a particular clip, effect, or device, it turns _scale aware_.

Scale awareness on clips can be switched on through the Scale Mode toggle on the Control Bar or straight from the Clip View. The Root Note and Scale Name choosers beside the Scale Mode toggle let you pick a root key and a scale type. Whatever scale settings you choose apply to the selected clip, or — when nothing is selected — to whatever clips you create next.

The Scale Mode Toggle and Scale Choosers in the Clip View.

Whatever scale settings any selected clip carries are reflected by the Scale Mode controls on the Control Bar. Those same controls can flip Scale Mode on/off or assign one shared scale across several selected clips at once.

Scale Options in the Control Bar.

Inside the Clip View, switching on Scale Mode causes the [Fold to Scale and Highlight Scale options](https://www.ableton.com/en/live-manual/12/editing-midi/#folding-and-scales) to surface in [the MIDI Note Editor](https://www.ableton.com/en/live-manual/12/editing-midi/#the-midi-note-editor-layout). With Fold to Scale switched on, the editor presents only the key tracks tied to notes within the scale. With Highlight Scale switched on, those scale-note key tracks get tinted purple — the hue that marks scale awareness right across Live.

While a scale is in force, every pitch-related parameter throughout MIDI Tools and the Pitch and Time Utilities panel adopts that chosen scale as well.

A Use Current Scale toggle appears in the device title bars of Live's [Arpeggiator](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#arpeggiator), [Chord](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#chord), [Pitch](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#pitch), [Random](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#random), and [Scale](https://www.ableton.com/en/live-manual/12/live-midi-effect-reference/#scale) MIDI effects. Flip it on and the clip's active scale takes hold, with pitch-based device parameters then tunable in scale degrees instead of semitones.

You can likewise switch on scale awareness for [Auto Shift's](https://www.ableton.com/en/live-manual/12/live-audio-effect-reference/#auto-shift) Quantizer and for the oscillators and filters of [Meld](https://www.ableton.com/en/live-manual/12/live-instrument-reference/#meld).

<a id="source-314-the-mixer"></a>
### 3.14 The Mixer

Picture an audio clip sounding on an audio track. That clip's audio signal arrives at the chain's leftmost device. After that device alters the signal, it passes the outcome along to the device that follows, and so the chain continues. In theory there's no cap on how many devices a track may hold. Practically, though, your computer's available power sets a ceiling on how many devices run together at once — a matter worth its own [separate discussion](https://www.ableton.com/en/live-manual/12/computer-audio-resources-and-strategies/#managing-the-cpu-load). Bear in mind that audio devices always connect to one another in stereo, yet the software's inputs and outputs may be set to mono within the Audio Settings.

<a id="source-live-concepts-part-2"></a>

After a signal travels through the device chain, its final stop is Live’s [mixer](https://www.ableton.com/en/live-manual/12/mixing/#the-live-mixer). Because the same pool of tracks underlies both the Session and the Arrangement, those views rely on a single shared mixer too. For convenience, that mixer is available from either view.

The Live Mixer shown within the Arrangement View.

You can declutter the screen by toggling each mixer section on or off — either through the Mixer Controls entries under the View menu or via the choices in the Mixer Config Menu tucked into the lower right of Live’s window.

The options found in the Mixer Config Menu.

Among the mixer’s controls are volume, pan position, and _sends_, the last of which set how large a portion of a track’s output is routed into the matching _return track’s_ input. A return track holds effects exclusively — never clips. Through their sends, every track is able to route some of its signal toward a return track and tap into the effects it carries.

Built into the mixer as well is a [crossfader](https://www.ableton.com/en/live-manual/12/mixing/#using-lives-crossfader) for blending seamlessly between clips that play across separate tracks. Although Live’s crossfader behaves much like the crossfader on a standard DJ mixer, it goes further by letting you blend across any quantity of tracks rather than only two — the returns included.

The Crossfader and the buttons that assign tracks to it.

Picture a MIDI track running a clip. That clip’s MIDI signal flows into the device chain belonging to the track. Inside, it first encounters however many MIDI effects sit there. Each MIDI effect takes in MIDI and passes MIDI back out. After the final MIDI effect comes an instrument, which accepts MIDI and produces audio. Beyond the instrument you may place any quantity of audio effects, just like on an audio track.

A MIDI Effect, an Instrument and a few Audio Effects within a MIDI Track.

When a MIDI track carries neither an instrument nor any audio effects, its output stays a bare MIDI signal that must be routed elsewhere before it can turn into audio. Under those circumstances, the mixer no longer displays that track’s mix and send controls.

The Mixer as it appears for a MIDI Track lacking an Instrument.
